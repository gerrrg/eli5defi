---
description: >-
  Because Coinbase "crashes" when prices move too much, and RobinHood sells your
  "risky" positions for you to "protect you"
---

# Decentralized Exchanges

## What is a DEX?

A Decentralized Exchange \(DEX\) is a system that allows users to trade crypto. DEXs never close, and most of them allow anybody to list any token they like, so long as it's compatible. In general, DEXs allow you to trade any ERC-20 token.

DEXs are built on Smart Contracts. Each DEX has a series of contracts for different trading pools. Each of these pools is an Automated Market Maker \(more below\).

DEXs are remarkable in that a trader doesn't need to trust the "other party" in a trade. These exchanges happen entirely between a trader and a contract, and the transactions are atomic, so the send of Token A happens at the same time as the receive of Token B.

## Where do the tokens come from?

People looking to passively generate income from their tokens can become liquidity providers \(LPs\) at decentralized exchanges. This means they put their own tokens into the DEX contracts and let people trade between them. When someone makes a trade, the pool gets to keep a small percentage as a fee.

## How does a DEX know what price to charge?

DEXs generally don't use outside price feeds. Instead, they have equations that set prices according to certain rules. Since anyone can trade with a DEX, anyone can make a profitable trade when the prices disagree between exchanges. This is called arbitrage, and it is how DEX prices reflect and influence market prices.

These equations are the foundations of Automated Market Makers \(AMMs\). Different DEXs use different formulas, but they all take the quantities and weight of assets into account.

## What is "Impermanent Loss" \(IL\)?

Impermanent Loss is the difference in value between holding a set of assets and providing liquidity for those same assets.

Some people find the word "Impermanent" misleading and prefer to call it "Divergence Loss" or "Rebalancing Loss" because one token may perpetually out-value another token, and the loss may seem... permanent. Anyway, let's look at an example:

Let's start a pool with two tokens, each worth $1USD.

* 100 of Token A 
* 100 of Token B
* Total Value: $1\*100 + $1\*100 = $200

Now let's pretend that suddenly, Token A becomes worth twice as much at $2USD. People will trade with our pool until the price in our pool approaches the price of the market. If this pool uses a **constant product formula** \(see the pages about [Uniswap](https://explain.eli5defi.info/decentralized-exchanges/uniswap) and [Balancer](https://explain.eli5defi.info/decentralized-exchanges/balancer) for the relevant math\), our pool balances will approach these:

* 70.7 of Token A
* 141.4 of Token B
* Total Value: $2 \* 70.7 + $1\*141.4 = $282.80

Now we might be thinking, wow we made $82.80 in profit, that's great! And though we should never complain about making money, we might notice that we could have made a bit more money if we hadn't put our tokens in the pool to begin with:

* 100 of Token A 
* 100 of Token B
* Total Value: $2\*100 + $1\*100 = $300

So in this example, our IL is $300 - $282.80 = **$17.20**, or **5.7%** of $300. Read more about Impermanent Loss [here](https://blog.bancor.network/beginners-guide-to-getting-rekt-by-impermanent-loss-7c9510cb2f22?gi=789c65d67891). Why might someone choose to provide liquidity despite this loss? A few reasons:

1. They expect the price ratios to be stable in the long term
2. Trading fees
3. [Liquidity mining rewards](https://explain.eli5defi.info/incentives#liquidity-mining-transaction-mining-yield-farming)

#### Reducing Impermanent Loss

In the above example, we had an even pool with 50/50 weighting. This is the type of pool you can get if you use Uniswap. Using a provider like Balancer, however, you can change the pool weights to be 33.3/66.6, 20/80, or even 2/98. Using an asymmetric pool can give you more exposure to price movement in assets that you expect to perform well. Read more about the advantages of asymmetrically weighted pools [here](https://medium.com/balancer-protocol/80-20-balancer-pools-ad7fed816c8d).

![IL at different Pool Weights. Image by Fernando Martinelli \(Balancer Labs\)](../.gitbook/assets/il.png)



