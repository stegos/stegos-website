---
author: "Vladimir Lebedev"
date: 2019-05-22
linktitle: Tech Report 20190501
title: "Tech Report May, 6th - May, 17th"
description: "Development team reports past sprint results and is announcing an upcoming first testnet release."
metaTitle: ""
metaDescription: ""
categories: [ "DEVELOPMENT" ]
tags: ["stegos", "report", "technology"]
weight: 7
draft: false
---

During the last two weeks our development team has been working hard to finalize major features of the upcoming testnet release.

Here is what we accomplished in the period **May, 6th — May, 17th**:


Done in Sprint 16


 - New StakeUTXO, Core Blockchain, StakeUTXOs with BLS signatures
 - Public payment UTXO, Core Blockchain, UTXO with uncloaked recipient pubkey and amount
 - Adding time locks to all UTXO types, Core Blockchain, allow UTXOs to be time-locked
 - Introducing micro and macro blocks, Core Blockchain, adding more security to microblocks
 - Slashing, Consensus, punishing the cheating slot owner for publishing two different blocks on the same height
 - Re-Staking, Consensus, changing validators’ PBC keys related to staked tokens at the predetermined intervals
 - Stabilize ValueShuffle facilitating in the event of epoch change, ValueShuffle, fine-tuning of the Facilitator code
 - Change PBC keys: network, Network, support for changing node’s pbc (validator) keys on the go
 - Check for stale connections, Network, check if some neighbor connections are stale and re-connect
 - Stress Testing: Deploy TxGenerator, Testing, transaction generator deployment support for devnets
 - Use AONT (All or Nothing) for all serialized representation of secrets, Security, additional security for in-memory representations of secrets
 - Implement WAU (Wipe After Use) for all secrets, Security, additional security for in-memory representations of secrets



Plans for Sprint 17


 - Speed-up node bootstrap and re-synchronization, Node, fine-tuning bootstrap constants
 - Service Awards, Core Blockchain, required to create an incentive for validators to be always online
 - Compress Micro Blocks to Macro Blocks, Consensus, remove last epoch’s micro blocks by moving their data to a single macro block
 - Optimize bulletproofs, Crypto, make bulletproofs verification faster than current 23 ms using parallelization (no processor-dependent optimizations yet)
 - HashCash: more bug-fixing, Network, bug fixing of HashCash protocol
 - Fork Resolution: more bug-fixing, Consensus, bug fixing of fork resolution mechanism for micro blocks
 - UTXO Timestamp Locking, Core Blockchain, implement locking of UTXOs
 - PublicPaymentUTXO: additional tx validation rules, Core Blockchain, implement additional transaction verification rules for transactions involving public payment UTXOs
 - PublicPaymentUTXO: support in wallet, Wallet, implement support for public payment UTXOs usage in wallet
 - Introduce variable fees in transactions, Core Blockchain, Wallet, introduce the ability to set arbitrary fee amount for transaction in order to increase chances of transaction to be included in the nearest block
 - DDoS Protection: blacklisting and rate-limiting, Network, implement rate-limiting and blacklisting as initial network-level DDoS protection mechanism
 - Change PBC keys: wallet, node, Node, support for changing node’s pbc (validator) keys on the go
 - Persist Payment History in Wallet, Wallet, required to support showing the payment history in wallet
 - Don't require wallet secret key for validator nodes, Security, reduce chances for an attacker to get hold of private wallet keys on hosted validator nodes by simply not requiring them to be present
 - LRU cache for unpacked UTXO, Node, node UTXO database optimization
 - Stress Testing: Packet Delay and Loss, Testing, part of test harness
 - Stress Testing: Large Number of Nodes, Testing, part of test harness
