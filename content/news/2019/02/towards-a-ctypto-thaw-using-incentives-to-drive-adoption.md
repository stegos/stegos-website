---
author: "Joel Reymont"
linktitle: Crypto Thaw
title: "Towards a crypto thaw: Using incentives to drive adoption"
metaTitle: ""
metaDescription: ""
categories: [ "OVERVIEW" ]
tags: ["stegos", "design", "competition"]
date: 2019-02-11T21:02:22+06:00
weight: 10
draft: false
---

As the crypto winter stretches past the twelve-month mark, many people are asking what went wrong and when (or indeed if) it’s going to end.

But the diagnosis isn’t mysterious. And neither is the cure.

Fostering breathless excitement about price and moon lambos was always unsustainable. Yes, ICOs injected a lot of tokens into the ecosystem, but that’s not how you bootstrap. Cryptocurrencies only have value if they’re useful, so we need people to use them. HODLing and trading aren’t true adoption, and without true adoption we won’t get anywhere.

I realize this isn’t exactly a revelation. There are countless articles, even from long before the crypto winter, making the same basic three-point case:

1. Crypto isn’t a gimmick or a scam. It has enormous real-world utility.
2. But theoretically useful things only become genuinely valuable if they’re actually used.
3. People won’t use their crypto if they think it’s about to explode in value.

Which is all well and good, but it’s February 2019. No-one thinks their crypto is about to explode in value any more. And the first two points about crypto’s potential are as true as always. And yet it’s still winter. So what’s going on?

Well as with anything in tech, just identifying the problem gets you nowhere. Any armchair futurist can see what went wrong, maybe throw in some vague talking points and a nod towards “gamification”, as if that means anything on its own. We know adoption is the problem, and we know incentives are the answer, but no-one has made any progress beyond that.

We need a viable and actionable plan.

So what should crypto projects do to drive real, sustainable adoption? At Stegos, I believe we’ve found the answer. Like all good plans it’s tailored to our specific requirements, but I think there is a lot that will hold true for any crypto project feeling the bite of crypto winter.

## Forget the tech

First, projects need to stop relying on their technology alone to attract investors. The base technology is proven at this point – what’s doubtful is whether enough people want to use it. Clear models for how a project plans to attract and retain users are far more valuable.

From a user perspective, adoption has two dimensions: incentives and accessibility. Or, to put it another way: “What do I get out of it?” and “What do I have to do to get it?” These are closely linked. People will put in a lot of effort for a high enough reward, and with a low enough barrier to entry people will find even modest incentives enticing (but only if they don’t already have a good alternative, or often even a markedly inferior one. We’ll circle back to that.).

From a project perspective, the questions are different: “What can we offer users?” and “What do we want in return?” The standard answers here are “A solid crypto use case” and “For people to flock to our platform (but we haven’t built anything yet, so for now just our Telegram)”, but these are woefully insufficient.

“Look at our use case!” has been the standard line for the whole of 2018 (ever since investors woke up to the fact that projects basically just yelling “CRYPTO! YEAH!” wasn’t much of a value proposition). And its not working. Users aren’t interested, and investors certainly aren’t buying it.

Maybe there is a killer use case out there that’s good enough to attract everyone to a brand-new platform, sight unseen. But it would have to be lifechanging.

That’s because there aren’t just barriers to entry, there are barriers to exit. People are locked in to their existing tech and services. Someone might only ever have bad things to say about their bank – but it’s still going to take a lot for them to leave the safety of the established system and shift to something they see as new and scary.

No, those users have to come later, once the platform has grown enough. To start with, it’s important to focus on people who are already on board with crypto.

So what do they want? Well, you only have to look in any project Telegram or Discord to find out. They want tokens. And what do they want to do to get them? As little as possible, frankly.

Well, luckily, tokens are exactly the thing that every crypto project has to offer.

## Tokenized incentives

But if we use our tokens as incentives, aren’t we just back where we were before? Handing out tokens like candy, hoping that’s the same as bootstrapping a platform?

Not at all. The key is in the second question. We’re offering tokens: What do we want in return? In our case, the answer is active participation. Stegos is a privacy coin that benefits strongly from having a large number of active users. And not just active in the sense of hanging around on Telegram asking when the next airdrop is. Running nodes, validating transactions, growing and securing the network.

Which brings us back to accessibility.

“What do I have to do to earn tokens?” “Run a node.” “That’s too hard. I’m out.”

So we’ve decided to make it easy. And not just crypto easy. Actually easy.

Most people are never going to set up a crypto node as they exist today. It’s complicated and scary. What they will do is download and install an app on their phone. So we have to make that possible. And not just a minimally functional light wallet. Remember: we’re trading these tokens for active participation. It needs to be a fully functional node that’s helping to validate and maintain the blockchain.

(The question of how that’s possible will have to wait for the next article: the short answer is that Stegos uses a unique method of cryptographic pruning to ensure the blockchain is always kept small enough for smartphone nodes to be viable.)

## Finding the balance

Now comes the crucial part. We need to decide how to distribute these tokens to maximize incentivization across the board. Who gets tokens, and in what proportion? A lot of crypto projects handwave their incentives with catch-all concepts like “Everyone gets incentivized” or “Everyone gets paid”, but that’s not a useful model. Everyone in a sweatshop gets paid, but you wouldn’t want to work there.

“Everyone gets paid” isn’t sufficient on its own. Everyone needs to get paid enough.

If a project is running its own blockchain, then tokens are distributed to miners or validators via the regular block rewards and the transaction fees, depending on the chosen consensus mechanism. The Stegos blockchain is designed to run on phones, so Proof-of-Work (PoW) is immediately out. It’s too computationally expensive, and it uses too much energy.

So we’re using Proof-of-Stake (PoS). Proof-of-Stake is the perfect choice for smartphone users, as it’s inexpensive and low effort.

But PoS has its own problems. The average user doesn’t have much to stake, so they hardly ever win the right to create a block. Users can pool their stakes, but this gets messy and complicated. So the small stakes drift away, and the network gradually centralizes around the whales.

Of course, those whales are important! They’ve invested the most money. But the little guy is important too, or the network won’t grow. We’ve tweaked the token distribution to incentivize our smartphone users without discouraging large stakers. Instead of giving the entire block reward to the winner of each consensus round, a proportion is given to every active validator. So everyone running a node is constantly earning.

That’s a good start, but it won’t be enough on its own.

How can we give everyone a lot of tokens, without totally devaluing the block rewards? The answer is to offer everyone the potential of getting a LOT of tokens. Instead of only awarding tokens based on stake, we also add a lottery mechanism, based on a unique algorithm for providing verifiable distributed randomness designed by the Stegos team. Part of the block reward for each block is added to a jackpot pool, which is periodically awarded to a random single validator. As the jackpot grows, it’s more likely to be awarded. We’re also always seeding the next jackpot, so winning doesn’t reset the prize pool to zero, killing the incentive.

## Don't lose sight of the fundamentals

It’s important to not go overboard. The block reward must remain the highest and most reliable form of income. The network needs large stakes to increase security. But Stegos’s extra gamified layer which the lottery adds means there’s always an incentive to be a validator, especially because it’s virtually no effort thanks to the smartphone app. It’s also fun, which is an essential component of long-term engagement. The size of the current jackpot is always visible, and it grows with every block until it’s been won. The odds of winning increase the longer you’ve been validating, too, which will encourage user retention.

There are always more tweaks to make, different types of incentives for behaviors helpful to the project. For example, new wallets could be seeded with a small number of tokens, so everyone can start running their node right away.

We’re still balancing things, but the crucial point is that we’re not trying to convince people based solely on our innovative tech or various use cases (although of course those are also important, and I’ll be talking about them in future articles). We’ve made incentives and adoption a cornerstone of the platform, not just an afterthought.

The crypto boom showed us that people love getting tokens. Escaping crypto winter is simply a matter of being creative in how you give people what they want.
