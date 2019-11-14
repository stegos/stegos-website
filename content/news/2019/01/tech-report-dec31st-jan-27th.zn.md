---
author: "Vladimir Lebedev"
title: "Stegos技术周报（2018.12.31更新)"
date: 2019-02-13T17:06:33+06:00
linktitle: Tech Report Cn 20190129
description: "12月31日 - 1月13日，Stegos开发团队发布了区块链原型（MVP）。MVP版本包含以下基本功能： 节点可以在他们中选出验证器组； 节点可以选出共识的领导者； 节点可以验证传入的事务； 共识的领导者可以创建和提出块； 验证器可以验证提出的块并使用他们的BLS签名共同对块进行签名； 领导者可以形成最终的BLS多重签名和广播密封的块到网络； MVP版本中没有磁盘持久性，新节点也无法与活动节点连接和引导；"
metaTitle: ""
metaDescription: ""
categories: [ "DEVELOPMENT" ]
tags: ["stegos", "report", "technology", "chinese"]
weight: 30
draft: false
---

**12月31日 - 1月13日**，Stegos开发团队发布了区块链原型（MVP）。MVP版本包含以下基本功能：

- 节点可以在他们中选出验证器组；
- 节点可以选出共识的领导者；
- 节点可以验证传入的事务；
- 共识的领导者可以创建和提出块；
- 验证器可以验证提出的块并使用他们的BLS签名共同对块进行签名；
- 领导者可以形成最终的BLS多重签名和广播密封的块到网络；
- MVP版本中没有磁盘持久性，新节点也无法与活动节点连接和引导；


**1月14日 - 1月27日**，我们的开发人员开始工作于提交testnet-1版本。该冲刺我们取得了一些成功，Stegos节点添加了以下功能：

- ValueShuffle的Diffie-Hellman密钥交换；
- ValueShuffle的DiceMix协议（需要更全面的测试覆盖）；
- ValueShuffle的交易池Facilitator选举；
- 针对共识和验证者组形成协议的杂项错误修复；
- 赌注和赎回交易；
- 区块奖励；
- 我们的网络、libp2p和floodsub已经更新到最新版本，最新版的libp2p引入了
- 很多突破性改进；
- Unicast Messaging（模拟）已经在新的floodsub版本之上重新引入；
- 全球区块链货币余额验证；


**1月28日 – 2月10日**的计划如下：

- 研究更深入的分支和削减主题；
- 完成DiceMix；
- 完成Value Shuffle：超级交易形成及其广播；
- 用于功能测试、tx处理功能测试、块处理和选举的通用框架；
- Strawman磁盘持续性，完全未修剪的块；
- 节点引导程序；
- 网络层：基于Kademlia DHT的Peer Store；
- 网络层：Node Discovery协议；
- 网络层：节点之间的正确的（非模拟）单播消息传递；
- 网络层：跟踪Peer State；

    
请关注Stegos官方平台动态
