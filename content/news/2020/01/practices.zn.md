---
author: "Sergey Timoshenko"
date: 2020-01-13
linktitle:  "保护个人资金安全的最佳做法 20200113"
title: "保护个人资金安全的最佳做法"
description: "手把手教你保护自身隐私和安全"
metaTitle: "保护个人资金安全的最佳做法"
metaDescription: "手把手教你保护自身隐私和安全"
categories: [ "DEVELOPMENT" ]
tags: ["stegos", "Practices", "Security"]
weight: 7
draft: false
---

## 隐私和安全是密不可分的，Stegos团队致力于确保您的Stegos节点和资金的安全性，尤其是在交易方面。 但是，与所有加密货币一样，最终保护安全的责任要落在用户自身，请阅读这些简单的提示，以帮助保护自己免受黑客和恶意行为者的侵害！

<img src="/images/practices_zn.png" style="object-fit:cover;width:100%"/>

我们的CEO Joel最近在Stegos Telegram官方群里评论了有关的安全措施，交易所以及Stegos团队如何将其转化为执行决策的方法，同时说明了用户可以采用的一些策略来保护他们的STG资产。（我们建议在[此处](https://t.me/stegos4privacy/47177)，[此处](https://t.me/stegos4privacy/47216)和[此处](https://t.me/stegos4privacy/47224)查看原始评论。）

### 交易所的漏洞

现在Stegos主网已经启动，并且每个人都有他们的STG币，那么可以理解，一些用户渴望我们获得交易所上市。实际上，寻找Stegos所在的交易所并不需要花费很多精力。

但是Stegos团队忌讳非正式交易所，却又总是在继续等待正式上交易所，为什么要坚持这样的立场呢？

Stegos不只是一个普通的区块链：它是一个真正的隐私区块链，致力于保护您的数据和元数据的安全，其中很大一部分是密钥管理。

如果您在社区中待一段时间，您会看到Joel重申将资金汇入未经批准的交易所的风险，这些交流所尚未与团队联系，我们知道他们都没有浏览我们最新的API文档的信息，因此他们无法得知与Stegos链进行安全可靠地集成的正确方法，他们将Stegos视为像其他加密资产那样对待，但事实并非如此！

至关重要的是，尚未与我们的开发人员合作以整合的非官方交易所无法正确地保护您的STG资金，更糟糕的是，无法判断他们是否使用了基本机制，例如离线签名和冷存储，如果没有，那么您的资金很容易被盗。

为了促进健康、安全的交易所集成，我们团队已编写了离线签名API以供交易所进行部署，这将在下一个节点版本中发布，同时，我们正在与知名的交易所直接合作，致力于在上交易所之前实施正确的安全措施，得到合作交易所合作伙伴的授意后，我们将宣布这家交易所，不幸的是，我们无法提前宣布交易所，因为我们冒着他们完全退出上币的风险。

在那之前，我们必须重申，我们**不建议**您将代币转移至未经认可的交易所，如果您的资金在未经认可的第三方交易所被盗或以其他方式丢失，则**Stegos团队不承担任何责任**。

然而，良好的安全措施不只是局限于交易所。

### 保护您的私钥

使用Stegos，您的私钥将用于签署发送STG交易，此外，您的私钥可用于扫描Stegos区块，以识别和核实从交易、区块奖励和VSA中转入的STG。

最好将您的STG保存在一个只有您自己持有私钥的地址上，此外，您的私钥不应保存在容易被无意或恶意的眼睛看到的地方，例如云服务器。相反，您应该将它们保存在通常不用于在线连接的单独设备上，例如冷设备或离线状态的笔记本电脑。

然而，我们是否也不建议人们在其节点上使用云服务器来最大化其稳定性和赢得VSA的机会呢？

节点操作员的关键点在于，您**不需要**私钥即可出块并验证网络，当然，节点必须保持联机才能运行，因此云服务器是一个很好的解决方案，但是，您应始终使**节点与私钥在不同的服务器上**运行，当您的节点连接到您持有私钥的同一服务器上的网络时，**黑客可以直接访问您的资金**。

我们将在本周发布本地和通过云服务器进行质押的指南，但是如果您觉得这太复杂了，请记住Stegos官方质押矿池是一种简单，安全，有保障且有益的选择！

### 密码管理

黑客针对用户的最常见攻击媒介是通过密码，无论是通过跟踪信息泄漏、记录键盘信息或强行攻击漏洞，都使您的密码都埋有重大的安全风险！

Stegos团队利用 [1Password](https://1password.com/) 更好地整合和保护公司密码，通过1Password，用户可以维护一个主密钥，该密钥可以解锁服务上托管的其他密码。我们建议个人同样使用1Password或替代密码管理服务作为另一种针对黑客的防御措施！如果您确实打算遵循我们的建议，建议您使用至少30个字符以及6-7个数字和符号的主密码。

我们还在所有团队帐户上使用双向认证（2FA），以提供第二级安全性，如果可以的话，我们建议您也这样做。

加入我们在Telegram或我们的论坛上，以更多地讨论隐私和安全性。

Stegos团队

官网: [https://www.stegos.com](https://www.stegos.com/)

论坛: [https://forum.stegos.com](https://forum.stegos.com/)

电报群: [https://t.me/stegos4privacy](https://t.me/stegos4privacy)

钱包: [https://github.com/stegos/stegos-wallet/releases](https://github.com/stegos/stegos-wallet/releases)

百科: [https://github.com/stegos/stegos/wiki/](https://github.com/stegos/stegos/wiki/)

本文于2010年1月12日[首发于Medium](https://medium.com/stegos4privacy/stegos-personal-security-best-practices-ca4a5e9e995)

