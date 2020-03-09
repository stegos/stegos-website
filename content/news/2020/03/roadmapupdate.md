---
author: "Sergey Timoshenko"
date: 2020-03-09
linktitle: Updated Roadmap 20200309
title: "Stegos Updated Roadmap"
description: "An updated roadmap for Stegos in 2020"
metaTitle: "Stegos Updated Roadmap"
metaDescription: "An updated roadmap for Stegos in 2020"
categories: [ "Development" ]
tags: ["stegos"]
weight: 7
draft: false
---

<img src="/images/Roadmap_Update.jpg" style="object-fit:cover;width:100%"/>

Things have been a little quiet here at Stegos this past month, but not because there hasn't been anything going on. In fact, quite the opposite: everyone is hunkered down developing some of our best and most private technology yet. If you want to follow our progress, you can always check out our GitHub.

Here's the updated roadmap of cool things we're developing in 2020 (and beyond), along with a brief explanation about why each milestone is so important. If you've got any questions or comments, be sure to head to our Telegram channel to let us know.

### Block Explorer v1

This is already up and running, and can be found here. It's a little different from other block explorers, because Stegos is so private, but you can check out the current block number, number of transactions per block and the current size of the validator service award jackpot, along with the past history of the awards.

### Mobile App Demo

The Stegos mobile app is currently undergoing internal testing and bug fixing ready for a wider demo rollout in the next few weeks.

We're calling this version a demo because it won't quite meet our self-imposed usability requirements: the app has a smaller storage footprint than the desktop app, but it achieves that by downloading the whole chain first and then deleting the parts it doesn't need. We'll change that in the next update, but for now this is only really suitable for use over WiFi.

We'll be looking for your help putting the app through its paces, so be on the lookout for a testing and feedback bounty very soon.

### Gossip Protocol

The Stegos network currently relies heavily on our bootstrap nodes, with all network traffic being routed through them. With the gossip protocol nodes will be able to communicate among themselves, making the network more secure and much faster. This will reduce our infrastructure load and massively improve syncing times.

### Block Explorer v2

Our current block explorer provides a lot of useful data about the Stegos chain and the validator service award, we've had a lot of requests to make it searchable. After the update, you'll be able to search for public payments. (Private payments will obviously always remain private — we couldn't provide data for them even if we wanted to!) 

### Full Mobile App

The first truly mobile version of the Stegos app. Once we update the app to only download the block headers and the transactions relevant to your account, you'll be able to use the app over data as well as WiFi, finally giving you privacy in your pocket at all times!

### Mobile App Optimizations

Even once the app is released, we won't be resting on our laurels. We've got a lot of plans to optimize the app and reduce resource consumption, to make sure you won't have to keep running to charge your battery.

### Private Chat

This is the big one: fully private one-to-one and group messaging, all secured by the Stegos blockchain. This has been pushed from the first release because the chat protocol requires some fundamental changes to the underlying blockchain, but once these changes have been implemented, you'll be able to send messages and transact with complete privacy, all from a single app: something no other crypto currency or messaging app can provide!

### Streamlined desktop node

Like the mobile wallet, the streamlined desktop node will just download the block headers and the data related to your own transactions. This will massively reduce storage requirements and syncing times for users where this is in an issue.

### Public IP addresses

With this update, full nodes will be required to use public IP addresses. This will further reduce the load on the Stegos nodes, which are currently handling all the traffic from IP-shielded nodes on our network.

### Flexible node discovery

Improving how node discovery works will remove the need for Stegos-controlled bootstrap nodes, making the Stegos network truly decentralized and ensuring that the Stegos chain will always live on even if the nodes controlled by the Stegos team are disrupted or otherwise taken offline.

### Red packets

Private red packets are our marketing ace in the hole: send tokens via chat to your friends and contacts, or use bigger packets for promotions and advertising. Red packets have an in-built delay while they interact with the chain: you'll be able to use this time to show messages, short videos or advertising.

### Two-key encryption scheme

It's currently impossible to build truly secure Stegos apps because you need to use your private key to scan the blockchain to search for incoming transactions. This introduces an extremely small but real security risk. Ideally, your private key should always remain in cold storage and never be connected directly to the internet. But many decentralized apps require a constant connection to work. It's a tricky problem.

By switching to a two-key encryption scheme, we can add a new kind of key which lets you scan the blockchain but not make any outgoing transactions. So this key can be used to power the apps, while the all important private key stays in cold storage.

This will allow all kinds of automated private apps without putting anyone tokens at risks. It will also allow us to minimize the use of public transactions, which are an inelegant solution in a privacy network.

### Privacy Marketplace

The Stegos privacy marketplace will replicate the features of the world's largest online marketplaces, like Taobao and Ebay, but completely privately. By scaling up the same technology used in our private transactions and messaging, we'll be able to offer large-scale e-commerce in complete privacy.

### Decentralized exchange (DEX)

Cryptocurrencies are ushering in a new era of privacy, but exchanges are an enormous weak point. You often have to undergo more KYC to register with an exchange than you would to set up a normal bank account! A decentralized exchanged will give people a truly private gateway to the world of crypto.

### iOS app

We've focused on Android so far because we can reach more users that way and it's easier to distribute Android apps than iOS ones (getting privacy apps onto the Apple Store is a nightmare!). But we know a lot of people use iOS, so we're committed to providing a version of the mobile app so everyone has access to mobile privacy, regardless of their device.

### Blockchain pruning

Blockchains are cumbersome beasts. The Stegos blockchain is still less than six months old and it's already growing quite large. This is a problem for our dream of fully mobile privacy, even with the streamlined nodes which only download block headers.

Luckily, we have a solution. By pruning spent UTXOs and expired messages, we'll be able to ensure the Stegos blockchain always stays at around 1-2 GB, no matter how long the chain gets. The encryption required to ensure this is done correctly, securely and privately, all without expending huge amounts of computational resources, is complicated and intricate.

The Stegos Team

Website: [https://www.stegos.com](https://www.stegos.com/)

Telegram: [https://t.me/stegos4privacy](https://t.me/stegos4privacy)

Wallet: [https://github.com/stegos/stegos-wallet/releases](https://github.com/stegos/stegos-wallet/releases)