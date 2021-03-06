---
author: "Sergey Timoshenko"
date: 2020-03-09
linktitle: 最新的路线图 20200309
title: "最新的路线图"
description: "一个2020年的最新路线图"
metaTitle: "最新的路线图"
metaDescription: "一个2020年的最新路线图"
categories: [ "Development" ]
tags: ["stegos"]
weight: 7
draft: false
---

<img src="/images/Roadmap_Update.jpg" style="object-fit:cover;width:100%"/>

在过去的一个月中，Stegos中的一切似乎都有些安静，但这并不是因为没有任何事情发生。实际上，情况恰恰相反：每个开发者都致力于开发我们迄今为止最好和最隐私的技术，如果您想了解我们的开发进展，可以随时查看我们的GitHub。

这是我们在2020年（及以后）要开发的很酷的东西的最新路线图，并简要说明了每个里程碑为何如此重要的原因。如果您有任何疑问或意见，请务必访问我们的Telegram群或微信群告知我们。

### 区块浏览器 v1

它已经启动并运行，可以在这里找到了，Stegos是如此私密，所以它与其他区块浏览器有点不同，但是您还是可以查看当前区块高度，每个区块的交易数量以及验证者服务奖的当前大小，以及历史奖励的记录。

### 移动app体验版

Stegos移动应用程序目前正在接受内部测试和错误修复，准备在接下来的几周内推出，以进行更广泛的测试。

我们将此版本称为体验版，是因为它无法完全达到我们自己的可用性要求：该应用程序占用的存储空间比台式机应用程序小，但它是通过首先下载整个链然后删除其不需要部分来实现的，我们将在下一次更新中对此进行更改升级，目前仅允许在WiFi环境下使用。

我们会一直在寻求您的帮助，以帮助推进该app的开发和测试，因此请留意即将到来的测试和反馈赏金活动。

### Gossip协议

Stegos网络当前严重依赖于我们的引导节点，所有网络流量都通过它们进行路由。使用Gossip协议，节点之间将能够进行通信，从而使网络更安全，更快。这将减少我们的基础架构负载，并大大缩短同步时间。

### 区块浏览器 v2

我们当前的区块浏览器提供了许多有关Stegos链和验证器服务奖励的有用数据，我们收到很多需求，希望其具备搜索功能。更新后，您将可以搜索公共付款。（显然，匿名付款将始终是匿名的-即使我们愿意也无法为他们提供数据！）

### 完整的移动app

Stegos移动应用程序真正的第一个版本。一旦我们更新了该应用程序，使其仅下载与您的帐户相关的区块头和交易，您就可以通过流量数据和WiFi使用该应用程序，从而最终在任何时候都为您提供隐私保护！

### 移动应用优化

即使发布了该移动应用程序，我们也不会在取得的里程碑旁休息。我们有很多计划来优化移动应用程序并减少资源消耗，以确保您无需在持续运行时对设备进行充电。

### 匿名聊天

这是最大的一环：完全私密的一对一和群聊，全部由Stegos区块链保护。这是从第一版开始推动的，因为聊天协议需要对基础区块链进行一些根本性更改，但是一旦实现了这些更改，您就可以通过单个应用程序进行完全隐私的消息通讯和交易： 独一无二，没有其他加密货币或消息传递应用程序可以提供！

### 简化的桌面节点

像移动钱包一样，简化的桌面节点将只下载区块头和与您自己的相关交易数据。这将大大减少存储需求并为出现问题的用户减少同步时间。

### 公共IP地址

通过此次更新，将要全节点使用公共IP地址。这将进一步减轻Stegos团队节点的负载，这些节点当前正在处理来自我们网络上隐藏IP节点的所有流量。

### 灵活的节点搜寻

改善节点搜寻的工作方式将消除对Stegos团队控制的引导节点的需求，从而使Stegos网络真正实现去中心化管理，即使Stegos团队控制的节点被破坏或以其他方式脱机，也可以确保Stegos链始终存在。

### 红包

隐私红包是我们的营销王牌：通过聊天向您的朋友和联系人发送代币，或者使用更大的包进行促销和广告。红包与链互动时会产生内置的延迟：您将可以利用这段时间显示消息，短片或广告。

### 双密钥加密方案

当前无法构建真正安全的Stegos应用程序，因为您需要使用私钥来扫描区块链以搜索传入的交易。 这带来了极小但真正的安全风险。理想情况下，您的私钥应始终保留在冷库中，并且永远不要直接连接到互联网。但是许多去中心化应用程序需要持续的联网才能正常工作。这是一个棘手的问题。

通过切换到双密钥加密方案，我们可以添加一种新型密钥，该密钥使您可以扫描区块链，但不进行任何外向交易。因此，此密钥可用于为应用程序服务，而所有重要的私钥均保留在冷存储中。

这将允许各种自动化的隐私应用程序，而不会给任何资产带来风险。它还将使我们能够最大程度地减少公共交易的使用，这是隐私网络中的一种不完善的解决方案。

### 隐私商城

Stegos隐私商城将复制世界最大的在线市场（如淘宝和Ebay）的功能，但完全是私密进行的。通过扩大隐私交易和消息传递中使用的相同技术，我们将能够在完全保密的情况下提供大规模电子商务。

### 去中心化交易所 (DEX)

加密货币正在进入一个新的隐私时代，但是交易所是一个巨大的弱点。与设置普通银行帐户相比，您通常需要经过更多的KYC才能在加密货币交易所进行注册！去中心化交易所将为人们提供通往加密世界的真正私密门户。

### iOS app

到目前为止，我们一直专注于安卓Android，因为我们可以通过这种方式吸引更多用户，并且相比iOS，Android应用更容易下载（将隐私应用发布到Apple Store是一场噩梦！）。但是我们知道很多人都在使用iOS，因此我们致力于提供一个版本的移动应用程序，以便每个人都可以访问移动隐私，无论使用什么设备。

### 区块修剪（Blockchain pruning）

区块链是繁琐的野兽。Stegos区块链还不到六个月的历史，已经变得相当庞大。这是通往我们梦寐以求的完全移动隐私的道路中所面临的问题，即使仅下载块头的精简节点也会面临这样的问题。

幸运的是，我们有一个解决方案。通过修剪用过的UTXO和过期的消息数据，我们将确保Stegos区块链始终保持在1-2 GB左右，无论链增长到多久。该加密技术需要在不消耗大量的计算资源的情况下，确保正确，安全和私密地完成区块修剪操作，因此该功能将非常复杂和富有挑战性。

Stegos团队

官网: [https://www.stegos.com](https://www.stegos.com/)

英文电报群: [https://t.me/stegos4privacy](https://t.me/stegos4privacy)

电报公告频道: [https://t.me/stegos4privacy_official](https://t.me/stegos4privacy_official)

钱包下载: [https://github.com/stegos/stegos-wallet/releases](https://github.com/stegos/stegos-wallet/releases)

节点下载: [https://github.com/stegos/stegos/releases](https://github.com/stegos/stegos/releases)

区块浏览器: [http://explorer.stegos.com/mainnet](http://explorer.stegos.com/mainnet)

开发者文档: [https://docs.stegos.com/](https://docs.stegos.com/)

微信公众号: stegos4privacy

English version: [https://stegos.com/news/2020/03/roadmapupdate/](https://stegos.com/news/2020/03/roadmapupdate/)