> * 原文地址：[UX Review and Redesign of the CocaCola Freestyle Kiosk Interface](https://medium.com/@vedantha/ux-review-and-redesign-of-the-cocacola-freestyle-kiosk-interface-f77fc087c09)
> * 原文作者：[Ved](https://medium.com/@vedantha)
> * 译文出自：[掘金翻译计划](https://github.com/xitu/gold-miner)
> * 译者：[ylq167](https://github.com/ylq167)
> * 校对者：[horizon13th](https://github.com/horizon13th) [yzgyyang](https://github.com/yzgyyang)

# 可口可乐自由风格售卖亭界面用户体验的回顾和重新设计 #

![](https://cdn-images-1.medium.com/max/800/1*ZydJMy1NI8CJ2Uwc0ocewA.jpeg)

一个可口可乐自由风格售卖亭的界面

### **任务** ###

- 理解这个售卖亭和它的用户体验
- 找到痛点以及用户体验的障碍
- 优化可口可乐自由风格售卖亭的用户体验和界面设计

### 设计流程 ###

![](https://cdn-images-1.medium.com/max/800/1*Jo9PS6PGeSzVPIJpSlnrLQ.png)

这是这个项目的设计流程

在重新设计中我遵循了简单的设计流程。

我自己之前从来没有用过这个机器，所以我需要理解它是如何工作的，以及它的使用环境。观察这个机器在不同的餐馆和电影院中如何被使用提供了重要的场景。

之后我做了一些快速用户测试，询问了当他们接饮料时在想什么。我把我的观察和用户访谈做了笔记，并分析数据以搞清楚他们的意义。这驱动了在这篇文章中提到的再设计。

### **观察** ###

我去了我所在区域附近有该机器的几家大众餐馆。主要目的是理解用户，环境和使用场景。通过和当地工作人员交流我也发现了（设备使用的）高峰时段。

**环境**

- 售卖机主要被放置在餐馆里，还有电影院等休闲场所。
- （这些场所）在周末，假期，以及工作日的特定时间会是高峰期。
- 高峰时经常会排队。

**终端用户**

机器的终端用户包括

- 年龄段：青少年及以上（够不着屏幕，不能操作屏幕的群体除外）
- 对热量和咖啡因有不同偏好的群体

### **快速的用户测试** ##

- 参与人数：4
- 熟悉程度：两人第一次用，两人曾经用过
- 时间：8、9 分钟左右

**来自用户测试的记录：**

- 曾经用过的用户明确的知道他们想要喝什么。他们快速的挑选类别，对图形界面很熟悉。
- 新用户花了很长时间做选择，他们在不同的几种主要饮料种类中纠结了一会儿。
- 新用户对屏幕底部的「Push」按钮也感到疑惑。
- 一些用户在装满杯子前想「尝试」新的味道或者是混合饮料。因此，他们也有许多反复的（操作）。

**一些用户建议**

> 「哇，太多选项了！」 

> 「我选的饮料通常在这儿」，用户指着饮料按钮说。

> 「我是否需要按住「Push」键？」

### 分析 ###

在界面和用户流等不同问题上，用户测试给了我一些很好的启发。为了理解更多，我们来探讨一下现有的用户流程。从用户站在售卖机前开始，到得到一杯饮料，过程如下图所示。

#### 当前用户流（仅适用于售卖机） ####

![](https://cdn-images-1.medium.com/max/800/1*zsd3Jch6qnl0JaerA700-g.png)

得到一杯饮料或者创造混合饮料的流程

这是一个最好的用户流程用例，适用于绝大多数的用户。虽然它一开始看起来相当简单，但是当用户没有想好要什么饮料时，这里最主要的障碍就是认知过载。 **每一屏上面都有 8 到 15 个选项可供选择。在这种情况下作出决策是相当困难的。而现有的设计并没有帮助（用户做出选择）。** 当用户需要创造一种混合饮料的时候花费的时间会更多。

#### 当前移动应用的用户流程 ####

![](https://cdn-images-1.medium.com/max/800/1*iOMdvGQAE33q_HYoXZZn1Q.png)

移动应用的用户流程

在售卖机上使用应用会稍稍简化流程，通过为用户准备好混合饮料节约了时间，所以他们不需要每次都浏览和选择。

#### 痛点 ####

从用户测试和[许多用户的在线反馈](https://www.facebook.com/IHateTheCocaColaFreestyleDrinkMachine/)来看，这些是我发现的痛点。

![](https://cdn-images-1.medium.com/max/800/1*rJ48-RHDEqtJJNfqK0kgSw.jpeg)

一个屏幕内展示 15 种饮料！

- 太多的选择中导致的认知过载（[根据西克定律](https://en.wikipedia.org/wiki/Hick%27s_law))
- 对于新用户和想要混合口味的用户来说，有太多反复的步骤
- 对于「push」按钮的初始认知不明确
- 屏幕超时的时间太短-造成了紧迫感
- 过滤器中可以不含咖啡因或者低热量，但不能同时过滤
- 获得一些常规口味的饮料像可乐和雪碧也需要太长时间。

### 重新设计 ###

根据前一阶段的发现，可以对用户体验进行细化，如下所示。辅助的移动应用也被考虑进行重新设计。首先让我们看看为了重新设计而定制的一些目标，约束和假设。

#### 重新设计的目标 ####

- 对于大多数人来说减少获得饮料所需要的步骤数
- 减少认知负荷
- 让创造混合（饮料）更简单
- 让导航更简单

#### **约束** ####
- 主要的约束就是触屏，它是电阻式触屏，适用于轻击的交互，而不太适合更高级的手势。

#### 假设 ####

- 售卖机可以给可口可乐（或者服务商）提供数据反馈
- 可口可乐和合作伙伴持续使用这些数据分析并优化产品。

#### 草图 ####

在快速产生创意上草图十分强大，我从做这些最初的草图中得到了最终的重新设计（方案），

![](https://cdn-images-1.medium.com/max/800/1*YUdZ1df6gR97Ntz1jHVs_w.jpeg)

探索一些初步的概念

![](https://cdn-images-1.medium.com/max/800/1*5Gab6nhVVNOHvP-kLBCY1Q.jpeg)

一些混合饮料的概念

#### 低保真原型 ####

这些初步的原型是用 Balsamiq 制成的。（他们源于大量的快速草图）

![](https://cdn-images-1.medium.com/max/1000/1*zBNUTKoV3u_vAM-i2ItgvA.png) 

左边：初始化界面 || 右边：用户选择一种饮料后的界面

思考下面的界面

左边：初始化界面由最受用户欢迎的饮料产品构成。请注意，「低热量」和「不含咖啡因」是过滤条件。用户可以选择两者，减少后续屏幕中的选项。

右边：用户选择了一种饮料后，系统「推荐」四种流行口味的饮料。请注意，这里有八种饮料可以选择。

这是更好的吗？那么，使用数据反馈的建议，设计 **可以更容易的从大约 100 个总数中选出 48 种最受欢迎的饮料。**

![](https://cdn-images-1.medium.com/max/1000/1*248PiUK1TkFRxuk2hvzQSw.png)

左边：在选择的饮料已经确定时 || 右边：用户接饮料时

上面的两个界面显示了接选中的饮料的流程。请注意，描述为「按住」，解决了用户早期对系统的混淆。作为改善微交互的一部分，它也相应了用户界面上的按钮。

另一个重要的事情需要注意-**这一行圆圈，这些是添加饮料到当前饮料中的建议。**用户可以快速按下这些选项之一，并将其添加到混合饮料中。再一次强调，**这些来源于数据的支持。**

![](https://cdn-images-1.medium.com/max/800/1*wje3sg8WTiqT0IGdXH6hXA.png)

在用户选择第二种饮料混合后

其他的关键点

- 设计使其易于导航。分页操作是一个容易的来回查找的设计，并且给出了可选择的全部选项的预期。

- 为了混合，用户还可以随时返回选择不用的饮料。这个设计试图简化此过程，但也使用户可以灵活的返回或重新开始。

#### 这如何改变用户流 ####

让我们考虑如何 **在数据驱动的支持下，针对大多数人，** 改变用户流。

![](https://cdn-images-1.medium.com/max/800/1*cyjjSL2T-qXC7uocWjDK8g.png)

重新设计的用户流

#### 移动应用如何进一步改善体验 ####

移动应用已经能创造更好的体验。但还可以进一步改善。让我们来看看我们如何在移动应用上选择饮料，以及如何改进。

![](https://cdn-images-1.medium.com/max/800/1*XG8SU63vMnjNmmsE1UAPzw.png)

左边：目前选择饮料的界面 || 右边：一个下拉搜索的设计

#### 高保真界面 ####

现在让我们看一看一些高保真设计，基于一些用户反馈，与低保真界面相比有一些小的变化。

![](https://cdn-images-1.medium.com/max/1000/1*dyJzBQnzaKCw1hFwONe-Nw.png)

左边：开始屏幕。该界面展示了第一页上最受欢迎的六种饮料。 || 右边：当用户点击一杯饮料后，变化如图所示。

开始画面上的一个变化是水图标被移到了右上角以获得更多的可见性，并且该按钮也用了圆形更符合饮料的图标形状。

![](https://cdn-images-1.medium.com/max/1000/1*tka8iXFvRQNEaDVwvYBz6g.png)

左边：一旦用户选择了一个饮料的变种，就把它倒入杯子里。||右边：当用户按下「Push」按钮时 UI 界面的反馈。

这些界面和低保真设计有一些不同。再最终版本中还有一个附加列-「混合饮料建议」旁边的「其他选择」。这更清楚的表达了用户（可以进行）的选择。如果用户想要选择与推荐的饮料不同的风味，这会引导他们进行下一步。

![](https://cdn-images-1.medium.com/max/1000/1*65IQM2cIqVpx421UaZtrjQ.png)

左边：用户点击推荐的第二杯饮料进行混合后，显示这个界面。|| 右边： 从开始的界面（界面 1），点击「水果味」进入此界面。

6 号屏幕显示「水果味」的选择。最受欢迎的五种口味显示在顶部并十分突出。下面显示不太受欢迎的口味。Kiosk 上有三种「混合」口味，这些都是混合口味。选择一个这些选项将显示类似于屏幕 2 的选项。

点击原型

[![](https://marvelapp-live.storage.googleapis.com/serve/2017/5/18854dfb4ab14e5ba0da5aa0eb69942a.png)](https://marvelapp.com/28f7gbe?emb=1&referrer=https%3A%2F%2Fmedium.com%2Fmedia%2F1dba6e6eec95ce7b8611343aef3c1237%3FpostId%3Df77fc087c09)

### 设计的局限性 ###

虽然重新设计解决了一些关键点，但仍存在一些不足。

- 当前设计将更受欢迎的选项优先于不常见的选项，如果用户想要不常见的选项，可能需要多做几步。

- 如果用户想要使用于推荐的口味不同的口味混合，需要重新开始活着回到口味选择页面，然后挑选另一种饮料。

**原型使用的工具：Balsamiq, Sketch**

**水果图标来自于 [*Freepik*](http://www.freepik.com)和 [*Madebyoliver*](http://www.flaticon.com/authors/madebyoliver)**

**如果您喜欢这篇文章，请点击原文里的小绿心。 它帮助别人发现这个帖子，并在我脸上放一个微笑：）。**

---

> [掘金翻译计划](https://github.com/xitu/gold-miner) 是一个翻译优质互联网技术文章的社区，文章来源为 [掘金](https://juejin.im) 上的英文分享文章。内容覆盖 [Android](https://github.com/xitu/gold-miner#android)、[iOS](https://github.com/xitu/gold-miner#ios)、[React](https://github.com/xitu/gold-miner#react)、[前端](https://github.com/xitu/gold-miner#前端)、[后端](https://github.com/xitu/gold-miner#后端)、[产品](https://github.com/xitu/gold-miner#产品)、[设计](https://github.com/xitu/gold-miner#设计) 等领域，想要查看更多优质译文请持续关注 [掘金翻译计划](https://github.com/xitu/gold-miner)。