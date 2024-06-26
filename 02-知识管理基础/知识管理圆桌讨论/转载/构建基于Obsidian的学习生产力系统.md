---
uid: 20240326141152
title: 构建基于Obsidian的学习生产力系统
tags:
  - obsidian
  - 生产力
  - 转载
description: 基于 Obsidian 搭建一套自己的个人生产力创造系统
author: 大圣不是圣
type: other
draft: false
editable: false
modified: 20240326141445
---

# 构建基于 Obsidian 的学习生产力系统


> [!Warning] 转载声明
> 本文原链接为：[构建基于Obsidian的学习生产力系统 (微信)](https://mp.weixin.qq.com/s/raGkfhLujfArGRQtQB8Q5Q)
> 已征求作者同意，转载至Pkmer。


> [!NOTE] 引言
> 本文以 Obsidian 为基础，介绍了如何构建个人生产力系统。这个系统不仅仅是关于如何记笔记，更是关于如何将想法转化为行动，如何在信息中寻找灵感，以及如何持续产出有价值的内容。
> 



![](https://cdn.pkmer.cn/images/202403261414014.webp!pkmer)

> 我们塑造了工具，而后工具也在塑造我们。 
>
> \---- 麦克卢汉

尽管这篇文章完全是基于 `Obsidian` 这个工具来展开的，但严格意义上来讲，我并不希望它是一篇介绍 Obsidian 的文章，更多是基于 `Obsidian` 搭建一套自己的个人生产力创造系统，是基于个人使用的经验总结，也是逐步沉淀下来的一套实践方法论，因此有强烈的个人偏好，当然，我会尽可能把我遇到的问题，以及为什么要这么做告诉大家，希望对你也有所有启发！

## 一、背景

> 创造力不是靠灵感凭空而来的，而是一套完整的流程机制来产出的。

就像很多人经历的一样，前前后后，我也使用过非常多的「笔记类」工具软件，初衷其实很简单，**遇到想记的能够快速记下来，想用时能够快速找出来**。Evernote、Gitbook、语雀、Flomo、Apple Notes、Notability、Roam Research、Logseq、Notion、实体笔记本，不列不知道，一列吓一跳。

到目前，留下来在使用就下面四个：

- Obsidian[^1]，使用频率最高。使用比例 85% 左右。

- Notion[^2]，便于文档协作与分享，使用比例 5% 左右。

- Hepta[^3]，个人因为比较喜欢卡片排列与组合的方式，体验实践。

- Typora[^4]，用于一些长文档写作输出，纯工具使用。

- 自建的莱特纳盒子，实体笔记卡片，参考这里的介绍[^5]。使用比例 10% 左右。

> 这里的使用百分占比只是根据真实情况的一个估计，并非精确数字。

之所以一直在尝试，主要是没有建立一套适合自己，满足前面描述初衷的系统。不知大家有没发现，很多时候，我们记了很多内容，链接、金句、想法、摘录笔记，记了一堆，但却很少用到，记了不用，就纯粹是一个笔记存储了。

目前基于 `Obsidian` 这套系统的使用情况是：

1. **稳定产出**。使用两年左右，生产超过 2600 张卡片，平均下来稳定每天生产 3 ~ 5 张卡片。

2. **使用频率极高**，以前遇到一个问题，首先找搜索引擎，现在基本上都是先进入系统提取。

3. **灵感触发器**，很多有启发的想法都来自于这套系统，而非凭空产生。


真正实现了**想记的时候能够快速记下来，想用时能够快速找出来，偶尔还会引出一些新的灵感和启发**。

## 二、原则

实际上这套系统是自然生长而成的，在生长的过程中，记录下了一些自己**使用的原则及反常识点**，这也是我个人觉得最值得分享的。

### 1. 基于卡片的创作

在用 `Obsidian` 记录的过程中，逐渐养成了卡片记录与创作的习惯，卡片这个概念最初是源于卢曼（Niklas Luhmann）的卡片记录法[^6]。

![](https://cdn.pkmer.cn/images/202403261414015.webp!pkmer)

但真正对我启发很大的是来自于奥斯卡最佳原创剧本奖得主 Dustin Lance 介绍他的剧本创作流程的一个纪录片视频。

![](https://cdn.pkmer.cn/images/202403261414016.webp!pkmer)

Dustin 整个**剧本创作的核心流程是围绕卡片来进行的**，从搜集的材料中提取内容，转换为卡片；将一部电影的剧本长度转换为排满一张桌子的卡片，然后对整张桌子的卡片进行排列、删除与重组；对铺满整张桌子的卡片确认后，这时已经对要写的东西非常熟悉了，剩下就是将这些内容转化为剧本。

当时看到这个视频，非常惊讶，惊讶于卡片组合与创造的魅力，惊讶于文学创作原来不仅仅是靠灵感，更需要一套科学的流程。

![](https://cdn.pkmer.cn/images/202403261414017.webp!pkmer)

也强烈推荐大家看看这个视频： 奥斯卡编剧教你写剧本[^7] 。实际上，下面几条原则也是基于卡片这个基础来谈的。

### 2. 坚持原子化记录

原子化记录。**一张卡片就是一条想法，一个节点**，节点越原子化，你就越容易写入，节点与节点之点的排列与组合也就更容易促进创造。

刚开始卡片记录的时候，人们习惯性会将所有脑袋中的想法一股脑全写在一张卡片中，这样做带来的问题是，一张卡片实际上讲了多个点，在添加卡片之间的关联时就犯难了，**卡片之间的关联不容易明确，未来要用时，提取也就更难**。

`Obsidian` 中，尽管一条笔记就是一个 Markdown 文件，但在记录时，因为创建和管理的成本很低，脑袋里就只有卡片，完全忘记一个个具体的文件存在了。

### 3. 注重链接而非收集

**链接优于一切**，每张卡片就是一条想法，这条想法通过双向链接与其它节点关联，最终构成了整个知识网络，这个网络的质量则取决于这些相互链接的节点。

在实际使用中，这里的链接其实分为两类：

- 一类是**内部链接**。也就是你的知识网络中卡片与卡片之间的关联。

- 一类是**外部链接**。所有卡片尽可能标明外部来源，以便未来有需要时能够溯源，可能是一本书，一部电影，一次聊天。


我现在写卡片的时候，已经养成了这样的习惯顺序，**先写来源 → 再写关联 → 最后才写卡片主体内容**。充分利用 `Obsidian` 的模板功能，我们可以将卡片的基本结构创建好，这样更不会忘掉填写来源与关联了。

**节点之间的关联越多，呈现在你面前的机率也就越大，记忆与检索的难度也就越低。**

### 4. 注重数量而非质量

最初是在 David Perell 的一篇文章 《The Ultimate Guide to Writing Online》[^8] 中看到这个观点的，他写到

> Focus on quantity over quality at first. If you publish something every week for a year, you’ll gain tremendous insights into what you should be creating. 首先注重数量而不是质量。如果你连续一年每周发表一些东西，你会对你应该创造的东西获得巨大的洞察力。

这一点比较反常识，我们在记录与创作时，如果刚开始过于注重质量，往往很难进行下去，而且，对于一套基于卡片的系统来说，只有当卡片积累得足够多时，卡片之间更容易组合创造，才会慢慢从记录走向创作。

**卡片并非一成不变，随时可以迭代完善**。整套系统也是随着卡片的积累在不断进化的，我自己的经验是，当卡片积累超过 500 张时，知识网络的力量也就慢慢开始出现了，你准备写一张卡片，系统中快速搜索，很可能有与正准备写的卡片相关的内容已经记录了，立马添加上链接，或者直接更新之前的卡片，无论怎样，整个网络的质量都在不断提升。

优先注重数量而非质量，实际上也在提醒我们**需要转变一种思维方式**，数量是需要主动去积累的，而质量是在潜移默化中不断提升的。

下面是我较早写的一张卡片，可以看到，从内容本身上来，写得甚至不太通畅，但要表达意思是清楚的，毕竟卡片系统是私人使用而并非公开发布的，这样就够了。

最关键的是一张卡片只说一件事，来源与关联必须考虑到（从日期可以看到，有一张关联卡就是后面才加的）

![](https://cdn.pkmer.cn/images/202403261414018.webp!pkmer)

### 5. 强调卡片思维

把 `Obsidian` 当作一个卡片生成与创造工具，而不是一个简单的笔记管理与存储工具，这是一个基础前提。

当你把这些文档或文件抽象为卡片（Card）后，你思考更多是，**如何能生产更多的卡片，如何在卡片之间建立更多的链接，如何通过卡片的灵活组合来进行创造**！

- 配合内容地图（MOC） ，提供不同维度的卡片组合视角～

- 通过随机漫游和双向链接在不同卡片之间游走，激发创造

- 通过全局或局部视图来观察节点与整个知识网络的生长情况


下面这张讲从数据到智慧的图刚好能表达这种思维方式。

![](https://cdn.pkmer.cn/images/202403261414019.webp!pkmer)

___

大的原则聊差不多了，终于说到很多人可能更感兴趣的，也就是一些具体的操作实践，下面一一为大家呈现。

## 三、选择 `Obsidian` 的主要原因

兜兜转转，最终选择 `Obsidian`，最主要的原因就是：**快，并且刚好够用**。没想到这一点占了主要因素，但快确实很关键，快带来的好处是，**极大降低了使用负荷**，让整个使用的感觉非常流畅。

### 1. 打开快

`Obsidian` 并非一个网络应用，而是一个客户端程序，所有记录的文件都是以 markdown 文件本地（离线）存储的，这一点和 `Notion`、 `Road Research`、`Heptabase` 不同，后面这几个都是基于 Web 的，慢了不是一个等级。在 `Obsidian` 里打开文件几乎都是极速秒开。

> 之前对酷炫的 `Obsidian` 全局视图呈现感兴趣（对，就是文章开头那幅图），有在社区看到他们的开发团队谈到，最初是使用的 `D3` 库来创建的，但对渲染效率不满意，后来整个这一块全部用 WebGL 重写了，从这一点也看得出，他们对于整个软件的响应速度是很在意的。

### 2. 录入快

快捷键配合模板，创建卡片非常快，下面的录屏显示，借助模板，创建一张卡片的基本框架几秒钟就可以完成。

- `⌘ + N`，创建文件

- 使用 Alfred[^9] 的 Snippet 创建的快捷方式，输入当前日期

- `Shift + ⌘ +I` 快速打开预先准备卡片模板


![](https://cdn.pkmer.cn/images/202403261414020.gif!pkmer)

### 3. 检索快

在 `Obsidian` 中，模糊检索特别方便，比如说，我前面那张「笔记与网络」的卡片，我想找出来，只需要两步。

- `⌘ + O` ，快速打开文件

- 任意输入「笔记」或「网络」或「笔记网」，都能快速找到相应的卡片


![](https://cdn.pkmer.cn/images/202403261414021.gif!pkmer)

在 `Obsidian` 中，同样提供了基于文件内容和标签的全局检索，但我使用得并不多，90% 以上的场景直接通过上面的步骤都可以实现。当然，能做这一点，也源于我后面会讲到的一套好用的文件命名规范机制。

### 4. 同步快

`Obsidian` 中所有文件都是本地存储的，但为了多设备使用，需要文件同步，最初我是自己配置的基于 iCloud 的同步方案，但时常遇到同步不及时的情况，也折腾过一些其它方案，最后还是购买了官方提供的同步服务。

不得不说，官方的同步服务做得真好，多设备同步极度顺畅，几乎全是实时同步，有两次换手机，需要全部重新同步，也非常快，没遇到任何问题，如果需要多设备同步，个人还是非常强烈推荐官方的同步服务。

大家也可以评估一下自己现在使用的工具或流程方法，看是否能做到上面这几点，如果能做到，恭喜你，你也找到了适合自己的一套学习生产力系统。

### 5. 刚刚够用

这一点比较个人化，在使用 `Obsidian` 之前，用 `Notion` 更多，但 `Notion` 毕竟是一个基于 Web 的应用程序，打开和检索内容确实较慢，更适合比较长的文档及协作需求，`Notion` 独创的 Database 设计非常棒，但同时也带来一些问题，尤其是在通用性和迁移这一块，鱼和熊掌有时真不能兼得，根据自己的需求来选择吧。

过程中又尝试了 `Road Research` 和 `Logseq`，RR 也慢，而且挺贵的，`Logseq` 其实挺不错，不过默认基于大纲（Outline）的设计方式并不太喜欢。

大部分基于大纲设计的工具，特别适合块（Block）的双向链接，一行就是一个块级内容，但我自己的使用感受是，**块（Block）层级的链接粒度太细了，不太利于提取与创造**，因此尽管后来 `Obsidian` 也支持了块级双向链接，但我也基本没用，**卡片级的粒度对我来说刚刚够**。

> 这一点比较有个人倾向，因为我采用的是**以卡片为最小单位来进行知识管理与创造**，我也有看到别人基于块的方式在使用，用得也挺好的，所以这本身不是问题，关键你的策略是什么。

## 四、`Obsidian` 基础配置

在安装好 `Obsidian` 后，有一些基础配置，对日常使用会有一些有帮助。

### 1. 开启同步

我会用到移动端（主要是 Iphone 和 iPad），因此优先开启了同步，目前使用的是官方的付费同步服务。同步选项基本上是打开的，包括插件同步、图片、音频、视频等的同步。这一点 `Obsidian` 做得也很好，各种配置打开后，移动端的使用体验与桌面端几乎完全一致。到目前为止，整个仓库大小 700 M 左右（离上限 50G 还差得远）。

> 顺便说一句，`Obsidian` 的移动端也做得非常好，还曾获得了苹果每年的年度推荐工具称号。

### 2. 开启 Vim 键绑定

长期以来，自己比较习惯使用 `vim` 模式来编辑文字和代码了，`Obsidian` 默认也支持 `vim` 模式，通过 \`Editor > Vim key bindings），开启即可。

### 3. 选择适合的主题

一款适合的主题使用起来会比较舒心，这个看每个人的喜好，偶尔换一换也挺好的，我总共只使用过三款：

- `Obsidian` 官方默认的主题

- `Minimal` 一款极简的主题

- `Obsidian Nord`，目前使用的这一款主题，大概长下面这样（个人觉得中文显示效果更好看一些）


![](https://cdn.pkmer.cn/images/202403261414022.webp!pkmer)

### 4. 熟悉常用快捷键

快捷键可以极大提升使用效率，可以在 `Hotkeys` 里去查看或修改，除非特别需要，不建议修改默认的快捷键！

下面是一些我常用的快捷键。

- `⌘ + O`，快速打开文件，按文件名模糊搜寻

- `⌘ + P`，快速打开指令，比如说删除当前文件，移动当前文件

- `⎇ + Shift + R`，笔记漫游（random note）

- `⌘ + Shift + F`，可按文件内容进行全局搜索

- `⌘ + G`，打开全局关系视图，就是那个很炫酷的网状结点图

- `⎇ + Shift + G`，打开当前文件关联的局部关系视图

- `⎇ + Shift + F`，折叠起所有的标题栏

- `⎇ + Shift + U`，展开所有的标题栏

- `⌘ + ,` 打开参数设置窗口

- `⌘ + Shift + R`，打开（或关闭）右侧边栏（自定义的）

- `⌘ + Shift + L`，打开（或关闭）左侧边栏（自定义的）

> 说明：上面的快捷键是针对 macOS 的，如果使用 Windows，通常是将 `⌘` 键替换成 `win` 键，`⎇` 键换成 `alt` 键。

### 5. 其它配置

- 根据自己需要，在关于配置中开启英文或中文界面显示

- 在核心插件（Core plugins）页面，根据需求，选择启用一些配置选项


- 模板（Template）

- 漫游笔记（Random note）、

- 出链（Outgoing Links）

- 大纲（Outline）

- 字数统计（Word count）

- 白板（Canvas）


## 五、`Obsidian` 最佳实践

### 1. 少用插件

> 如无必要，勿增实体。
>
> \---- 奥卡姆剃刀定律

这一点我也是经过很长一段时间使用后的感受。以前也特别爱去折腾各种功能强大的插件，在 B 站或 Youtube 随便一搜，也是各种插件使用的教学视频，观看量还特别大。

不是说插件不好，尽量少用插件基于下面三点考虑：

1. 还是为了快，插件过多，必然会对软件的性能和稳定性有所影响

2. 既然记录的卡片原子化了，每张卡应该都比较简单，并不需要特别复杂的内容，大部分插件也就没必要了

3. 迁移，很多插件会对内容格式有一定影响，对于后续迁移会带来一些阻碍


看了下，目前正在使用的第三方插件只有下面三个：

- Local images plus[^10]，对于 Obsidian 的图片，希望都是本地离线存储的，使用该插件可以快速将在线的图片自换下载并替换为本地地址，非常方便。

- Advanced Slides[^11]，因为经常要做课堂使用的演示文档，有时打开 Keynote 去弄太麻烦，直接在 `Obsidian` 里写 Markdown 来自动生成 Slide，简洁高效，非常方便。

- Dataview[^12]，顾名思义，这个插件与数据呈现相关，你可以理解为 Obsidian 中的高级数据查询与可视化，类似 SQL，非常强大，后续会写点内容介绍一下结合自己的需求对该插件的用法。


使用这三个插件仅仅是因为刚好满足我的需求，也并未增加过多的复杂度。使用 `Dataview` 的一些页面在加载速度上还是会稍微有一些影响，所以也只会有有限、特定的页面中使用。不能破坏整体系统对「快」的要求这个关键需求。

> `Obsidian` 中很多功能强大的高质量插件，如 `Advanced Tables` 高级表格制作 、`Excalidraw` 手绘风格绘图、`Mind Map` 思维导图制作等，选择自己合适的就行，别老是在折腾这些插件，却没生产多少内容，得不偿失。

### 2. 文件命名规范

在个人知识管理实践中，文件的组织与管理一直是一个绕不开的话题，有太多讨论的文章和视频。

其实无论是文件夹组织还是文件命名，都是为了在使用时能够快速提取，就像我们传统在硬盘上存储文件一样，弄了一套非常完善的多层级文件夹，但要用时半天找不到，肯定就不是一种好的组织方式。

在 `Obsidian` ，全局快捷键 `⌘ + O` 打开检索栏，模糊检索功能非常好用，正是因为有了这一点，我现在已经完全摆脱文件夹组织的困扰了，甚至也很少使用标签（Tag）了，所有的重心都放在文件的命名上了，事实证明，这个方向是对的，**基于文件名的模糊检索方式，效率提高了不知多少倍**！

每个人的文件命名习惯都可能不太一样，建议大家多琢磨一下这一点，对于提升使用效率有极大的帮助。

我目前的文件命名由三部分构成，像下面这样：

![](https://cdn.pkmer.cn/images/202403261414023.webp!pkmer)

下面来具体看一些文件命名例子

**1. 普通卡片示例**

- `2022-02-22_card01_城市对冲`

- `2022-02-22_card02_任务卡片驱动学习`


**2. 人物卡片示例**

> 国外人物加上中英文也是为了便于检索

- `2021-10-13_people_Seymour Papert 西摩.派珀特`


**3. 书籍卡片示例**

- `2022-02-22_book_因计算机而强大`


**4. 周计划卡片示例**

- `2022-03-27_2022-04-02_W13`，代表 2022 第 13 周，从 3 月 27 号到 4 月 2 号


**5. 学习卡片示例**

- `2022-12-14_learning_algorithm`，代表算法学习


**6. 待办事项**

- `2023-10-20_todos`


**7. 内容地图 moc**

- `2022-02-02_moc_ai`，与 AI 主题相关的内容地图


可以看到，通过这样的文件命名方式，其实变向将原有的文件夹，甚至部分标签融入到文件名里去了，再配合卡片原子化的书写原则，带来的最大的好处是：**真正实现快速检索到需要的文件**。

> 注：关于文件命名规范，是我这套系统能够快速运转的关键，对于现有的工作和创造流程有很大的帮助，因此这部分迭代的比较勤，现在规范慢慢稳定了，最近会把 1.0 版公开出来。

实际上，一个好的生产力系统，输入只是一部分，更重要的是能够快速检索（提取），检索应该是非常频繁并且高效的，因此**系统中很多简化与设置都是为了最终实现高效检索和提取**。

### 3. 善用模板

模板使用频率还是比较高，对于常见的卡片类型，我都有创建对应的模板，最常见的就是卡片模板了，模板相对来说也比较偏个人化，下面是我目前使用的一些模板。

- card template：普通卡片模板

- book template：书籍模板

- note template：笔记模板

- weekly template：周模板

- people template：人物模板

- course template：课程模板

- teaching template：教学计划

- newsletter template：以前创建 newsletter 时建的模板


以普通卡片模板为例，内容其实非常简单，主要就是一些简单的替换符号使用：

![](https://cdn.pkmer.cn/images/202403261414024.webp!pkmer)

### 3. 内容地图 MOC

**内容地图（MOC，Map of Content 的简称）就是一张卡片（笔记），一种特殊的卡片类型。**，MOC 这个概念最初由 Nick Milo 提出 In what ways can we form useful relationships between notes?[^13]，感兴趣的可以去原文看看。

举个例子，我现在创建了很多与卡片使用相关的笔记，这时我可以创建一个与编程学习相关的内容地图（也就是一篇笔记），这篇笔记里把与学习相关的笔记直接引用关联进来。

需要注意的是，**使用 MOC 的真正意义并不是分类，而一种「面向主题」的设计**，它与目录也不同，内容地图是灵活的，是流动的，根据需要随时可以更改，而目录只是一个具体的，比较固定的，用线性形状来组织内容的一种结构。

MOC 使用很简单，但足够灵活，它为我们提供了看待卡片的不同视角。经常使用就会有这样的体会了。

下面的截图展示了我的一张主题为技术栈（techstack）的 MOC 卡片在全局视角下的关联 。

![](https://cdn.pkmer.cn/images/202403261414025.webp!pkmer)

### 4. 随机漫游

随机漫游，实际上是给我带来很大惊喜的一个小功能，其实就是随机帮你在所有卡中挑选一张显示出来，**随机带来的好处就是意外惊喜**，有些卡片如果不是主动搜寻，很少有机会打开，但随机就给了一个机会让它可能出现在你的面前，感觉这是强化整个知识网络的一个非常棒的功能。

无论是在 `Obsidian` 桌面端还是移动端，这个功能都很好用，使用没任何负担，我一般在坐地铁、休息或脑袋放空的时候就会刷一刷，经常会带来一些意想不到的灵感和启发。

比如说，我在手机上设置了通过**下拉来触发随机漫游**的动作，非常方便，下面是一个实际使用的演示图。

![](https://cdn.pkmer.cn/images/202403261414026.gif!pkmer)

这是被大部分人忽略掉的非常有价值的功能之一。

### 5. 文字替换快捷输入

另外，为了减少重复输入，我现在是使用 `Raycast` 中的 snippet 功能 创建了大量快捷输入语，方便文字和符号录入，下面是部分我常用的快捷输入

- 经常以 YYYY-MM-DD 格式动态输入当前日期，创建了 `;dt` 快捷方式，写卡片时第一反应就是这个

- 一些日常高频词，如输入 `;tel` 可以快速生成我的电话号码；如 `;id` 会生成我的身份证号码

- 一些不太方便直接输入的符号，如 `;ra` 会帮我输入向右的箭头符号 `→`， `;cmd` 会帮我输入苹果 command 符号 `⌘` ，`;star` 会帮我直接输入五角星符号 `★` ，等等


最好自己有一套自己的习惯方式，积累下来，会方便很多，也不仅仅只在 `Obsidian` 里使用，这种配置通常是全局的，任何地方都可以使用。

Mac 自带的文本替换功能也可以实现同样的功能；也可以使用功能更强大的一些专业文本替换类工具，如 aText[^14]、TextExpander[^15] 或 Typinator[^16] 等。

## 六、小结

如果你正在尝试使用某些工具构建自己的学习生产力系统，请反过来思考，我们构建这样系统的目的是什么，**一定是为了使用和创造，而不仅仅是存储，如果你记得很爽，从来没用，不一定是你懒，可能是这套系统流程有问题，不适合你**。

希望本篇文章对你有所启发。

参考资料

[^1]: Obsidian: https://obsidian.md/

[^2]: Notion: https://www.notion.so/

[^3]:Hepta: https://heptabase.com/

[^4]:Typora: <https://typora.io/

[^5]:这里的介绍: https://www.dailyup.blog/posts/spaced-repetition-practice

[^6]:卡片记录法: https://zettelkasten.de/introduction/

[^7]:奥斯卡编剧教你写剧本: https://www.bilibili.com/video/av9692264/

[^8]:《The Ultimate Guide to Writing Online》: https://perell.com/essay/the-ultimate-guide-to-writing-online/

[^9]:Alfred: https://alfred.app/

[^10]:Local images plus: https://github.com/Sergei-Korneev/obsidian-local-images-plus

[^11]:Advanced Slides: https://github.com/MSzturc/obsidian-advanced-slides

[^12]:Dataview: https://github.com/blacksmithgu/obsidian-dataview

[^13]:In what ways can we form useful relationships between notes?: https://medium.com/>@nickmilo22/in-what-ways-can-we-form-useful-relationships-between-notes-9b9ec46973c6_

[^14]:aText: https://www.trankynam.com/atext/

[^15]:TextExpander: https://textexpander.com/

[^16]:Typinator: https://www.ergonis.com/products/typinator/