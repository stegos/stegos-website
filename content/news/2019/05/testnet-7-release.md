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

This is the sixth testnet release of the Stegos blockchain. Changes since [Testnet 5](https://github.com/stegos/stegos/releases/tag/v0.5):

- Added HashCash challenge to PubSub protocol to limit denial-of-service attacks
- Implemented simplified Re-Staking for tracking validators' online status
- Implemented wallet recovery using 24-word recovery phrase
- Implemented wallet password protection and encryption of keys stored on disk
- Split 1 STG to 1 000 000 microSTG.
- Limited the number of UTXO in transactions and blocks

**Breaking changes:**

TestNet-6 release is not compatible with TestNet-5. Please reset your local database if you upgrading from the previous release:

```
rm -rf database/
```

Check [the project plan](https://github.com/stegos/stegos/wiki/project-plan#sprint15) for additional information.

Please join us on [Telegram](https://t.me/stegos4privacy) to get test tokens and let us know your thoughts.

### Testnet node installation

#### Linux 64-bit:

```bash
curl -L https://github.com/stegos/stegos/releases/download/v0.6/stegos-linux-x64 -o stegos
chmod a+x stegos
./stegos
```

#### macOS 64-bit:

```bash
curl -L https://github.com/stegos/stegos/releases/download/v0.6/stegos-macos-x64 -o stegos
chmod a+x stegos
./stegos
```

Right after the start the node will print a lot of `INFO` messages with debugging information regarding bootstrapping your node. Press `Enter` to get `stegos>` prompt. To get help enter `help` command at the prompt. 
