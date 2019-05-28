---
author: "Vladimir Lebedev"
date: 2019-05-01
linktitle: Tech Report 20190501
title: "Tech Report Apr, 22nd - May, 3rd "
description: "Development team reports past sprint results and is announcing an upcoming first testnet release."
metaTitle: ""
metaDescription: ""
categories: [ "DEVELOPMENT" ]
tags: ["stegos", "report", "technology"]
weight: 8
draft: false
---

During the last two weeks our development team has been working hard to finalize major features of the upcoming testnet release.

Here is what we accomplished in the period **April, 22nd — May, 3rd**:

Done

 - Finalize HashCash integration, Network, required to prevent DoS-attacks
 - Stress Testing: Transactional Load Generator, Testing, the part of test harness
 - Determine major blockchain constants: Maximum UTXOs per Block, Epoch Length & Block Time, Consensus, those are important parameters of the consensus protocol
 - Wallet Recovery, Wallet, required to recover wallet keys using 24-word recovery phrase
 - Key Encryption on the Disk, Wallet, implement safe storage of keys on disk
 - Proof of UTXO Construction, Wallet, a feature allowing to prove that a particular transaction has taken place in the past


In progress

 - Slashing, Consensus, punishing the cheating slot owner for publishing two different blocks on the same height
 - Re-Staking, Consensus, changing validators’ PBC keys related to staked tokens at the predetermined intervals
 - Service Awards, Core Blockchain, required to create an incentive for validators to be online
 - Stress Testing: Multiple Regions, Network, launch nodes in multiple AWS regions to test consensus with real-life latencies
 - ValueShuffle: Bots, ValueShuffle, required to facilitate VS transactions in absence of enough VS transactions intents


Roman Tsisyk

 - Wallet Recovery is about recovery using 24-word recovery phrase. This feature has been implemented and can be used by Wallet UI.

