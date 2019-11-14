---
title: "Smart Contracts Are Useless"
linktitle: Smart Contracts Are Useless
author: "Joel Reymont"
date: 2019-02-22T12:05:29+01:00
description: ""
metaTitle: ""
metaDescription: ""
categories: [ "OVERVIEW" ]
tags: ["stegos", "design", "smartcontracts"]
weight: 10
draft: false
---

The ideas behind smart contracts are [over twenty years old](http://www.fon.hum.uva.nl/rob/Courses/InformationInSpeech/CDROM/Literature/LOTwinterschool2006/szabo.best.vwh.net/smart.contracts.html), but smart contracts only became a major talking point in the past five years, with the release of Ethereum and its Solidity programming language. 

For much of 2017, you couldn’t move for ICOs promising to use smart contracts to revolutionize the way we transact and do business, and the cryptosphere is still awash with articles explaining the coming [smart contract revolution](https://blockchainmagazine.net/the-smart-contract-revolution-is-coming/), how smart contracts are going to disrupt everything from [logistics](https://medium.com/@credits/how-blockchain-could-help-logistics-c3b2ab60be55) to [real estate](https://medium.com/ethereum-dapp-builder/smart-contracts-and-the-real-estate-59e3dfdb5d2c), will put [lawyers everywhere out of jobs](https://qz.com/459009/the-technology-behind-bitcoin-could-replace-lawyers-too/), and render thousands of years of developments in human contract law obsolete.

But now it’s 2019, and what have smart contracts got us? Endless ERC20 tokens and [fake cat breeding](https://www.cryptokitties.co/)…

That’s a little harsh on ICOs and CryptoKitties, which are undeniably important, at least as proofs of concept. But what else is there? Where are the billion-dollar, market disrupting businesses people promised? Where are the life-changing dApps? Of all the Ethereum dApps written so far, [only 10% are used on any given day](https://www.longhash.com/news/ten-percent-of-ethereum-dapps-are-used-on-any-given-day). EOS dApps fare a little better, [but fewer than 5% have more than 2000 daily active users](https://www.longhash.com/news/over-50-of-eos-dapps-are-used-on-any-given-day-compared-to-10-of-eth-dapps).

The fact is, smart contracts are useless and will continue to be useless for the foreseeable future. There’s nothing smart about them — they’re dumb programs with limited capabilities that can only access data stored on the blockchain and cannot talk to the outside world. 
The breathless crypto pundits claiming that all contracts are just fancy chains of [nested IF-THEN statements](https://www.forbes.com/sites/forbescoachescouncil/2018/05/16/how-smart-contracts-could-change-the-way-you-do-business/#236a2f6c1288), so obviously they can be replicated in machine language, haven’t grasped the first thing about what makes contracts useful, how and why they work, and why problems and disputes arise.

How have we ended up down this blind alley, and what should we be doing instead?

First, let’s look at how smart contracts work, and then I’ll explain why they emphatically _don’t work_ in any meaningful way.


## How do smart contracts work?

Smart contracts are small computer programs that every blockchain node is required to run periodically. Nodes have no control over the instructions that a smart contract executes and thus should not trust it with full access to the resources of the machine the node runs on.

Due to this lack of control, blockchain projects come with _virtual machines_ (VMs) that focus on making smart contract execution safe. The VM serves as the _sandbox_ that prevents smart contracts from wreaking havoc on the host computer. Each VM runs a very limited set of instructions, also called _byte codes_, that comprise each smart contract (e.g., arithmetic operators, blockchain transactions, etc.). Naturally, this means that smart contract functionality is super-limited compared to natively running machine code. 

Smart contracts also cannot be allowed to run forever, indefinitely tying up the resources of their host computer. Smart contracts are guests in someone else’s house and must leave eventually. Unfortunately, one of computing theory’s [most famous results](https://en.m.wikipedia.org/wiki/Halting_problem) means it’s impossible to know whether your average smart contract will ever stop running, so VMs resort to counting byte code and forcing the smart contract to stop at some point. This is the only way to ensure smart contracts stop without restricting functionality even further, but it makes them extremely obnoxious to actually use.

Are you a smart contract owner? Did you pay enough to deploy the smart contract? No? Then your contract will just stop mid-execution. Even if you’re careful, the gas price fluctuates all the time, so it’s impossible to properly budget the costs of running contracts. 

And the problems aren’t limited to the owners. The block winner updates the blockchain with the results of smart contract execution and is compensated with block rewards and transaction fees. But the rest of the network must run the same smart contract to check these execution results for no reward. Are you a node operator who didn’t win the right to sign the block? Tough luck — you still have to waste computing cycles executing the smart contract. And no, you won’t get paid for it!

## No access to the outside world

It’s often argued that many or most real-world contracts can be expressed as collections of IF-THEN statements. _If_ some condition is met, _then_ process the appropriate clause of the contract. _If_ I receive 100BTC, _then_ transfer ownership of my house. _If_ the customer doesn't return your rental car by the agreed upon date, _then_ apply the fine. IF-THEN statements are a computer’s bread and butter, and blockchain lets us run these programs in a trustless environment, so why should we fork out $200 an hour for a lawyer? 

This might sound compelling, but it’s sneaky sleight of hand. Lawyers and notaries and thousands of years of legal apparatus aren’t all just a clumsy input/output processing system. The problem of validating whether real-world conditions have been met and then reaching an agreement on that validation is extremely hard, and smart contracts get us precisely nowhere towards solving it.  

Imagine: Say how your contract resolves is contingent on what time it is when it executes. That seems reasonable, right? But blockchains have no objective source of time. So your smart contract needs to access an outside time service. Calling the time service returns the current time down to the millisecond, which is then used to execute the contract. The results of this contract execution are then added to the blockchain. 

But because the results are being added to the blockchain, all nodes must agree on them. This is part and parcel of maintaining blockchain consensus. But remember, every node is running these contracts independently in their own VM. So they're all accessing the time service at slightly different times and receiving slightly different timestamps. So when it’s time to validate the next block the results of smart contract execution will be different for every node. 

(And it’s no good saying we don’t care about millisecond-level accuracy, let’s just round to the nearest second, minute, hour, whatever. With thousands of nodes all accessing the same service at different times, the difference between rounding decisions is inevitably going to come down to a millisecond, and you’re back at the same problem.)

No matter how you swing it, the nodes will never agree with each other and the blockchain will never reach consensus.
 
## Enter the oracles

Since smart contracts cannot access the outside world, the outside world must be brought to smart contracts. Some entity can put data from the outside world onto the blockchain, making it available for all future smart contracts run across the network. These entities are called _oracles_.

But this doesn’t really help us. The data needs to be on the chain before we use it, but how can we know what data we’ll need? We can’t stuff every fact of life onto the blockchain. All modern blockchains already suffer from bloat.

So oracles are limited to a very narrow view of the real world. But the problem doesn’t end there. Even if we agree on a handful of data sources to have oracles for, that data will evolve with time. And every time it does, the oracle must add more data to the blockchain. The old data often becomes obsolete, yet it stays on the chain. Think of the time service mentioned above and how incredibly wasteful it would be to include timestamps on a blockchain that keeps all transaction history.


## Oracles must be paid

Oracles need incentives for putting data on the blockchain — they want to get paid. But oracles aren’t like blockchain validators, who receive ongoing rewards for maintaining the blockchain: once an oracle has put data on the blockchain, that data will be available for anyone to access. The oracle developer has no control over how many times data will be accessed, potentially spreading that single payment over thousands or millions of smart contract invocations and reducing the payment per access to a minuscule amount. This reduces the incentives for oracles to provide truly valuable information.

## Oracles must be trusted

Smart contracts are supposed to be trustless, but this only applies while they’re tethered to the trustless nature of blockchain consensus. As soon as they leave the blockchain sandbox, an element of trust is introduced. Smart contract developers and users must trust the oracle to provide true and precise information. Lack of proper oracle incentives encourages the proliferation of scammy oracles that provide junk data. Such an oracle would hope to collect at least one payment from someone before the smart contract developer realizes the data is crap and stops using the oracle.

Blockchain developers could try to prevent the plague of oracle scams by building a reputation system into their platform. But there’s nothing preventing a sly oracle developer from building up a reputation by providing a few valuable answers before switching to providing stale or junk data and collecting payments for free. Social stigma does not translate to machine code!

Nor can you sidestep this by obtaining answers from multiple oracles and cross-checking or averaging them. Relying on multiple oracles for answers increases security and decreases the need for trust in a single oracle answer, but quickly devolves into a blockchain consensus issue of its own. Think of it as the _oracle consensus problem_. Plus, the still unresolved-problem of oracle incentivization just got exponentially worse!

Oracles need to be both incentivized for providing correct answers and punished for providing false information. Consensus needs to be reached on the one true answer among those provided by different oracles and this mechanism needs to be cheap to use for smart contract developers or it will not be used. None of these things are possible without introducing an element of trust, and if you’re prepared to do that, then why are you messing around with blockchains? We have plenty of long-established trust-based systems which are far cheaper and simpler to use.
 
## You are what you eat

But perhaps your ambitions for smart contracts are less lofty. Blockchain and smart contracts have been proposed as a way to streamline logistics, by tracking shipments and following raw materials and products all the way along the supply chain.

Automatically tracking, say, oranges all the way from the farm to our fruit bowls seems like the kind of tedious busywork that computers excel at. But using smart contracts to automatically release payments when a shipment arrives just runs into the same trust problems, though. We still need to trust a human to make sure the oranges are in good condition and to enter correct data into the system that will put the data on the blockchain. We also need to trust some external system to correctly verify that the oranges arrived. There are certainly some auditing benefits here, but it's still a billion miles away from the automated paradise people were schilling during the ICO boom.

## Smart contracts have no power 

So that’s the IF part of our IF-THEN statements. What about the THEN? Well it turns out things aren’t any better there, either. Smart contracts have no power to rule over the outside world; they can only adjudicate on digital assets. Sure, you can tokenize your house, sell it on the blockchain and try to collect mortgage payments through a smart contract, but the smart contract won’t be able to repossess the house on your behalf in the event of non-payment. The smart contract won’t be able to access the government registry to update ownership of the house either. So you’re still going to need lawyers and notaries and governments and bailiffs and the whole messy trust-based apparatus we've been using for thousands of years. 

## A blind alley

And that's just the theoretical problems. The practicalities are a nightmare too. Despite smart contracts being pitched as the simple alternative to paper contracts, people are absolutely terrible at writing and securing them. Billions of dollars have been lost and stolen due to loopholes and bugs in smart contracts.

In short, smart contracts are trying to solve the wrong problem. They're looking at IF-THEN and deciding the important part is the dash. 

The truly smart contracts are the legal contracts we have been using for centuries now. We don’t need a computer to run these contracts — we have the best computer to interpret them right between our ears! We can use the courts to adjudicate over these contracts and the power of the government to enforce them. 

But enough griping. Hopefully I've convinced you smart contracts are nothing more than a beguiling blind alley. But what should we be doing instead?

## Autonomous agents on the blockchain 

Smart contracts are useless, but the blockchain is still an incredible innovation. Decentralized ledgers facilitate [triple-entry accounting](http://iang.org/papers/triple_entry.html), otherwise known as [the most important invention in the last 500 years that everyone missed](https://hackernoon.com/why-everyone-missed-the-most-important-invention-in-the-last-500-years-c90b0151c169). Think of the blockchain as the master ledger into which all transactions are entered and from which other internal systems are updated. 

Instead of trying to get the blockchain to access the outside world, let’s focus on doing the opposite. The capabilities of smart contracts pale in comparison to applications that can directly access the blockchain. The distributed ledger and consensus are great mechanisms for implementing web, mobile, and other kinds of applications, the kind that we have been writing and deploying for ages now.

We've gotten really good at building computer applications using the full power of the hardware available to us. The missing link is how to allow apps to communicate privately and securely in a way all parties can trust, all without having to pay some centralized authority to manage (and doubtless spy on) the proceedings. What we really need is a decentralized _message bus_ that these applications can use to communicate. We are building just such a message bus at Stegos and it’s part of our [platform for building privacy applications](https://github.com/stegos/stegos). 

Stegos will enable a future where smart autonomous agents communicate using a blockchain, privately and confidentially. In a future article, I'll be explaining how that will work and why it's so important. In the meantime, [join us on Telegram](https://t.me/stegos4privacy) to follow our progress!

