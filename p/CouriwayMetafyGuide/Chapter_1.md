这一节的内容大部分是由Draconix编写的，他是一名顶尖的玩家，主榜审核员，还是 [MC Speedrun.com](https://speedrun.com/mc) 网页的主管。多亏有了他，否则不会出现这篇指南。请观看下面的视频来开启你的mc速通之旅。

<iframe width="720" height="500" src="https://www.youtube.com/embed/RSLv7FfQZKY" title="How to setup Minecraft for Speedrunning - A comprehensive guide" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

所有在视频提及到的网页链接

[Prism Launcher](https://prismlauncher.org/)
[ModCheck](https://github.com/tildejustin/modcheck/releases/latest)
[Jarfix](https://johann.loefflmann.net/en/software/jarfix/)

[SeedQueue设置网页](http://maskers.xyz/sq-settings)
[SeedQueue wiki](https://github.com/contariaa/seedqueue/wiki/)

[MCSR Practice Map](https://github.com/Dibedy/The-MCSR-Practice-Map/releases/latest)
[MiniPracticeKit](https://github.com/Knawk/mc-MiniPracticeKit/raw/master/hotbar.nbt)

[Ninjabrain Bot](https://github.com/Ninjabrain1/Ninjabrain-Bot/releases/latest)
[Jingle](https://github.com/DuncanRuns/Jingle/releases/latest)
[更多关于Jingle的消息](https://github.com/DuncanRuns/Jingle)

完美灵敏度（船测）设置：

<iframe width="720" height="500" src="https://www.youtube.com/embed/l1Z2t9e6Qko" title="Boat Eye Setup Guide for Minecraft Speedrunning (Updated 2026)" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

在Speedrun.com提交成绩：

<iframe width="720" height="500" src="https://www.youtube.com/embed/z2n2fCV1GY0" title="How to Submit Minecraft: Java Edition Speedruns" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

下载OBS Studio: [OBS Studio](https://obsproject.com/)

JAVA版MCSR Discord服务器 (Javacord): [Discord服务器](https://discord.com/invite/jmdFn3C)

这些文本是作为上面视频的详细解释，建议先观看完上面视频。

这节是关于如何最好设置MC速通，其中包括练习图、工具以及尽可能去设置好你的配置的教程。这些步骤不是必需但还是极其建议，我们的目标是让你有个最佳的游玩经历，在正确的步骤上提升自己并在游戏中取得一个好成绩。

> 如果你对这部分指南有任何疑惑，或者无法解决的问题，请在页面底下查找FAQ部分，或者在Java版MCSR Discord服务器的#public-help频道寻求帮助。

Java版MCSR Discord服务器: [Discord服务器](https://discord.com/invite/jmdFn3C)
本指南以Windows平台为基础编写。

Linux用户务必要遵循在这里所有教程，在教程中会Linux会出现的小问题在[这里](https://its-saanvi.github.io/linux-mcsr)

在最初的游戏设置，Mac用户可以先跟着视频12:30前的教程设置。之后照着下面的"设置"开始设置，或者从上方的视频开始。

## 版本和种类

这些是1.16.1版本的设置。这个版本一般来说是最快和最容易上手Any% 随机种（RSG）的版本，因此也是个竞争最激烈的项目。很大程度是因为相比以后的版本，猪灵有更高的几率交易出末影珍珠，并且没有猪灵蛮兵。

在指南中的任何关于设置的指导方法是为了 [speedrun.com](https://speedrun.com/mc) 排行榜取得成绩。如果你对 [MCSR Ranked](https://mcsrranked.com) 感兴趣，虽然这里并没有关于MCSR Ranked的设置教程，但下面的教程依旧很重要。

## 需要什么？

运行Java版MC，你需要：

- Java
- 一个MC启动器

这两样都有不同的版本，哪怕其中一样使用不同的版本也会直接影响你的游戏性能（很容易去改善这种情况）。

还需要安装Fabric加载器来使用一些合法的mod，来提升性能和获得更好的游玩体验。

对于练习，要下载练习地图和工具来练习如何去使用它们。也包括一些允许在速通中使用的工具。

## 运行游戏

可以从 [minecraft.net](https://minecraft.net/) 下载官方（原版）启动器，同时也很容易起步，但是如果要更新Java版本并不简单，并且缺少其他启动器拥有的便捷功能，所以并不建议使用官方启动器来速通。
下面是 [speedrun.com](https://speedrun.com/mc) 排行榜所认可的启动器：

- 官方Minecraft启动器
- MultiMC
- Prism Launcher
- Modrinth App
- ATLauncher
- MCSR Launcher

在这些启动器中，推荐使用 [Prism Launcher](https://prismlauncher.org/)，其便于使用且拥有很多功能，适配了大多数的硬件和软件（包括Linux系统和较新版本的Mac系统）。如果你已经使用了上述的启动器，无需改动，但这里只包含Prism Launcher的教程（请注意Prism Launcher是MultiMC的衍生版，两者十分相似）。

你可以在 [这里下载 Prism Launcher](https://prismlauncher.org/)。下载并运行安装器，安装完毕后打开Prism，照着下面的简单步骤设置，到达下方所示界面。

![image](/image/ch1/1.png)

然后点击左上角的"添加实例"按钮，选择1.16.1版本，还要在底部勾选Fabri mod加载器。

![image](/image/ch1/2.png)

在运行游戏之前，需要设置使用较新版本的Java来获取更好的性能表现。在Prism窗口的顶部，点击"设置"，然后选择"Java"，可以在这里选择"跳过Java兼容性检测"和取消"自动检测Java版本"。

![image](/image/ch1/3.png)

然后点击"自动检测"一栏，在新弹出的窗口中，选择在17到22的任一Java版本。

![image](/image/ch1/4.png)

如果在列表中没有合适的版本，关闭窗口，然后选择"管理"一栏。

![image](/image/ch1/5.png)

在右侧点击"下载"，在新开的窗口中，在"主版本"一栏中选择"Java 21"，然后选择在右侧列表中选择最新的版本并点击"下载"。

![image](/image/ch1/6.png)

之后，回去"通用"一栏，重新检查"自动检测"列表，确认您新下载的Java版本是否在其中。
选择了Java版本后，关闭设置窗口。然后，请双击实例以启动游戏。

![image](/image/ch1/7.png)

## 设置

打开游戏后，打开"选项"，设置你的偏好。检查"控制"（热键、鼠标灵敏度、禁用自动跳跃）、"音乐和声音"（开启显示字幕）和"视频设置"（最大帧率为250fps、关闭垂直同步、实体渲染距离：500%）

### 从另一个启动器迁移

如果你想要从另外一个启动器复制你的设置，用那个启动器打开游戏后点击options（选项），然后 Resource Pack（资源包），然后点击Open Packs Folder（打开资源包文件夹）。然后，回到上一个文件夹前往".minecraft"。从这里，复制"options"或者"options.txt"。

![image](/image/ch1/8.png)

把这个文件复制到新的实例上。首先，确保游戏已关闭，然后在Prism右键你的实例，选择并打开名称为".minecraft"的文件夹，删除现有的"options"文件，并粘贴先前在另一个启动器的"options"文件。

## 快捷键

在速通当中，使用快捷键是极其重要的，根据你对速通的投入程度，来考虑是否值得优化操作控制方案。
即便每个人都有自己的快捷键偏好，还是建议至少为9个快捷栏设置成易于操作的键位，通常的选择有Z, X, C, V, F和R，你可以尝试一下。此外，还要知道还有很多键用于重置和宏，这些键也要便于触碰，常用的键位有G, B, T, Y,和H。但大多数玩家会设置成较远的地方，以免在速通的过程中造成误触。

最后，特别要考虑为"副手操作键"（Offhand）或"F3 功能键"设置快捷键。鼠标侧键是非常理想的选择，原因在于：当你的主手正在操作键盘进行复杂组合时，用副手（鼠标）的侧键来触发这些关键功能，可以最大限度地避免按键冲突，实现高效并行操作。

### AutoHotkey

由于F3菜单最初是用于开发目的，Mojang并未像其他按键一样给F3提供重绑选项。如果没有键盘制造商提供的专用驱动软件，在Windows系统上可以用一款名为 AutoHotkey 的应用程序来实现此功能。

[下载AutoHotkey V1.1](https://www.autohotkey.com)，使用其他版本可能会失效。

AutoHotkey安装完毕后，在桌面空白处点击鼠标右键，依次选择 "新建" → "AutoHotkey Script"，即可创建一个新的脚本文件。

![image](/image/ch1/9.png)

然后右键新的脚本文件，选择编辑脚本。
当文本编辑器打开时，复制以下文本

```json
#IfWinActive Minecraft
*F3::r
*r::F3
```

然后同时按下Ctrl和S保存文件，关闭文本编辑器，并双击脚本运行。

使用这段 AutoHotkey 脚本，即可将 R键的功能重绑定为 F3键。若您希望使用 R 以外的按键，只需将脚本第2、3行中的 r 替换为其他按键字符即可。所有可用的按键名称与代码，请参阅 [AutoHotkey官方文档的按键列表页面](https://www.autohotkey.com/docs/v1/KeyList.html/)

现在，双击 rebind.ahk 文件以运行该 AutoHotkey 脚本。运行后，当您游玩MC时，按下R键即可打开F3菜单。若需修改脚本，请右键点击 rebind.ahk 文件，选择 "Edit Script"。编辑完成后，请务必保存文件，并再次双击运行以使更改生效。

若要恢复游戏默认键位，请在Windows的系统托盘中找到绿色的 "H" 图标。右键点击该图标，选择 "Exit" 即可退出脚本。

![image](/image/ch1/10.png)

### 重绑规则

可以使用外部程序来重新映射按键，但是:

- 每个游戏操作只能绑定至一个按键，每个按键只能触发一个游戏操作。
- 不得将任何F3组合键（例如 F3+C、Shift+F3 等）绑定至单个按键。
- 所有输入必须由按键触发。禁止使用鼠标滚轮滚动、鼠标移动或类似连续信号作为操作输入。
- 严禁将"攻击/摧毁"或"使用物品/放置方块"绑定至键盘按键，防止使用连点器。

## 模组

现在，需要安装和设置合法的速通模组，可以使用一个叫做 [ModCheck](https://github.com/tildejustin/modcheck/releases/latest) 的工具，在页面顶部附近找到.jar 文件的下载链接。

![image](/image/ch1/11.png)

下载好之后，右键尝试运行，假如你并没有看到ModCheck如下方图片所示，[下载并运行Jarfix](https://johann.loefflmann.net/en/software/jarfix/)，之后，再次尝试运行ModCheck。

![image](/image/ch1/12.png)

使用ModCheck之前，首先需要为其配置MC游戏实例的路径。返回Prism，右键实例并选择文件夹，然后像这样点击顶部的地址栏来复制路径：

![image](/image/ch1/13.png)

在ModCheck,点击"选择实例路径"，将复制的路径粘贴在 "Folder name" 下方，然后点击选择。

![image](/image/ch1/14.png)

最后，在左侧选择您的操作系统，点击 "Select All Recommends"，然后点击 "Download" 即可。若不确定模组是否为最新版本，只需重新运行 ModCheck 工具即可自动检查并更新。

### 模组设置

现在，当你在Prism重启MC时，你可以在选项界面看到图标为"书与笔"的按钮

![image](/image/ch1/15.png)

在这里可以调整一些模组的选项，在这些模组中，你绝对要懂得使用StandardSettings和 SeedQueue这两个模组。

### StandardSettings

当你每次创建新的世界时，StandardSettings会自动把你的游戏内设置重置为预设状态，这意味着你每次都能以完全相同的配置开始，从而节省了在每次运行前反复检查、调整设置所耗费的时间。若您想修改重置后的预设配置，应在StandardSettings 界面中进行更改。

若你不希望使用此功能，可通过右侧按钮将特定设置切换为关闭，这样在每次创建新世界时，这些设置便不会被重置。也可以直接点击顶部的 "Use StandardSettings" 按钮，将StandardSettings模组完全禁用。

如果你找不到在StandardSettings里面想要调整的选项，可以按下Ctrl+F来进行搜索。在搜索栏里输入"亮度"并把其调整到500%。如果禁用了StandardSettings，可以在常规的"视频设置"里调整你的亮度。

![image](/image/ch1/16.png)

当你浏览设置界面时，会发现有额外的选项设置在底部，可以根据你的偏好决定是否启用和配置，此处有一项建议您设置为 ON，即 F3 Pause On World Load，这将显著改善你在预览界面中的视野范围。

### SeedQueue

SeedQueue可以同时创建多个新的世界和展示种子的墙界面以便于挑选。当你想更进一步，想筛选出更佳的种子时，我们强烈建议进行此模组的配置。否则，你可以选择直接跳至下方"重置操作"部分继续阅读。

首先，我们将为你的计算机找到一些基准设置。最佳方式是进入 Prism，右键单击实例，点击"编辑"，再点击"复制"。如果点击"编辑"后未看到日志，则说明游戏未启动——请通过 Prism 启动游戏后重试。

![image](/image/ch1/17.png)

然后，访问此网页：[http://maskers.xyz/sq-settings](http://maskers.xyz/sq-settings)。将你的日志粘贴到框中，并点击 "推荐设置"，随后您将看到如下所示的信息：

![image](/image/ch1/18.png)

在游戏中，进入书与笔菜单下的 "SeedQueue" 选项。在此处，将前三个数值修改为与网页上给出的建议值一致。以上文示例为例，SeedQueue的设置应调整如下：

![image](/image/ch1/19.png)

将鼠标悬停在左侧的标签上即可查看其余SeedQueue选项的说明。以下列出几项应调整的设置及其原因（在你学会如何使用SeedQueue后，会更容易理解这些设置的解释）：

- "最大世界加载进度%"调整为15%.
  > 这项设置将使种子的加载在达到 15% 后暂停，除非你将其锁定，这意味着你的计算机将仅加载你挑选的种子。
- 开启"恢复世界加载".
  > 该功能将绕过"最大世界生成百分比"选项——当所有队列中的种子均生成至 15%，且任何被锁定的种子已完全加载后，SeedQueue将继续加载剩余的种子，以便在您返回"种子墙"时，所有可能的好种子均已准备就绪。
- 开启"使用墙界面"
  > 该选项将启用先前展示的种子网格视图。
- 开启"跳过墙界面"
  > 当您尝试在游玩某个种子后返回种子墙时，SeedQueue 会自动检查您先前锁定的其他实例，并跳转至那些实例处。这一机制能提高效率。

然后，返回Prism启动器，右键点击你的实例，选择"编辑"，接着在左侧选择"设置"。勾选"内存"选项，并将"最大内存分配"修改为网站建议的数值。以上文示例为例，应将其设置为9500MB。

最后，在网站上复制 "Java 参数：" 下方的整段文本。返回Prism的设置窗口，勾选 "Java 参数" 选项，并将复制的文本粘贴到下方的输入框中。

![image](/image/ch1/20.png)

现在，关闭并重新启动游戏，以使上述更改生效。

若需进一步提升性能，网站可能会提供一些优化建议与提示，您可以根据需要自行选择是否采纳，例如：

![image](/image/ch1/21.png)

您也可以 [阅读这份指南以获取更多优化建议](https://gist.github.com/maskersss/5847d594fc6ce4feb66fbd2d3fda281d)。

## Resetting

在标题界面，你可以看见金靴子图标的按钮——点击后即可开始速通。世界加载完成后，你可以在屏幕角落看见计时器。

![image](/image/ch1/22.png)

RTA代表真实时间——这是从开始到结束的完整实际用时。IGT代表游戏内时间——此时间不计入所有加载界面和暂停的时间。[speedrun.com](https://speedrun.com/mc) 排行榜按IGT对成绩进行排序，因此玩家不会因电脑性能的差异而受到影响。

可以按F6键来reset当前种子，如果你已经开启了"使用墙界面"，你会返回到墙界面。

在墙界面上，将鼠标悬停于某个种子上并按 L键可将其锁定。随后，可以按T键来reset其余种子。被锁定的种子将继续加载——您的重置流程应为：先锁定较好的种子，然后重置其余所有种子。被锁定的种子加载速度会更快。当您准备进入某个种子时，其加载完成后，把鼠标悬停于其并按下R键。

如果你想更改在墙界面上使用的快捷键，请在SeedQueue设置中的"按键设置"进行调整。若需更改当前重置实例键（默认为 F6），请在StandardSettings中搜索并修改 "创建新的世界" 对应的按键。如需进一步了解SeedQueue及其自定义设置，请查阅 [SeedQueue Wiki](https://github.com/contariaa/seedqueue/wiki)。

Reset是一项重要的操作，且当你的目标越高，其重要性将呈指数级增长——本指南的"主世界"章节将对reset操作进行更详细的讲解。然而，请务必谨记：享受过程是第一位的。过度强求重置效率可能导致身心疲劳，这不仅会影响您的操作表现，甚至可能让你彻底失去对速通的热情。

## 练习

现在游戏内的所有设置均已完成，接下来可以开始学习速通的基本路线。当前速通路线的大致框架如下：

- 携带一把铁镐和桶进入下界
- 找到堡垒遗迹（以下简称"猪堡"）并规划路线来获取末影珍珠、线、黑曜石和抗火药水
- 找到下界要塞，通过杀死烈焰人获得烈焰棒，合成末影之眼
- 离开下界，使用末影之眼定位要塞r
- 返回下界，搭建传送至要塞的传送门，并找到通往末地的传送门
- 利用爆炸物来迅速击败末影龙

最好使用练习图和工具来进行练习。

### 地图

首先下载 [MCSR Practice Map练习图](https://github.com/Dibedy/The-MCSR-Practice-Map/releases/latest)，点击此.zip链接。

![image](/image/ch1/23.png)

下载完毕后，右键此.zip文件并点击"全部解压缩"，在出现的窗口中点击"解压"，完成后，你可以在.zip文件旁边看见这个文件：

![image](/image/ch1/24.png)

接下来，请在Prism中定位到 Minecraft 的世界存档文件夹。在Prism中右键点击您的游戏实例，选择 "打开文件夹"。然后，依次打开 ".minecraft" 文件夹和其中的 "saves" 文件夹。

把MCSR.Practice的文件夹移动到"saves" 文件夹中，然后在单人游戏中搜索"MCSR"。

![image](/image/ch1/25.png)

这张练习图包含了入门、练习和学习所需的大部分内容。最先需要掌握的是用床来杀死龙（单循环（以下简称"1c"））,基础下界传送门的搭建，猪堡路线——这些都会在指南中讲解。

### MiniPracticeKit

除了练习图，玩家还能在一个模拟完整速通流程的环境中进行训练，这也很有用。其中一些内容是在练习图中无法练习的，例如整场速通的后程分段（已收集完毕末影珍珠和烈焰棒的部分）。最广泛使用的工具是MiniPracticeKit（以下简称"MPK"），它是一个预设好的物品快捷栏配置，能让你高效地练习几乎任意一段你选择的速通流程。

[下载MPK](https://github.com/Knawk/mc-MiniPracticeKit/raw/master/hotbar.nbt)。添加进游戏前需要关闭游戏，然后去到你的游戏文件夹 (在Prism中右键点击您的游戏实例，选择 "打开文件夹"，然后打开 ".minecraft" 文件夹) ，并在这里把已下载好的文件放到这里。如果系统提示替换现有的快捷栏文件，请选择替换。文件应命名为 "hotbar" 或 "hotbar.nbt"，请勿更改成其他命名。

![image](/image/ch1/26.png)

重启游戏后，在创造模式下创建一个新世界。在控制界面中检查你的"加载快捷栏"快捷键（默认为X），并与你的"快捷栏1"快捷键一同按下，之后能看到如下图所示的快捷栏。如果未显示，请关闭游戏，并确保 hotbar.nbt 文件已按上图所示位置正确放置。请注意，按下"保存快捷栏"快捷键可能会被空快捷栏覆盖此配置，因此建议将其绑定至一个不易误触的按键。

![image](/image/ch1/27.png)

默认情况下有几个分段供你选择，例如"Nether Exit"分段，也就是后程。丢弃名为"Nether Exit"的木桶并放置在快捷栏9的命令方块，即可练习后程分段。之后，你将获得一些物品并被传送到远离出生点的位置。

若想自定义MPK，包括开局获得的物品和想要练习的分段，查阅 [MPK的GitHub界](https://github.com/Knawk/mc-MiniPracticeKit?tab=readme-ov-file#how-to-customize-mpk-behavior)

有另一种更简便的方式来编辑MPK，即[qMaxXen提供的这个网](https://qmaxxen.github.io/MiniPracticeKit-Editor/)。你可以通过网站界面直接编辑，然后下载新的 hotbar.nbt 文件并替换旧版本即可。

玩家在带着末影珍珠和烈焰棒离开下界后，首先会投掷末影之眼，并借助一个工具通过精确测量末影之眼的指向来定位要塞的确切位置，叫做 Ninjabrain Bot。

### Ninjabrain Bot

[下载Ninjabrain Bot](https://github.com/Ninjabrain1/Ninjabrain-Bot/releases/latest)。向下滚动页面，点击.jar文件链接进行下载。与ModCheck类似，Ninjabrain Bot是一个独立工具，而非游戏模组，因此请不要将其放入模组文件夹。下载完成后，双击运行即可。

使用Ninjabrain Bot最简单的方法是：投掷一颗末影之眼，看向末影之眼飞行的方向，然后按下 F3+C。接着，向任意方向旋转90度，跑动约30格距离，再次投掷并测量另一颗末影之眼。

![image](/image/ch1/28.png)

按下F3+C会把你当前的坐标与旋转角度复制到剪切板，Ninjabrain Bot会读取这些信息。之后，计算器会给出要塞位置的粗略估计——你可以在游戏内聊天栏里输入/locate stronghold来确认计算器的估计是否接近。需要注意的是，/locate stronghold告诉你的是要塞起始区块的中心（区块坐标 8,8）的坐标，而Ninjabrain Bot是告诉要塞起始楼梯的确切坐标（位于区块坐标 4,4）。此外，在使用Ninjabrain Bot定位要塞时，应参考 F3 菜单中的 "Block:" 信息，因为 "XYZ:" 信息在显示负数坐标时可能不准确。

Ninjabrain Bot 显示的百分比表示它对坐标准确性的可信度（上图中为 10.3%）。初次使用时，该工具默认对你测量末影之眼的精度为极低。虽然有一些方法可以提升测量精度，但在进行校准之前，Ninjabrain Bot会始终对你的测量结果保持低可信度。在进行校准前，我们先来提升测量末影之眼的精度。

投掷末影之眼后，暂停游戏并进入设置选项，将视场角（FOV）调至最低。然后，在控制设置中的鼠标设置，将鼠标灵敏度也调至最低。现在取消暂停，尝试将您的准星按如下方式定位：

![image](/image/ch1/29.png)

右侧准星应与末影之眼中心像素的左边缘对齐

为了更好地对齐准星，你可以使用暂停缓冲技巧：按住F3，然后反复按Esc来让游戏持续进入暂停状态。你可以在每次暂停之间不断移动鼠标，把准星慢慢对齐。

另一个确保测量准确的方法是修正不同步误差。操作很简单：完全静止站立一秒后，再投掷末影之眼。要了解为何这一步骤很重要，请[观看此视频](https://youtu.be/uBqAeZMlEFQ)。

最后，为了进一步提升测量精度，建议使用第二个工具来放大测量末影之眼。在 Windows 系统上，推荐使用Jingle工具。

### Jingle

[下载Jingle](https://github.com/DuncanRuns/Jingle/releases/latest)。点击 .jar 链接并运行下载的文件。和ModCheck and Ninjabrain Bot一样，Jingle是个工具, 而不是模组——不要把它保存在"save"文件夹中。

Mac用户可[下载SlackowWall](https://github.com/Slackow/SlackowWall)。 要完成此设置，请按照[此视频前2分25秒](https://youtu.be/Mj42HbnPUZ4)的步骤进行操作。

Linux用户在下列任选其一:

- [resetti (X11)](https://its-saanvi.github.io/linux-mcsr/minecraft/x11/resetti.html)
- 或者 [waywall (Wayland)](https://its-saanvi.github.io/linux-mcsr/minecraft/wayland/waywall.html)

打开Jingle后，进入"Hotkeys"标签页，点击右下角的"Add"，在弹出的下拉菜单中，选择"Resizing - Eye Measuring"，并设置一个快捷键来使用放大功能（最好设置为不易误触的按键）。

![image](/image/ch1/30.png)

接下来，切换到 "Scripts" 标签页，在 "Customize"选项旁点击"Resizing".。在弹出的窗口中，找到标有 "Enter your eye measuring size:" 的文本框，将其修改为 1920x3600（如图所示），然后点击OK。

![image](/image/ch1/31.png)

现在，当你将视场角（FOV）和鼠标灵敏度调至最低后，即可按下刚刚设置的快捷键来进一步放大观察末影之眼。请注意，Jingle必须保持开启状态才能生效。如果你不希望看到其窗口，可以在 "选项" 标签页中勾选 "最小化到系统托盘"，然后将Jingle最小化即可。

![image](/image/ch1/32.png)

此放大功能是通过调整MC游戏窗口尺寸实现的，窗口被拉伸为极高的竖屏状态。你还可以利用Jingle的窗口调整功能实现更多用途：

- "Thin BT" 将MC游戏窗口变得非常细长，适用于本指南"主世界"章节中介绍的无藏宝图定位宝藏策略。
- "Planar Abuse" 将MC游戏窗口变得非常扁平，在下界中使用时可以大幅度消除屏幕边缘的迷雾，极大提升能见度。

若要尝试这些功能，请返回 Jingle 的 "Hotkeys" 标签页并点击 "Add"。请注意，Mac 用户可使用 SlackowWall，Linux 用户也可使用 resetti/waywall。

此外，Jingle还包含许多其他实用功能，例如：清理旧世界以节省磁盘空间，以及启动游戏和其他自动辅助程序（如Ninjabrain Bot、录屏软件、AutoHotkey脚本等）。想了解更多功能详情，请访问[该网站](https://github.com/DuncanRuns/Jingle)。

了解末影之眼的测量流程后，接下来应对Ninjabrain Bot进行校准。请点击Ninjabrain Bot 上的齿轮⚙️图标，进入 "高级" 标签页，并选择 "校准标准偏差"。按照计算器给出的步骤完成校准，并多加练习后，计算器的预测可信度将会显著提升，并且可以在两次投掷末影之眼之间移动更短的距离来完成准确定位。

以下是为 Ninjabrain Bot 推荐的一些设置：

- 在 "基本" 中，将"数据显示"更改为 "详细"。
- 在 "高级" 中，启用 "显示角度偏差" 与 "用不同颜色显示负坐标"。
- 在 "快捷键" 中，为 "重置" 功能设置一个快捷键，按下该快捷键即可清空计算器中的所有测量数据。
  > 也可以直接点击计算器界面上的 "重置"、"撤销" 和 "重做" 按钮来管理测量记录。

![image](/image/ch1/33.png)

• 在"可选功能"中，打开"常规"里的所有功能。
更高阶的玩家会采用一种名为 "像素级精准"（也称 "船测"）的末影之眼测量方法。该方法结合了多种高阶技巧，能实现极其精确的测量，其精度之高使得仅需一次测量便足以确定要塞的精确位置。不过，这所能节省的时间相当有限——建议当你的通关时间接近或低于20分钟时再去使用。

像素级测量法设置指南:

- [Windows平台](https://youtu.be/l1Z2t9e6Qko)
- [macOS平台](https://youtu.be/Mj42HbnPUZ4)
- [Linux平台(X11)](https://its-saanvi.github.io/linux-mcsr/minecraft/x11/boat-eye.html)
- [Linux平台(Wayland)](https://its-saanvi.github.io/linux-mcsr/minecraft/wayland/boat-eye.html)

## 验证

如果你已经坚持到这里，那么恭喜————你已经在成为一名出色玩家的路上了。若你希望将通关记录提交至 speedrun.com，则需要提供完整的通关录像，并至少完整展示一次F3界面，同时在提交说明中附上世界种子（通关后可在游戏聊天框中输入 /seed 获取）。速通规则的摘要版本可在 [https://www.speedrun.com/mc?rules=game](https://www.speedrun.com/mc?rules=game) 查看，或直接在 [speedrun.com](https://www.speedrun.com/mc) 页面点击 "显示规则" 按钮。

![image](/image/ch1/34.png)

如果你的通过时间少于13分钟，你还需要在speedrun.com提交更多的证据才能通过验证，关于如何正确提交通关记录的更多信息，请观看[该视频](https://youtu.be/z2n2fCV1GY0)。

### 录制

想正确录制MC游戏画面，尤其是在Jingle调整窗口大小时，推荐使用 [OBS Studio](https://obsproject.com/)。请下载并安装该软件，完成基础设置。若你使用 Jingle，请进入其 "OBS" 标签页，其中列出了具体配置步骤：

![image](/image/ch1/35.png)

完成上述步骤后，你的OBS中会出现三个新场景。

![image](/image/ch1/36.png)

要录制游戏画面，请选择"Playing"场景，然后点击"开始录制"。其他场景的功能将在下方的"进一步设置 OBS"部分进行说明。

如果不使用Jingle，只需在OBS的"源"面板中点击"+"按钮，并选择"游戏采集"。当出现如下图所示的 "属性" 窗口时，将 "模式" 更改为 "采集特定窗口"，然后在"窗口"的下拉菜单中选择"Minecraft"。

![image](/image/ch1/37.png)

添加完游戏采集后，点击该来源并按 Ctrl+S 将其拉伸至铺满整个屏幕。

### 进一步设置 OBS

如果你此前已按照Jingle中 "OBS" 标签页的步骤完成设置，请注意，Jingle将自动在 "Playing" 和 "Walling" 场景之间切换。当你处于SeedQueue墙界面时，会自动切换到 Walling 场景，当你进入世界时，则会切换到 Playing 场景。如果你想添加其他源，例如摄像头和直播覆盖层（聊天框、通知提醒等），根据你想要它们显示的时机，将内容添加到对应的场景中（例如你可能只希望在进入世界时展示摄像头画面，而在墙界面时隐藏）。"Jingle Mag"场景用于像素级测量，无需理会。

在OBS中，点击右下角的 "设置"。以下是应确保设置正确的几项OBS设置：

- 在左侧的 "输出" 中:

  > 将 "输出模式" 更改为 "高级"。

- 在 "直播" 和 "录制" 内，均将 "视频编码器" 更改为可用的 H.264 选项（例如 "NVIDIA NVENC H.264"、"AMD HW H.264 (AVC)"、"QuickSync H.264" 等）。尤其是在录制MC时，不建议使用x264编码器。

- 在 "录制" 中，若想录制更好的画质，则将 "速率控制" 更改为"CQP"，若想有更好的性能表现，则更改为"CBR"。

  > 若选择 CQP，"CQ级别" 数值越低，画质越好，但文件体积也会相应增大。

  > 若选择 CBR，"比特率" 数值越高，画质越好，但文件体积会增大，并可能影响性能。

- 在左侧的 "视频" 中:

  > 确保 "基础（画布）分辨率" 设置为最高值，即与你的显示器分辨率保持一致。

为符合 speedrun.com 的验证要求，你的录像至少需要在某一时刻能够清晰完整地显示 F3 界面，且不应有明显卡顿或模糊。在开始冲击排行榜之前，请务必确认你的录像是清晰可辨的。

如果希望Ninjabrain Bot的画面也出现在OBS录制内容中，请进入Ninjabrain Bot的设置，进入 "OBS覆盖" 选项，勾选 "启用OBS覆盖" 及 "如果覆盖有一段时间没有更新，则隐藏覆盖"。然后，选中 "nb-overlay.png" 的文件路径并复制。

![image](/image/ch1/38.png)

接下来，在OBS中（若使用 Jingle，请在Playing场景下操作），点击 "源" 面板的"+"号按钮，选择 "图像"。在打开的窗口中，点击 "图像文件" 旁的 "浏览" 按钮，然后将之前从Ninjabrain Bot设置中复制的路径粘贴到 "文件名" 栏中。

![image](/image/ch1/39.png)

现在，当你测量末影之眼时，OBS将会把计算器的信息连同游戏画面录制下来。

## FAQ

1.  我的Minecraft游戏崩溃/闪退！怎么办？

    > 在Prism启动器中，右键点击您的游戏实例，选择 "编辑"，然后点击 "复制" 以复制日志内容。如果点击 "编辑" 后未看到如下图所示的日志界面，请重现一次崩溃情况，然后再次检查。

    > ![image](/image/ch1/40.png)

    > 点击 "复制" 后，请访问此网页：[http://maskers.xyz/log-analysis](http://maskers.xyz/log-analysis)。并将你的日志粘贴到文本框中，然后点击 "查找问题"。

    > ![image](/image/ch1/41.png)

    > 若网站给出的建议未能解决问题，请确保在复制日志前重现了崩溃现象。也可前往Java版MCSR Discord服务器里面的#public-help频道寻求帮助：[https://discord.com/invite/jmdFn3C](https://discord.com/invite/jmdFn3C)。提问时请附上日志及任何其他明显的错误信息或相关情况。

2.  我是笔记本玩家，在按照本指南设置后性能仍然不佳，怎么办？

    > 这可能是因为Java（以及 Minecraft）正在使用集成显卡。可尝试以下操作：
    >
    > - 在Prism启动器中，右键你的游戏实例，选择 "编辑"，然后进入 "设置" 页面。复制 "Java 路径" 字段中的完整路径。
    > - 按住 Win 键并按下 S 键，打开Windows搜索界面并搜索 "图形设置" 并打开该界面。界面应类似于下图：
    >   ![image](/image/ch1/42.png)
    > - 点击 "添加桌面应用" ，粘贴刚才从Prism复制的 "Java 路径" 字段中的路径。
    > - Windows图形设置列表中会出现一个名为 "javaw.exe" 的新应用。点击该条目，选择 "选项"，将其设置为 "高性能"，然后点击 "保存"。

3.  我没有购买正版Minecraft/使用未经认证的启动器，还能速通吗？

    > 你当然可以按自己的方式游玩，但有风险，并且speedrun.com不认可使用非本指南前述的启动器、或在非正版游戏的通关记录。此外，部分未经认证的启动器已知存在恶意行为（例如 TLauncher），因此强烈建议获取正版Minecraft。

4.  为什么ModCheck/Ninjabrain Bot/Jingle无法启动？

    > 请下载并运行 Jarfix：[https://johann.loefflmann.net/en/software/jarfix/](https://johann.loefflmann.net/en/software/jarfix/)。若仍无法解决，可尝试通过命令提示符运行该.jar文件，操作方法参见此视频：[https://youtu.be/MhwX8_ohOD8](https://youtu.be/MhwX8_ohOD8)。

5.  为什么OBS无法捕捉我的游戏画面？

    > 首先，请确保游戏窗口未处于最小化状态（可点击任务栏中的游戏图标将其前置）。同时检查你在游戏捕获属性中是否选择了正确的窗口。

    > 如果上述方法无效，请尝试参照上文 "我是笔记本玩家，在按照本指南设置后性能仍然不佳，怎么办？" 中的步骤进行操作

    > 如果问题仍未解决，请在OBS中进行以下操作:
    >
    > - 若使用Jingle：前往 "工具" → "脚本"，选择 "Regenerate With ‘Window Capture’"。
    > - 若未使用 Jingle：在"源"面板中点击"+"号并选择 "窗口采集"，然后在弹出的窗口中选择 Minecraft。

    > 请注意，窗口采集仅在Minecraft处于非全屏模式时有效，因此请确保已关闭全屏模式（同时检查StandardSettings中的相关设置！）。若使用Jingle，可尝试点击 "Go Borderless（无边框模式）"，这会让Minecraft看起来像全屏，但实际上仍处于窗口化状态，从而兼容窗口捕获。若此方法有效，可在Jingle的 "Option" 标签页中勾选 "Auto Borderless（自动无边框）"。

    > 若以上步骤仍无法解决问题，请右键点击窗口捕获来源（若使用 Jingle，该源将命名为 "Jingle MC Capture W"），选择 "属性"，然后将 "采集方式" 更改为 "Windows 10（1903或更新版本）"。

6.  为什么创建新的世界时游戏会自动切换全屏/窗口模式？

    > 请在StandardSettings设置中，点击 "全屏" 选项右侧的按钮，将其设置为OFF。

7.  为什么无法校准Ninjabrain Bot？

    > 请确保你已严格遵循了校准步骤。常见的错误包括：在开始校准时按住 F3+C 或误触其他按键——在被传送到钻石块上并获取末影之眼前（如视频指南所示），请勿触碰键盘或鼠标。此视频能帮助你更好地理解该过程：[https://youtu.be/Gp6EnDs24NI](https://youtu.be/Gp6EnDs24NI)。

    > Mac用户或使用Wayland的Linux用户可能在校准时遇到问题（若使用Wayland，切换至X11/Xwayland 通常可解决）。或者也可以在Ninjabrain Bot设置的 "高级" 标签页中，手动降低 "标准偏差（1.13+）" 的数值，并通过练习测量末影之眼来手动调整。建议从 0.01 开始尝试。

    > ![image](/image/ch1/43.png)

    > 标准偏差越低，代表Ninjabrain Bot对你的测量精度要求越高。如果工具提示您的测量结果不准确（如下图所示），请提高标准偏差并多加练习。

    > ![image](/image/ch1/44.png)
    > ![image](/image/ch1/45.png)

8.  为什么重启后Jingle没有保存我的快捷键/设置？

    > 请确保是以正常方式关闭Jingl（例如点击右上角的 X 按钮），而不是在电脑关机时仍让其处于开启状态。

9.  如何设置其他Minecraft版本或速通分类？

    > 请注意，本指南的其余部分主要围绕1.16.1任意进度随机种子无漏洞（1.16.1 Any% Random Seed Glitchless）这一分类展开。

    > 对于 1.14 及以上版本，你基本可以按照前述流程进行设置，只需在Prism启动器中创建实例和使用ModCheck时，将指南中提到的1.16.1和随机种子替换为你选择的分类和版本即可。

    > 对于 1.14 以下版本，请访问此页面：[https://github.com/Minecraft-Java-Edition-Speedrunning/legacy-fabric-instance-generator/releases/latest](https://github.com/Minecraft-Java-Edition-Speedrunning/legacy-fabric-instance-generator/releases/latest)。下载需要的版本，然后将下载的文件拖入Prism启动器以创建游戏实例，再按照前述方法使用ModCheck下载最新模组。

    > SeedQueue在大多数Minecraft版本中不可用，且StandardSettings等其他模组的功能也因版本而异。对于多数旧版本，替代方案是使用 Julti，可参照此视频进行设置：[https://youtu.be/\_8gQkgZcTKo](https://youtu.be/_8gQkgZcTKo)。

10. 为什么安装后，MCSR Practice Map练习图没有出现在我的世界列表中？

    > Windows系统可能在解压时损坏了地图文件。请下载并安装 7-Zip：[https://www.7-zip.org/](https://www.7-zip.org/)。然后，在右键点击 .zip 文件时选择以下选项：

    > ![image](/image/ch1/46.png)

    > 另外，请确保文件夹结构与下图所示一致：

    > ![image](/image/ch1/47.png)

11. 当SeedQueue reset时，我的电脑变得非常吵/发热严重！这是正常的吗？

    > 不用担心，这通常代表着SeedQueue正在充分利用CPU的全部性能。CPU制造商设定了安全的最高运行温度，并在过热时自动降低性能以避免硬件损坏。但如果仍旧不放心，可以检查电脑的散热情况，或在SeedQueue设置中适当调低 "种子加载上限数" 等相关选项。

12. 如何关闭视场角效果/下界传送门屏幕扭曲效果？

    > 请再次打开ModCheck，但在点击 "全选推荐项" 前，勾选左侧的 "辅助功能" 复选框，会安装 Extra Options模组，该模组移植了高版本中提供的无障碍功能选项。关于成绩验证的重要事项：如果使用 Extra Options 模组，请避免执行在未安装此模组时可能无法实现的操作，例如：
    >
    > - 在下界传送门中测量末影之眼
    > - 在穿戴着附魔灵魂疾行的靴子时站在灵魂沙上测量末影之眼
    >   若未遵守此规定，speedrun.com 将拒绝验证你提交的通关记录。

13. speedrun.com 允许使用哪些资源包？

    > 完整的A.4规则章节中列出了允许的资源包修改内容：[https://www.minecraftspeedrunning.com/public-resources/rules](https://www.minecraftspeedrunning.com/public-resources/rules)。稳妥起见，建议仅使用原版（vanilla）资源包。

14. 使用Jingle/ Ninjabrain Bot时遇到问题，怎么办？

    > 这得看情况，但许多常见问题可通过在整个系统范围内安装更新版本的 Java来解决，而非仅在Prism启动器中配置。请从此处下载并运行 .msi 安装文件：[https://adoptium.net/temurin/releases/?os=windows&arch=x64&package=jdk](https://adoptium.net/temurin/releases/?os=windows&arch=x64&package=jdk)。安装时请选择为所有用户安装。

15. 如何设置多人合作速通？

    > 请使用以下任一工具：
    >
    > - Bore: [https://www.youtube.com/watch?v=8NYvWOt42kg](https://www.youtube.com/watch?v=8NYvWOt42kg)
    > - the Jingle Easy Co-op plugin: [https://github.com/DuncanRuns/Jingle-Easy-Coop](https://github.com/DuncanRuns/Jingle-Easy-Coop)
    > - e4mcbiat: [https://github.com/DuncanRuns/e4mcbiat](https://github.com/DuncanRuns/e4mcbiat)

    > 请注意，后两种工具要求系统已安装较新版本的 Java——如需安装，请参照上一个问题的解答进行操作。

16. 当我设置像素级精准测量时，Ninjabrain Bot却给出了错误坐标，哪步错了？

    > 像素级精准测量的设置和操作流程非常精细（毕竟是像素级！），因此可能会忽略很多细节。最好前往 Java版MCSR Discord服务器的#public-help频道寻求帮助：[https://discord.com/invite/jmdFn3C](https://discord.com/invite/jmdFn3C)。

    > 常见问题包括：
    >
    > - Jingle的缩放分辨率错误：在 Jingle 中，进入"Scripts" ，点击"Resizing" 旁边的"Customize"，将末影之眼测量的分辨率改回默认的 384x16384。
    > - 测量值调整不当：请观看设置视频末尾部分的示例，学习如何辨认投影窗口并正确调整测量值。
    > - 使用Desmos计算器时，必须取"新灵敏度"值，并在以下列表的第一列中找到最接近的匹配值：[https://gist.github.com/ExeRSolver/cd8e89256a5f51ee4e32ba9df2db748f](https://gist.github.com/ExeRSolver/cd8e89256a5f51ee4e32ba9df2db748f)。例如，如果计算器给出的新灵敏度为 "0.1225"，则应在列表第一列中查找最接近 0.1225 的值：
    >   ![image](/image/ch1/48.png)
    >   然后，只需在standardsettings.json文件和Ninjabrain Bot中直接使用此灵敏度值即可。
    > - 确保Ninjabrain Bot和standardsettings.json中使用的鼠标灵敏度一致且无误。

17. 如何像其他玩家一样放大F3界面的特定部分？

    > 这通常是在OBS中实现的，可观看此视频教程：[https://youtu.be/ZXPM1f00wmY](https://youtu.be/ZXPM1f00wmY)。对于Linux（Wayland）用户，可使用 waywall 替代 OBS：[https://tesselslate.github.io/waywall/02_waywall_mirror.html](https://tesselslate.github.io/waywall/02_waywall_mirror.html)。

18. 使用快捷键缩放窗口时，如何给游戏画面设置自定义背景？

    > 这同样通常是在OBS中实现的——速通玩家本人未必能看到背景，但背景会出现在录制画面中。不过，如果打开OBS的投影窗口（例如像上一个问题解答中设置放大功能），就能看到在OBS中放置在游戏画面背后的所有内容。要添加背景，只需将图片/GIF/其他媒体文件拖入OBS。然后，在"源"面板中，将你的背景拖至"源"列表的最底部：

    > ![image](/image/ch1/49.png)

19. 如何以特定的F3饼图开始速通？

    > 在StandardSettings中，搜索 "Pie Directory（饼图目录）" 选项，此处应填写的值取决于你想要的饼图类型。常用目录包括：
    >
    > - 无藏宝图定位宝藏/定位传送门房间方向：root.gameRenderer.level.entities
    > - 下界要塞/村庄的饼图透视：root.tick.level.entities.blockEntities

    > 你可以在游戏内找到其他的饼图目录:

    > ![image](/image/ch1/50.png)

如果在这里没找到想要的答案，请在 [Java版 MCSR Discord 服务器的 #public-help 频道](https://discord.com/invite/jmdFn3C)寻求帮助。

## 鸣谢

本指南中提及的应用与成果，得益于以下Minecraft速通社区成员的贡献：

ModCheck：tildejustin & RedLime

SeedQueue和StandardSettings：KingContaria

SeedQueue计算器设置、日志分析及指南协助：maskers

MCSR Practice Map练习图: https://github.com/Dibedy/The-MCSR-Practice-Map?tab=readme-ov-file#credits

MiniPracticeKit：Knawkt

Ninjabrain Bot：Ninjabrain

Jingle/Julti：DuncanRuns

SlackowWall：Slackow

resetti和waywall：tesselslate

macO指南：neo_the_human

Linux指南：Saanvi

不同步误差讲解视频：Char

Windows平台像素级精准测量原始指南：osh

macOS 像素级精准测量指南：FlaxyB

speedrun.com提交视频：Ismexion/r0hkx

像素级测量指南、Bore设置视频及指南协助：montage

montage for the pixel perfect eye measuring guide, Bore setup video, and for helping with the guide

Ninjabrain Bot设置视频及指南协助：olock

本章节的内容由[shadowmeiyou@Bilibili(shadow啥都没有)](https://b23.tv/KrnS11M)翻译，在此特别感谢他的贡献！（编者注）
