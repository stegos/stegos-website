---
author: "Alan Li"
date: 2019-09-23
linktitle: 区块方舟AMA 20190923
title: "Stegos区块方舟AMA回顾"
description: "Stegos在区块方舟社区AMA的回顾"
metaTitle: "Stegos区块方舟AMA回顾"
metaDescription: "Stegos在区块方舟社区AMA的回顾"
categories: [ "INTERVIEW" ]
tags: ["stegos", "interview", "technology", "ama"]
weight: 7
draft: false
---

9月17日晚上7点，Stegos创始人Joel在社区进行了长达100分钟的AMA直播活动，并在9个社群同步转播，观看人数高达4500人，分享了Joel创立Stegos的曲折，讲解了Stegos技术干货以及现场答疑讨论十分精彩，一起来回顾昨晚的文字记录吧~
<br>

本次的嘉宾为Stegos创始人Joel，Joel是一位经验丰富的黑客和区块链先驱。他曾是AE的前首席技术官。也曾担任德意志银行大宗经纪技术总监，负责海外开发团队。目前他专注于Stegos，以解决隐私通信和付款问题。

主持人为BlockArk联合创始人大副，以下为直播实录：

<img src="/images/ama_2_zn.jpeg" style="object-fit:cover;width:75%"/>

## 直播实录

*区块方舟大副*:

Stegos是由AE的前任CTO-Joel创立<br>
Stegos主要特性：
- 隐私交易：完全的隐私，扩展性通过Omniledger分片+区块删减保证，首个支持分片的的轻量级区块链，所谓TPS根本不是什么问题，扩展性最强的隐私链。
- 隐私邮件：拒绝邮件监视。
- 隐私聊天：匿名版微信，链上隐私通信，与传统通信系统完全不同的架构。
- 隐私OTC：链上OTC赋予BTC匿名性，与OTC隐私聊天绝配。
- 赌注权益证明：1/3区块奖励注入赌注池，让pos不再拉大贫富差距，穷人也有机会一夜暴富。
- 移动挖矿：第一个支持移动设备运行全节点的区块链，真正允许每个用户运行节点，参与区块链治理。
我们的口号：**拒绝监控，拥抱自由！**


本次的AMA大概持续80-100分钟，分为两个环节。

第一个环节我将代表社区，讲最近两周社区的疑问提给Joel。

大概60-80分钟之后，会有自由提问环节，Ask Me Anything时间，在AMA总群和转播群的小伙伴都可以自由提问，由Joel为我们解答。

*区块方舟大副*:<br>
第一部分关于**目标愿景**，第一个问题：
JOEL创立Stegos的经历可谓十分曲折，AE、Emotiq、Stegos三个项目的构想和愿景都有很大的差别，是怎样的契机让JOEL最终选择了在Stegos这条路上走下去呢？相对于前两个项目，Stegos有哪些东西是最让人兴奋的？<br>
*Joel*:<br>
AE和Emotiq都是始于某种假定：有个很酷的东西叫做区块链，一旦产品建立好之后就可以找到很多有用的应用场景。但是对于Stegos，我发现了一个亟待解决的问题，然后建立了区块链。
现在设想下我们应该接受政府监控，因为我们无法对此采取任何行动。Stegos将把你从政府监控的束缚中解放出来，使你能够与任何人交谈，或向任何人进行绝对自由的付款，无论是你的付款和通讯都不可追溯！

*区块方舟大副*:<br>
Okay，第二个问题：
区块链技术在越来越多的国家和地区得到了认同，facebook也发布了libra的白皮书，在未来将更好地服务全世界的用户，这可能也会将移动支付带入一个新的阶段。对于Stegos来说，或许也迎来了一个非常好的机会，JOEL怎么看这一点呢？<br>
*Joel*: <br>
我们将来可能会推出一个基于算法的隐私型稳定币。我们现在完全专注于移动隐私付款。

*区块方舟大副*:<br>
好的, 第二部分的问题关于**解决方案**, 第三个问题：<br>
第三个问题：
作为首个支持移动app的POS隐私币，把手机作为区块链节点是很多项目都在尝试的事，但由于手机性能、网络波动等问题，至今没有一个成熟的解决方案或者出色的项目，Stegos要解决这个问题，有什么比较好的解决方案吗？<br>
*Joel*:<br>
在我们在全球拥有稳定的5G之前，仅仅由移动节点组成的区块链网络是不可行的。不过，值得提前做好准备。此外，请记住，许多智能手机花费他们的夜晚，甚至一天的部分时间，充电，闲置和连接到快速WiFi。我们的解决方案目前还不成熟，但我们正在取得进展！

*区块方舟大副*:<br>
第四个问题：<br>
Stegos提出用分片来解决区块链的速度，并且用修剪功能来减轻节点的数据负担，但是在一个匿名的隐私网络中，如何在分片及修剪后还能保证数据的可靠性？<br>
*Joel*:<br>
我们使用高级加密技术来确保隐私和匿名，同时确保我们的方法可靠。例如，我们实现了ValueShuffle，您可以将其视为内置比特币混币器。分片不会减少隐私，并且只要分片足够大就是安全的。此外，我们还有引导(bootstrap)节点，可以保留大部分区块链数据，以便新节点可以从头开始安全启动。我们正在致力于在将来淘汰这些引导节点。

*区块方舟大副*:
Okay，第五个问题：
Stegos提出了新的gPOS共识机制，能否为我们简单介绍下gPOS相比于传统的POS有何优势吗？在未来手机也成为验证节点后，对手机的性能或者网络（比如需要5g）是否有要求呢？<br>
*Joel*:<br>
使用传统的PoS，您获得区块奖励的机会与您的赌注大小成正比。如果您的邻居的赌注是您的10倍，那么随着时间的推移，您的赌注将减少10倍。因此，PoS是一个富人变得富裕但穷人保持贫困的体系。Stegos 的 Gamified PoS（gPoS）让任何人都有机会致富，无论他们的赌注大小如何。
每个块奖励的一部分会进入公共的奖励池，该奖励池会累积1-2周后，将奖励随机授予一个节点（验证器）。不过，gPoS不仅仅是一个简单的彩票，只有全天候在线并支持我们网络的节点才有资格获得奖励。这就是为什么我们称之为验证者服务奖！

*区块方舟大副*:<br>
在未来手机也成为验证节点后，对手机的性能或者网络（比如需要5g）是否有要求呢？<br>
*Joel*：<br>
只要手机连接到快速4G网络，它就应该可以工作。我们还没有分析运行节点可能导致的电池消耗。在晚上和工作工作期间，大多数智能手机花费大量时间用于连接WiFi和充电，这是将这些智能手机用于支持Stegos网络的最佳时间段。

*区块方舟大副*:<br>
第六个问题：<br>
在Stegos网络中，可以匿名交易和发送数据，但是为了保证匿名性，将没有身份信息会在网络上得以体现。在没有身份信息下，如何证明信息和数据真伪呢？比如有人冒充“我”与你交流，告诉你“我”换了个地址并希望你给他支付，该怎么证明他的身份？<br>
*Joel*:<br>
这既简单又困难。
我们仍然使用公钥/私钥加密。您可以与要与之聊天或付款的人交换公钥，一旦您这样做，您仍旧可以放心，您可以使用发件人的公钥验证邮件确实来自该发件人。使用您的私钥对邮件进行签名，并且能够使用您的公钥验证这些邮件，这可以保证安全性。
您的私钥证明了您的身份。我无法假装成为您，因为我无法得知您的私钥，也无法使用您的私钥签署邮件和付款。如果我在假装成您的同时使用我的私钥对邮件进行签名，那么您共享公钥的所有人都将无法解密和验证我的邮件。
请记住，公钥是公开的，因为它意味着要共享！您可以使用公钥创建QR码，并将其贴在墙壁和人行道上。对您或其他任何人都不会有任何伤害。但是，拥有公钥的任何人都可以对来自您的邮件进行身份验证，因为只有您的公钥才能解密您使用私钥签名的邮件！

*区块方舟大副*:<br>
第七个问题：<br>
从白皮书和stegos的发展路线中，看得出来JOEL很喜欢微信发红包的功能，并且将这个功能加入了stegos的匿名网络中。但是我们注意到，如果发送的红包没有人领取，这个红包将会进入到奖金池中而无法退回，这样设计的目的是什么呢？<br>
*Joel*:<br>
将无人认领的红包归还给验证者服务奖池（又名奖池）只是一种权宜之计，可以避免让STG币陷入永久锁仓的困境并让他们回归流通状态。我们预计无人认领的红包会非常罕见。

*区块方舟大副*:<br>
第八个问题：<br>
我们之前很多的竞争品对比分析都着重在隐私币这一方面，大家也更加关心支付的匿名性。但是对于stegos来说，点对点加密的消息传递也是一个重大的功能，这项功能相对于市场上其他类似的项目，比如telegram，有什么优劣势呢？<br>
*Joel*:<br>
这个问题我们需要花一点时间来回答...不过我会尽量长话短说。
默认情况下，电报不是端到端加密的。在Telegram上发送的任何消息仅从发送方加密到服务器，然后从服务器加密到接收方。这意味着任何人都可以利用其服务器上的Telegram消息，无论是电报本身，政府还是黑客。电报也使得设置端到端加密的聊天非常不方便。您需要明确创建此类聊天，并且它们仅保留在您启动它们的设备上。这是一个非常糟糕的设计，但也许它是故意这样做的。
其他信使软件确实具有端对端（点对点）加密功能，例如，iMessage，WhatsApp或Viber。请注意，这些信使软件与您的电话号码相关联。这意味着任何拥有足够权力的人都可以观察您的沟通方式并从中获得结论，特别是如果他们可以访问您的互联网浏览历史记录和其他通信记录。
Stegos是完全加密和匿名的，不需要邮箱地址或电话号码。Stegos不泄漏元数据，例如您的电话号码，聊天时间和持续时间。与Stegos一起发送的消息只与公钥相关联，无法追溯到您。邮件无法解密和读取，付款也是如此。
我应该提醒下微信没有任何加密。

*区块方舟大副*:<br>
第三部分关于**市场发展**, 第九个问题:<br>
STG代币在网络中有哪些作用？支付是否需要支付STG？发送信息是否需要支付STG？换句话说，STG的代币升值逻辑是什么？<br>
*Joel*:<br>
STG主网币用于支付Stegos区块链上的所有事务，包括付款和消息。从理论上讲，对Stegos主网币的需求越多，它们就越发升值。我们将努力确保Stegos移动应用程序的广泛采用，并使应用程序本身尽可能诱人。出于法律原因，我无法进一步谈论代币定价或升值。

*区块方舟大副*:<br>
第十个问题：<br>
纵观整个团队，我们对David mcclain很感兴趣，作为首席火箭科学家，在团队中扮演的是什么角色呢？在太空搭建stegos节点吗？两年前一个名字叫太空链的项目似乎有同样的构想但是最终失败了。<br>
*Joel*:<br>
David是我们团队的重要开发人员，同时他也是一位密码学大师级人物。他在Stegos区块链上运用了他包括太空行业在内的各个行业多年来积累的知识。

*区块方舟大副*:<br>
第十一个问题：<br>
Stegos进行过很多轮的融资，之前进行过一轮种子轮融资和两轮私募，总募资额达1585万美元，之后团队还会进行两轮私募以及可能的IEO，而且在主网上线后12个月团队的代币也将解锁，团队会进行售卖以满足资金需求。对于一个目前11个人的团队来说，为何需要如此大的资金体量？1585万美金的融资至今已经使用了多少了？未来还会使用多久？在新的一轮融资后团队会拓展到什么规模？<br>
*Joel*:<br>
哦，这真的是一个比较难回答的问题...
Stegos将进行IEO，但不计划进一步的私人配售轮次。请注意，IEO不会为团队筹集资金，因为筹集的资金将用于提供流动性。通常，团队还需要添加自有的资金，匹配或超过IEO金额，也用于流动性和做市。
由于我自己的经验不足，我已经让所筹集的加密货币资金从1585万美元缩减到这个数额的一小部分。我本应该立即卖掉加密货币但没有这么做。请留意，我们在ETH在800美元至1000美元时筹集资金，现在仅为180美元至190美元。
我们有高达200万美元的现金和加密货币，并且已经在小心地花这笔钱。但这不会持续很长时间，因此我们需要通过在IEO一年后出售我们的一些代币持有来为运营提供资金。我们只根据我们的开发计划和现金流进行团队扩展。

*区块方舟大副*:<br>
最后一个问题:<br>
Stegos的未来市场发展规划是什么样的？经历了一个牛熊过后，JOEL对未来的市场环境做一个预测吧，区块链将给我们的生活带来什么样的改变？持有STG代币的人会如何获得成功？<br>
*Joel*：<br>
出于法律原因，我不允许进行任何市场或价格预测。我真诚地希望通过使用Stegos，您将在广泛的政府监督下获得自由，并能够在和平与安全的环境中开展业务。
拒绝监控 — 拥抱自由！

*区块方舟大副*:<br>
非常感谢Joel的分享，现在我们进入到自由提问环节吧~

*区块方舟大副*:<br>
第一个自由问题来这AMA总群林炳辉：
"我想问：一些交易所正在取消隐私代币以进行监管，这对流动性会不会有很大的影响呢？"
还有一个就是，你为什么要使用全节点钱包？它不是很友好使用。


*Joel*:<br>
迄今为止，很少有交易所下架隐私硬币。日本宣布隐私币为非法，现在在韩国有一家交易所也这么做了。对于这些决定放弃机会的交易所，其他交易所就会涌现出来或者取代他们原有的位置。
我们正在开发自己的P2P交易功能。因此，只要购买STG硬币，就不会失去隐私。例如，您将能够可靠地将BTC替换为STG和替换回BTC。我们将扩展我们的钱包应用程序与这一交易功能，包括场外聊天室，交易订单以及完全隐私匿名的交易！
至于全节点钱包，这只是一个快速的方法，以便上线主网做好准备。我们目前已经在开发Stegos移动App了。
其他问题？

*区块方舟大副*:<br>
第二个自由问题来这AMA总群林檎：
"Hello，joel，你好，我想问的问题是，做匿名支付的货币很多，例如Zcash、门罗，你认为Stegos跟其他竞品对比的优势在哪里？"
*Joel*:
Stegos是第一个也是唯一的支持移动PoS的隐私硬币。所有其他硬币都是Pow，需要消耗大量的电力才能发挥作用，这样它们就不能在口袋里的智能手机上运行。

*区块方舟大副*:<br>
第三个问题来自总群流星雨：
"我认为，beam这种，挖出来的矿币团队抽成，模式不错，joel觉得呢?"
<br>
*Joel*:<br>
Beam从投资者那里筹集资金，据我所知他们得到了很多投资。我很确定他们可以靠这笔资金工作多年而无需对社区征税。我们的团队比Beam的团队规模小得多，我认为当你从私人投资者那里筹集资金后，再征收开发税对社区不公平。

*区块方舟大副*:<br>
第四个问题来自总群郑格：
"hi，joel，过去的IEO项目很多都是牺牲了私募投资者的利益，给IEO更好的价格跟流动性，Stegos怎么看待这种做法，你们怎么平衡私募与IEO投资者的利益冲突的呢？"<br>
*Joel*:<br>
平衡IEO和私募投资者的利益是不可能的。投资者被IEO吸引的原因是他们比私募投资者有优势！不过，我们确实试图减轻私募投资者的痛苦。我们缩小了IEO和私募投资者之间的价差，还给了私募投资者2倍的币。

*区块方舟大副*:<br>
中间总群林炳辉穿插一句提问：
"隐私权保护的问题最近已经引起人们的关注，你是怎么想的呢？"<br>
*Joel*:<br>
我想强调的是，如果你心甘情愿地将隐私信息送人，我们将无法保护你的隐私。例如使用社交网络和其他的应用程序，比如面部识别软件。我们能做的就是保护你不受监视。<br>

*区块方舟大副*:<br>
由于时间关系，我们的AMA到此告一段落拉，感谢Joel的分享，祝Stegos越来越好！

本篇文章同步发布于以下主流媒体：

金色财经：https://www.jinse.com/blockchain/470279.html<br>
链向财经：https://www.chainfor.com/news/show/89244.html<br>
币看：https://bitkan.com/zh/ksite/articles/68621<br>
火星财经：https://news.huoxing24.com/20190918193628983582.html<br>
链节点：https://www.chainnode.com/post/377188<br>
