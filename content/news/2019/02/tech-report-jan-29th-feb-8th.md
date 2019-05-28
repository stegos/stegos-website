---
author: "Vladimir Lebedev"
date: 2019-02-12
linktitle: Tech Report 20190212
title: "Tech report Jan, 29th - Feb, 8th"
description: "Development team reports past sprint results and is announcing an upcoming first testnet release."
metaTitle: ""
metaDescription: ""
categories: [ "DEVELOPMENT" ]
tags: ["stegos", "report", "technology"]
weight: 10
draft: false
---

During the last two weeks our development team has been working hard to finalize major features of the upcoming testnet release.

The following tasks were completed in the period **January, 29th — February, 8th**:

 - Core: **Blockchain persistency**. Blocks are stored on disk now but no transaction pruning is applied.
 - Core: **Node bootstrap**. A new node can connect to any Stegos nodes to download the blockchain.
 - Core: The special Data UTXO type has been removed and data functionality has been rolled into the payment UTXO.
 - ValueShuffle: **DiceMix**
 - ValueShuffle: **Composing the super-transaction**. More unit tests are needed. 
 - Networking: **Global Network Peer Store**. Based on Kademlia DHT.
 - Networking: **Node Discovery**. Including node authentication.
 - Networking: Unicast Messaging.

Our next sprint will be dedicated to thorough testing, bug fixing and launching the very first Stegos **testnet**!

Tasks for **February, 11th — February, 22th**:

 - Testing: Meticulous testing and bug fixing applied to transaction processing, block processing, initial randomness (VRFs), consensus, persistence and bootstrapping.
 - Core: Node CLI enhancements.
 - Core: Orphan transactions processing.
 - Core: Limiting the maximum size of a block.
 - ValueShuffle: **First working implementation**
 - DevOps: Collecting and processing metrics and logs (Logstash, Prometheus, Grafana, ElasticSearch, Filebeat, Kibana, etc).
 - DevOps: **TestNet deployment on AWS**.
 
We are planning to freeze new features early in the second week of the Sprint 10 to release the testnet binaries and launch the tesnet by Thursday, February 21st. 
