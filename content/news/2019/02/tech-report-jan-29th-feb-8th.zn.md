---
title: "Stegos技术周报（01.29 - 02.08）"
linktitle: Cn Tech Report 20190212
description: "在过去两周内，我们的开发团队一直在努力完成即将推出的testnet版本的主要功能。"
date: 2019-02-18T14:03:09+06:00
metaTitle: ""
metaDescription: ""
categories: [ "DEVELOPMENT" ]
tags: ["stegos", "report", "technology", "chinese"]
weight: 10
draft: false
---

在过去两周内，我们的开发团队一直在努力完成即将推出的testnet版本的主要功能。

**1月29日 - 2月8日完成了以下任务：**

- Core：区块链持续性。块现在存储在磁盘上，但未应用任何事务修剪；
- Core：节点引导程序。新节点可以连接到任何Stegos节点以下载区块链；
- Core：已删除特殊的数据UTXO类型，并且数据功能已滚入支付UTXO。ValueShuffle：DiceMix；
- ValueShuffle：组成超级交易。需要更多的单元测试；
- Networking：全球网络同行商店。基于Kademlia DHT；
- Networking：节点搜寻。包括节点认证；
- Networking：单播消息传递；
 
我们的下一个冲刺周期（sprint）将致力于彻底的测试，错误修复和启动第一个Stegos testnet！
 
**2月11日 - 2月22日的任务：**

测试：应用于事务处理，块处理，初始随机性（VRF），共识，持久性和引导的细致测试和错误修复。

- Core：节点CLI增强功能；
- Core：孤儿交易处理；
- Core：限制块的最大大小；
- ValueShuffle：第一个工作实施DevOps；
- 收集和处理指标和日志（Logstash，Prometheus，Grafana，ElasticSearch，Filebeat，Kibana等）；
- DevOps：AWS上的TestNet部署；
 
我们计划在冲刺周期10（Sprint 10）的第二周早些时候冻结新功能，以便在2月21日星期四之前发布testnet二进制文件并启动testnet。
