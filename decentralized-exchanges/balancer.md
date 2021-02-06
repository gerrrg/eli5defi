# Balancer

## What is Balancer?

Balancer is a decentralized exchange that allows anyone to trade ERC-20 tokens. While Uniswap uses a one-size-fits-all approach to pool design, Balancer exposes a tremendous deal of flexibility in liquidity pool design. Balancer pools can have up to 8 assets and the trade fee is determined by the pool creator. Trade fees can range from 0.0001% and 10%. Additionally, assets can have unequal weightings, so instead of using 50/50, someone could make a pool that has an 80/20 weighting to reduce [Impermanent Loss](https://explain.eli5defi.info/decentralized-exchanges#what-is-impermanent-loss-il).

## What's the advantage of multi-asset pools?

With multi-asset pools, a trader can come and trade between any two assets in a pool. This means that with a single pool with 8 assets, the liquidity provider is making 28 \(8 choose 2\) different trading pairs available. This high number of pairs means more potential trades, and more trade fees. 

## What else can Balancer do?

Balancer has Smart Pools, which have a number of interesting features including surge pricing, liquidity bootstrapping, and more. 

Balancer has [recently announced](https://medium.com/balancer-protocol/balancer-v2-generalizing-amms-16343c4563ff) their Version 2, which is scheduled to be released in March 2021. New features will include:

* Even more customization in trading pools
  * Including Stablecoin-focused price formulas
* Reduced gas usage
* Protocol Vault for all pool assets
  * One contract holds all assets instead of each pool holding its respective assets
* Two types of Price Oracles
  * Resilient
  * Low gas cost
* Asset Managers

See more details in the Medium post linked above!

## How are prices determined?

Balancer uses a "constant product" formula like Uniswap does, but with the increased number of assets and varied weights of assets in a pool, the equation looks a bit more complicated:

$$
\prod{{x_i}^{w_i}}=k
$$

 Instead of the "xy=k" of the Uniswap formula, Balancer's formula accounts for the custom weight by raising each "x" its weight's exponent. 

While spot price \(_SP_\) in a Uniswap-style pool can be calculated with:

$$
SP = \frac{B_i}{B_o}
$$

With _Bi_ as the balance of the input and _Bo_ as the balance of the output, a Balancer-style pool calculates spot price accounting for the weights, _Wi_ and _Wo_, of the input and output assets as well.

$$
SP = \frac{(B_i/W_i)}{(B_o/W_o)}
$$



