---
author: "Sergey Timoshenko"
date: 2020-01-13
linktitle:  "Personal Security: Best Practices 20200113"
title: "Personal Security: Best Practices"
description: "Privacy and security go hand-and-hand"
metaTitle: "Personal Security: Best Practices"
metaDescription: "Privacy and security go hand-and-hand"
categories: [ "DEVELOPMENT" ]
tags: ["stegos", "Practices", "Security"]
weight: 7
draft: false
---

Privacy and security go hand-and-hand, and the Stegos team is dedicated to ensuring the security of your Stegos nodes and funds, particularly when it comes to exchanges. But as with all crypto, ultimate responsibility lies with the user. Read on for some simple tips to help protect yourself against hackers and nefarious actors!

Our CEO Joel recently commented on the official Stegos Telegram channel about security measures, exchanges and how that translates to executive decisions by Stegos team, along with some  strategies users can employ to protect their STG holdings. (We recommend checking out the original comments [here](https://t.me/stegos4privacy/47177), [here](https://t.me/stegos4privacy/47216), and [here](https://t.me/stegos4privacy/47224).)

### Exchange Vulnerabilities

Now that the Stegos mainnet has launched and everyone has their tokens, some users are understandably itching for us to get an exchange listing. And actually it won't take much scouting to find exchanges where Stegos IS listed. 

But the Stegos team has a consistent position on shunning unofficial exchanges and waiting for an official listing. Why is this?

Stegos isn't just a normal blockchain: it's a truly private blockchain dedicated to keeping your data and metadata safe from prying eyes. A huge part of this is key management.

If you've spent *any* time in community channels, you'll have seen Joel reiterate the risk of sending funds to unapproved exchanges. These exchanges haven't been in contact with the team, any we *know* they haven't been looking at our API documentation, so they just can't know the proper way to integrate safely and securely with the Stegos chain. They're treating Stegos as just any other crypto asset, which it certainly isn't!

Crucially, unofficial exchanges which haven't worked with our devs to integrate their exchange can't properly protect your STG deposits. Worse, there's no way to tell if they're using even basic mechanisms such as offline signing and cold storage. If they're not, then your funds are vulnerable to being stolen.

In order to promote healthy, secure exchange integration, the team has compiled an offline signing API for exchange implementation. This will go live with the next node release. In the meantime, we're working directly with a reputable exchange to implement proper security measures in advance of STG integration. We will announce this exchange once we've received the thumbs up from the partnered exchange. Unfortunately we cannot pre-announce the exchange, as we'd risk them backing out of the deal entirely.

Until then, we must reiterate that **we do not recommend** moving tokens onto unapproved exchanges.  **The Stegos team can take no responsibility** if your funds are stolen or otherwise lost on unendorsed third-party exchanges.

But good security practices aren't just limited to exchanges.

### Protecting Your Keys

With Stegos, your private keys are used to signed outgoing STG transactions. Additionally, your private keys are utilized to scan Stegos blocks to identify and authorize incoming STG from transactions, block rewards, and VSA payouts.

Your STG is best kept at an address which you, and only you, hold the keys to. Additionally, your keys should NOT be kept somewhere that can be easily accessed by unwanted or malicious eyes, such as a cloud server. Instead, you should secure them on a separate device that isn't typically used to connect online: such as a laptop that is kept "cold" and offline.

But aren't we also recommending people use cloud servers for their nodes to maximize their stability and chance of winning the VSA?

The key point for node operators is that your keys are **not** required to forge blocks and validate the network. Of course, nodes must remain online to operate, so cloud servers are a great solution here. But you should always keep your nodes running **on separate servers from your keys**. When your node is connected to the network on the same server your keys are held, **hackers can gain direct access to your funds.**

We're releasing a guide to staking locally and via cloud server this week, but if this seems too complicated for you, remember that the Stegos staking pools are a simple, safe, secure and rewarding option!

### Password Management

The most common attack vector hackers use in targeting users is through passwords. Whether it's through tracking leaks, logging keystrokes, or brute-forcing weak points, your passwords represent a major security risk!

The Stegos team utilizes [1Password](https://1password.com/) to better secure and organize company passwords. Through 1Password, users maintain a master key that can unlock other passwords hosted on the service. We recommend individuals to similarly use 1Password or an alternative password management service as another defence against hackers! If you do plan to follow our lead, we recommend a master password of at least 30 characters and 6-7 numbers and symbols.

We also use two-faction authentication (2FA) on ALL our team accounts to provide a second level of security. Where available, we recommend you do the same.

Join us on Telegram or our forums for more talk about privacy and security.

The Stegos Team

-Website: [https://www.stegos.com](https://www.stegos.com/)

-Forums: [https://forum.stegos.com](https://forum.stegos.com/)

-Telegram: [https://t.me/stegos4privacy](https://t.me/stegos4privacy)

-Wallet: [https://github.com/stegos/stegos-wallet/releases](https://github.com/stegos/stegos-wallet/releases)

-Wiki: [https://github.com/stegos/stegos/wiki/](https://github.com/stegos/stegos/wiki/)

This article was [first published on Medium](https://medium.com/stegos4privacy/stegos-personal-security-best-practices-ca4a5e9e995) on January 12th 2020