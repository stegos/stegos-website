---
author: "Vladimir Lebedev"
date: 2019-06-05
linktitle: Tech Report 20190606
title: "Tech Report May, 20th - May, 31st"
description: "Progress report on the development team's most recent sprint, and plans for the next sprint."
metaTitle: "Tech Report May, 20th - May, 31st"
metaDescription: "Progress report on the development team's most recent sprint, and plans for the next sprint."
categories: [ "DEVELOPMENT" ]
tags: ["stegos", "report", "technology"]
weight: 8
draft: false
---

During the last two weeks our development team has been working hard to finalize major features of the upcoming testnet release.

Here is what we accomplished in the period **May, 20th — May, 31st**:


## Done in Sprint 17

- Speed-up node bootstrap and re-synchronization, `Node`, fine-tuning bootstrap constants

- Service Awards, `Core Blockchain`, required to create an incentive for validators to be always online

- Compress Micro Blocks to Macro Blocks, `Consensus`, remove last epoch’s micro blocks by moving their data to a single macro block

- Optimize bulletproofs, `Crypto`, a single bulletproof verification is now 10 ms (without AVX optimization)

- HashCash: more bug-fixing, `Network`, bug fixing of HashCash protocol

- Fork Resolution: more bug-fixing, `Consensus`, bug fixing of fork resolution mechanism for micro blocks

- UTXO Timestamp Locking, `Core Blockchain`, implement locking of UTXOs

- PublicPaymentUTXO: additional tx validation rules, `Core Blockchain`, implement additional transaction verification rules for transactions involving public payment UTXOs

- PublicPaymentUTXO: support in wallet, `Wallet`, implement support for public payment UTXOs usage in wallet


## Plans for Sprint 18

- Base functionality of GUI Wallet desktop application, `Wallet`, implementing bootstrapping visualisation, accounts and payments

- Improve security of Docker image, `Security`, strengthen the security of the node's docker image

- Introduce variable fees in transactions, `Core Blockchain, Wallet`, introduce the ability to set arbitrary fee amount for transaction in order to increase chances of transaction to be included in the nearest block

- Persist Payment History and Payment Certificates in Wallet, `Wallet`, required to support showing the payment history in wallet

- Use Base58 for external representation of wallet public keys (addresses), `Core Blockchain`, provide more user-friendly encoding of addresses

- Implement WebSocket API Authorization, `Security`, introduce API tokens for authorizing WebSockets API usage, even on localhost

- Support changing the wallet password, `Security`, provide the ability for the user to change wallet password

- Stress Testing: Packet Delay and Loss, `Testing`, part of test harness

- Stress Testing: Large Number of Nodes, `Testing`, part of test harness

- Stress Testing: Blockchain, Consensus, Service Awards, Slashing, ValueShuffle, `Testing`, stress testing the vital subsystems using transactional loads from transaction generator

- Introduce variable fees in transactions, `Core Blockchain, Wallet`, introduce the ability to set arbitrary fee amount for transaction in order to increase chances of transaction to be included in the nearest block
