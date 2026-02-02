<strong><em><font color=red size=5>该版本 API 已停止更新，以下 API 将在一段时间后删除，请参考最新版本： [APIDoc v2](p/APIDoc_v2.md)</font></em></strong>

本页面为 MCSR Ranked 数据库的 API 文档，供开发者参考使用。

> MCSR Ranked 数据库包含了历史上所有 MCSR 排位赛的比赛、玩家详细信息以及 2025 年 11 月 13 日起的约 80% 的实际种子信息，该 API 目前主要提供对实际种子信息的获取功能

## 目录

- [概述](#概述)
- [端点](#端点)
  - [获取最小 id 的 n 条数据（最大 10 条）](#获取最小id的n条数据最大10条)
  - [获取指定 id 的数据](#获取指定id的数据)
  - [获取并删除最小 ID 的种子数据](#获取并删除最小-id-的种子数据)
  - [获取并删除满足条件的最小 ID 的种子数据](#获取并删除满足条件的最小-id-的种子数据)
  - [数据库剩余种子信息](#数据库剩余种子信息)
- [错误码](#错误码)
- [限流](#限流)

## 概述

**基础信息**

- **Base URL**: `http://43.143.231.104:8000/api/`
- **数据格式**: JSON
- **编码**: UTF-8

## 端点

### 1. 获取最小 id 的 n 条数据（最大 10 条）

返回数据库中最小 id 的 n 条种子数据，n 最大值为 10。

**端点**

```
http://43.143.231.104:8000/api?count={count}
```

**参数**

| 参数  | 类型    | 必需？ | 描述                            |
| :---- | :------ | :----- | :------------------------------ |
| count | Integer | true   | 返回种子数据的数量，最大值为 10 |

**请求示例**

```
http://43.143.231.104:8000/api?count=3
```

**返回示例**

```json
{
  "success": true,
  "message": "获取到3条数据",
  "count": 3,
  "data": [
    {
      "id": 3651799,
      "overworld": "SHIPWRECK",
      "nether": "BRIDGE",
      "end_towers": "[100, 79, 82, 91]",
      "variations": "[\"chest:structure:carrot\", \"biome:structure:deep_ocean\", \"type:structure:normal\", \"chest:structure:carrot\", \"biome:structure:deep_ocean\", \"type:structure:normal\", \"bastion:triple:1\", \"bastion:single:1\", \"biome:bastion:nether_wastes\", \"biome:fortress:nether_wastes\", \"end_tower:caged:front_center\", \"end_tower:caged:back\"]",
      "overworldSeed": "599175178330882171",
      "netherSeed": "234064443581912",
      "theEndSeed": "599175178330882171"
    },
    {
      "id": 3651804,
      "overworld": "SHIPWRECK",
      "nether": "BRIDGE",
      "end_towers": "[82, 103, 94, 100]",
      "variations": "[\"chest:structure:carrot\", \"biome:structure:deep_ocean\", \"type:structure:full\", \"chest:structure:carrot\", \"biome:structure:deep_ocean\", \"type:structure:full\", \"bastion:triple:1\", \"bastion:single:1\", \"biome:bastion:nether_wastes\", \"biome:fortress:nether_wastes\", \"end_tower:caged:front\"]",
      "overworldSeed": "-3287507984166956424",
      "netherSeed": "208265525993114",
      "theEndSeed": "-3287507984166956424"
    },
    {
      "id": 3651808,
      "overworld": "SHIPWRECK",
      "nether": "BRIDGE",
      "end_towers": "[100, 79, 91, 94]",
      "variations": "[\"chest:structure:carrot\", \"biome:structure:deep_ocean\", \"type:structure:sideways\", \"chest:structure:carrot\", \"biome:structure:deep_ocean\", \"type:structure:sideways\", \"bastion:triple:1\", \"bastion:single:1\", \"biome:bastion:warped_forest\", \"biome:fortress:nether_wastes\", \"end_tower:caged:front_center\"]",
      "overworldSeed": "927822452312523127",
      "netherSeed": "261207410001954",
      "theEndSeed": "927822452312523127"
    }
  ]
}
```

### 2. 获取指定 id 的数据

返回数据库中指定 id 的种子数据。

**端点**

```
http://43.143.231.104:8000/api?id={id}
```

**参数**

| 参数 | 类型    | 必需？ | 描述              |
| :--- | :------ | :----- | :---------------- |
| id   | Integer | true   | Ranked 的 MatchID |

**请求示例**

```
http://43.143.231.104:8000/api?id=3651804
```

**返回示例**

```json
{
  "success": true,
  "message": "数据获取成功",
  "data": {
    "id": 3651804,
    "overworld": "SHIPWRECK",
    "nether": "BRIDGE",
    "end_towers": "[82, 103, 94, 100]",
    "variations": "[\"chest:structure:carrot\", \"biome:structure:deep_ocean\", \"type:structure:full\", \"chest:structure:carrot\", \"biome:structure:deep_ocean\", \"type:structure:full\", \"bastion:triple:1\", \"bastion:single:1\", \"biome:bastion:nether_wastes\", \"biome:fortress:nether_wastes\", \"end_tower:caged:front\"]",
    "overworldSeed": "-3287507984166956424",
    "netherSeed": "208265525993114",
    "theEndSeed": "-3287507984166956424"
  }
}
```

### 3. 获取并删除最小 ID 的种子数据

返回并删除最小 ID 的种子数据。

**端点**

```
http://43.143.231.104:8000/api/seed
```

**返回示例**

```json
{
  "success": true,
  "message": "种子数据获取并删除成功",
  "deleted_id": 3651205,
  "data": {
    "id": 3651205,
    "overworldSeed": "1463813851565049564",
    "netherSeed": "170390546644921",
    "theEndSeed": "1463813851565049564"
  }
}
```

### 4. 获取并删除满足条件的最小 ID 的种子数据

返回并删除满足指定主世界和下界堡垒遗迹类型的最小 ID 的种子数据，可仅传入其中一个参数以进行单条件筛选。

**端点**

```
http://43.143.231.104:8000/api/seed?overworld={overworldType}&nether={netherType}
```

**参数**

| 参数          | 类型   | 必需？ | 描述                                                                                              |
| :------------ | :----- | :----- | :------------------------------------------------------------------------------------------------ |
| overworldType | String | false  | 主世界类型（可选值：`village`、`desert_temple`、`shipwreck`、`ruined_portal`、`buried_treasure`） |
| netherType    | String | false  | 下界堡垒遗迹类型（可选值：`bridge`、`treasure`、`housing`、`stables`）                            |

**请求示例**

```
http://43.143.231.104:8000/api/seed?overworld=village&nether=bridge
```

**返回示例**

```json
{
  "success": true,
  "message": "种子数据获取并删除成功",
  "deleted_id": 3651211,
  "data": {
    "id": 3651211,
    "overworldSeed": "896232095842398803",
    "netherSeed": "87400885019801",
    "theEndSeed": "896232095842398803"
  }
}
```

### 5. 数据库剩余种子信息

可以通过以下端点查询数据库中剩余的种子信息数量。

**端点**

```
http://43.143.231.104:8000/api/stats
```

**返回示例**

```json
{
  "success": true,
  "message": "数据库统计信息",
  "stats": {
    "total_records": 188779,
    "id_range": {
      "min": 3651219,
      "max": 3910225
    },
    "seed_data_available": {
      "overworldSeed": 188779,
      "netherSeed": 188779,
      "theEndSeed": 188779
    }
  }
}
```

---

# **Feinberg - 玩家战绩数据**

## 🔥 **核心数据**

| 项目     | 数据                                                |
| :------- | :-------------------------------------------------- |
| 当前排名 | **<strong><font color=red>#2</font></strong>**      |
| 当前 Elo | **<strong><font color=orange>2215</font></strong>** |
| 赛季胜率 | **<strong><font color=green>68%</font></strong>**   |
| 连胜场次 | **<strong><font color=blue>6 连胜</font></strong>** |

## 📊 **本赛季详细数据**

| 项目                 | 数值                                 |
| :------------------- | :----------------------------------- |
| 赛季最高 Elo         | **<font color=orange>2215</font>**   |
| 赛季平均完赛时间     | **<font color=green>9分36秒</font>** |
| 排位历史最佳完赛时间 | **<font color=gold>6分48秒</font>**  |
| 最近比赛时间         | 2026-01-22 09:45:31                  |

## 📌 **快捷查询指令**

- **查看玩家详细数据** → `/rankedDataDetail`
- **查看玩家历史排位记录** → `/rankedMatch`
