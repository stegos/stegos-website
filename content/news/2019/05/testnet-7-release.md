---
author: "Vladimir Lebedev"
date: 2019-05-30
linktitle: Testnet 7 Release 20190530
title: "Testnet 7 Release"
description: "This is the seventh Testnet release of the Stegos blockchain."
metaTitle: "test"
metaDescription: "test"
categories: [ "DEVELOPMENT" ]
tags: ["stegos", "report", "technology"]
weight: 7
draft: false
---

Stegos creates cutting-edge technology that keeps your secrets safe from prying eyes so you feel empowered and secure.

This is the seventh testnet release of the Stegos blockchain. Changes since Testnet 6:https://github.com/stegos/stegos/releases/tag/v0.6

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


Breaking changes:


TestNet-7 release is not compatible with TestNet-6. Please reset your local database if you upgrading from the previous release:

rm -rf database/
Check the project plan for additional information.


Please join us on Telegram to get test tokens and let us know your thoughts: https://t.me/stegos4privacy


Testnet node installation

Linux 64-bit:
curl -L https://github.com/stegos/stegos/releases/download/v0.7/stegos-linux-x64 -o stegos
chmod a+x stegos
./stegos

macOS 64-bit:
curl -L https://github.com/stegos/stegos/releases/download/v0.7/stegos-macos-x64 -o stegos
chmod a+x stegos
./stegos


Right after the start the node will print a lot of INFO messages with debugging information regarding bootstrapping your node. Press Enter to get stegos> prompt. To get help enter help command at the prompt.

