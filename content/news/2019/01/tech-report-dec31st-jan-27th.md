---
author: "Vladimir Lebedev"
date: 2019-01-29
linktitle: Tech Report 20190129
title: "Tech report Dec,31st - Jan, 27th"
metaTitle: ""
metaDescription: ""
categories: [ "DEVELOPMENT" ]
tags: ["stegos", "report", "technology"]
weight: 20
draft: false
---

**Dec,31st - Jan,13th**, the Stegos development team has released the blockchain prototype (MVP). The MVP release containts the following base features:

- Nodes can select a group of validators among them
- Nodes can elect a leader of the consensus
- Nodes can verify incoming transactions
- The leader of consensus can create and propose blocks
- Validators can verify proposed blocks and co-sign them with their BLS signature
- The leader can form the final BLS multi-signature and broadcast sealed block to the network
- Nodes can verify and process incoming sealed blocks by pruning spent UTXOs out of the UTXO set

There is no disk persistance in the MVP release, as well as new nodes cannot connect and bootstrap from the living nodes. The screencast of MVP in action can be seen [here]( https://www.youtube.com/channel/UC0eunQJw-SMxqVYgkDMTCIA).

**Jan, 14th - Jan, 27th**, our developer started working on delivering the testnet-1 release. As a result of that sprint the following features have been added to the Stegos node:

 - Diffie-Hellman key exchange for ValueShuffle
 - DiceMix protocol for ValueShuffle (needs more thorough test coverage)
 - Transaction Pool Facilitator elections for ValueShuffle
 - Transaction Pool formation for ValueShuffle
 - Miscellaneous bug fixing for consensus & validator group formation protocols
 - Stake and Unstake transactions
 - Block rewards
 - Our networking layer, libp2p and floodsub, have been updated to the latest version of libp2p which introduced a lot of breaking changes
 - Unicast Messaging (simulated) has been re-introduced on top of new floodsub version
 - Gloab blockchain monetary balance validation

Plans for **Jan, 28th - Feb, 10th** are the following:

 - Research more deeply topics of fork resolution and slashing
 - Finalize DiceMix
 - Finalize ValueShuffle: super-trasaction formation and its broadcast
 - Generic skeleton for functional tests and functional tests for tx-processing, block processing and elections
 - Strawman on-disk persistency, full un-pruned blocks
 - Node bootstrap
 - Networking layer: Peer Store based on Kademlia DHT
 - Networking layer: Node Discovery protocol
 - Networking layer: Proper (not simulated) Unicast Messaging between nodes 
 - Networking layer: Tracking Peer State
