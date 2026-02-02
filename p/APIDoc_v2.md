本页面为 MCSR Ranked 数据库的 API 文档 (v2)，供开发者参考使用。

<strong><font color=green>若要使用图形化筛种界面，请访问 [MCSR Ranked 种子查询工具](http://43.143.231.104:8080/)（待完善）。</font></strong>

> MCSR Ranked 数据库包含了历史上所有 MCSR 排位赛的比赛、玩家详细信息以及 2025 年 11 月 13 日起的约 80% 的实际种子信息，该 API 目前主要提供对实际种子信息的获取功能

## 目录

- [概述](#概述)
- [端点](#端点)
  - [随机获取一条种子数据](#_1-随机获取一条种子数据)
  - [随机获取满足条件的一条种子数据](#_2-随机获取满足条件的一条种子数据)
  - [根据比赛 ID 获取种子值](#_3-根据比赛-id-获取种子值)
  - [根据比赛 ID 获取种子详细信息](#_4-根据比赛-id-获取种子详细信息)
  - [Multiseed 公告获取](#_5-multiseed-公告获取)
- [变种类型](#变种类型)
- [功能前瞻](#功能前瞻)

## 概述

**基础信息**

- **Base URL**: `http://43.143.231.104:8001/api/v2/`
- **数据格式**: JSON
- **编码**: UTF-8

## 端点

### 1. 随机获取一条种子数据

返回随机 ID 的种子数据并显示满足条件的种子数量。

**端点**

```
http://43.143.231.104:8001/api/v2/seed
```

**返回示例**

```json
{
  "success": true,
  "message": "随机获取一条种子数据",
  "data": {
    "id": 4620828,
    "overworldSeed": "2260873127213409737",
    "netherSeed": "7415146110041",
    "theEndSeed": "2260873127213409737",
    "availableCounts": 1039488
  }
}
```

### 2. 随机获取满足条件的一条种子数据

返回满足指定条件的随机一条种子数据，并显示满足条件的种子数量。

**端点**

```
http://43.143.231.104:8001/api/v2/seed?overworld={overworldType}&nether={netherType}&variations={variationType}&without={withoutType}&completion={completionTime}
```

**参数**

| 参数           | 类型    | 必需？ | 描述                                                                                                                                                                                                    |
| :------------- | :------ | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| overworldType  | String  | false  | 主世界类型（可选值：`village`、`desert_temple`、`shipwreck`、`ruined_portal`、`buried_treasure`）                                                                                                       |
| netherType     | String  | false  | 下界堡垒遗迹类型（可选值：`bridge`、`treasure`、`housing`、`stables`）                                                                                                                                  |
| variationType  | String  | false  | 变种类型，可以同时指定多个变种，用逗号分隔，API 将返回 <strong><em>同时满足所有提供的变种条件</em></strong> 的种子，详细的变种类型及说明见[变种类型](#变种类型)部分                                     |
| withoutType    | String  | false  | 排除类型，可以同时指定多个排除类型，用逗号分隔，API 将返回 <strong><em>不包含任何提供的排除类型</em></strong> 的种子，详细的排除类型及说明见[变种类型](#变种类型)部分                                   |
| completionTime | Integer | false  | 原比赛完成时间上限<strong><font color=green>（单位：毫秒）</font></strong>[ 注：若 API 请求包含 completion 参数，则只返回 <strong><em>排位模式</em></strong> 且原比赛完成时间小于等于给定毫秒数的种子 ] |

**请求示例**

返回满足主世界类型为平原村庄且不包含足够多的黑曜石、堡垒遗迹类型为桥且左右均为三箱好塔，末地出生平台为封闭类型，且原比赛完成时间不超过 12 分钟的随机种子数据：

```
http://43.143.231.104:8001/api/v2/seed?overworld=village&nether=bridge&variations=biome:structure:plains,bastion:triple:2,end_spawn:buried&without=chest:structure:obsidian&completion=720000
```

**返回示例**

```json
{
  "success": true,
  "message": "随机获取满足条件的一条种子数据",
  "data": {
    "id": 4365315,
    "overworldSeed": "306273042741578200",
    "netherSeed": "33111158928462",
    "theEndSeed": "306273042741578200",
    "availableCounts": 140
  }
}
```

### 3. 根据比赛 ID 获取种子值

根据输入的比赛 ID，返回比赛时间及三个世界（主世界、下界、末地）的种子值。

注：只能获取排位模式、休闲模式和房主有铁镐及以上会员等级的私人房间的种子值，包含大约 80% 的历史比赛种子数据信息。该数据通常在比赛结束后 30 分钟内生成并存入数据库。

**端点**

```
http://43.143.231.104:8001/api/v2/seed/{matchId}
```

**参数**

| 参数    | 类型    | 必需？ | 描述                      |
| :------ | :------ | :----- | :------------------------ |
| matchId | Integer | 是     | 比赛 ID（不小于 3650001） |

**请求示例**

```
http://43.143.231.104:8001/api/v2/seed/5100003
```

**返回示例**

```json
{
  "success": true,
  "message": "获取ID为 5100003 的种子数据",
  "data": {
    "matchId": 5100003,
    "matchDate": 1768584208825,
    "seeds": {
      "overworldSeed": "2265576970181489816",
      "netherSeed": "274576943635675",
      "theEndSeed": "2265576970181489816"
    }
  }
}
```

### 4. 根据比赛 ID 获取种子详细信息

根据输入的比赛 ID，返回种子的详细信息。

注：该 API 能获取几乎所有比赛的种子详细信息，但由于数据上传需要人工处理，故可能有数天的延迟。

**端点**

```
http://43.143.231.104:8001/api/v2/seedinfo/{matchId}
```

**参数**

| 参数    | 类型    | 必需？ | 描述                     |
| :------ | :------ | :----- | :----------------------- |
| matchId | Integer | 是     | 比赛 ID（不小于 100876） |

**请求示例**

```
http://43.143.231.104:8001/api/v2/seedinfo/3650001
```

**返回示例**

```json
{
  "success": true,
  "message": "获取ID为 3650001 的种子数据",
  "data": {
    "matchId": 3650001,
    "overworld": "VILLAGE",
    "nether": "BRIDGE",
    "end_towers": "[76, 79, 85, 97]",
    "variations": "[\"biome:structure:plains\", \"biome:structure:plains\", \"bastion:triple:1\", \"bastion:single:1\", \"biome:bastion:nether_wastes\", \"biome:fortress:crimson_forest\", \"end_spawn:buried:56\", \"end_tower:caged:front_center\"]"
  }
}
```

### 5. Multiseed 公告获取

获取 Multiseed 模组的最新公告内容。

Multiseed 模组由 [fredoseep](https://github.com/fredoseep) 开发，用于定向筛选 [MCSR Ranked](https://mcsrranked.com/) 历史种子并辅助速通练习。

具体信息及下载链接见：[MultiSeedmod-for-Minecraft-fabric](https://github.com/fredoseep/MultiSeedmod-for-Minecraft-fabric)。

**端点**

```
http://43.143.231.104:8001/api/v2/multiseed/info
```

**返回示例**

```json
{
  "success": true,
  "message": "获取 Multiseed mod 公告信息",
  "data": "本次更新新增对于各结构细节变种类型的筛选功能以及输入 Match ID 获取对应种子数据的功能。"
}
```

## 变种类型

```
Overworld:
	- Village:
			biome:structure:desert
			biome:structure:plains
			biome:structure:savanna
			biome:structure:snowy_tundra
			biome:structure:taiga
			chest:structure:diamond
			chest:structure:obsidian
	- Desert Temple:
			chest:structure:diamond
			chest:structure:egap
	- Ruined Portal:
			chest:structure:egap
			chest:structure:golden_carrot
			chest:structure:looting_sword
			type:structure:completable
			type:structure:lava
	- Shipwreck:
			chest:structure:carrot
			chest:structure:diamond
			type:structure:normal
			type:structure:sideways
			type:structure:upsidedown
	- Buried Treasure:
			(无变种)

Bastion:
	biome:bastion:basalt_deltas
	biome:bastion:crimson_forest
	biome:bastion:nether_wastes
	biome:bastion:soul_sand_valley
	biome:bastion:warped_forest
	- Bridge:
			bastion:single:1
			bastion:single:2
			bastion:triple:1
			bastion:triple:2
	- Treasure:
			(无变种)
	- Housing:
			bastion:single:1
			bastion:triple:1
			bastion:triple:2
	- Stables:
			bastion:good_gap:1
			bastion:good_gap:2
			bastion:single:1 (双箱塔)
			bastion:single:2 (双箱塔)
			bastion:single:3 (双箱塔)
			bastion:small_single:1 (单箱塔)
			bastion:small_single:2 (单箱塔)
			bastion:small_single:3 (单箱塔)
			bastion:triple:1
			bastion:triple:2
			bastion:triple:3

Fortress:
	biome:fortress:basalt_deltas
	biome:fortress:crimson_forest
	biome:fortress:nether_wastes
	biome:fortress:soul_sand_valley
	biome:fortress:warped_forest

End:
	end_tower:caged:back
	end_tower:caged:back_center
	end_tower:caged:front
	end_tower:caged:front_center
	end_spawn:buried:xx (xx为20到64的任意数值)
```

## 功能前瞻

- 添加零循环塔和前后龙的筛选功能
- 利用 Elo 和完赛时间拟合种子的好坏程度
