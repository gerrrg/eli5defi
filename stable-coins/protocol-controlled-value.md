# Protocol Controlled Value

## Self-stabilizing, no collateral IOU

While most protocols offer rewards to keep your assets in their ecosystem, Protocol Controlled Value doesn't let you take it back -- directly, at least. When you buy the stablecoin from the protocol, the protocol deploys that asset you just gave it \(along with more of the stablecoin\) as liquidity in a secondary market \(DEX\).

This means that when someone wants to buy more of the stablecoin, they can either go to the secondary market, or to the protocol itself, whichever is cheaper.

If the price gets too high in the secondary market \(supply deficit\), reasonable people will buy the token direct from the protocol, which increases supply. If the stablecoin price gets too low in the secondary market \(supply surplus\), the protocol incentivizes buying the token, and penalizes selling it.

The protocol can also correct price discrepancies using a technique like:

1. Remove its own liquidity from the pool
2. Buy the surplus stablecoin from the remaining assets in the pool
3. Redeploy its liquidity in equal parts
4. Destroy \("burn"\) the excess tokens it just bought

This may sound like a bad trade for the protocol. It is! But it provides price stability. But because the protocol _owns_ the value that backs it, it's also able to generate more value so it can afford to provide this service. 

When you give the protocol assets to create the stablecoin, it can actually do more than just provide liquidity to the secondary market. It also can invest parts of it to generate income. How much and where to invest it is up to the governance community.

## Pros

* Don't have to worry about fleeing collateral if better rewards pop up \("Mercenary Capital"\)
* Decentralized
* Protocol can build value of controlled assets
* Protocol stabilizes the price itself 

## Cons

* Still needs to be proven in the market
* Greedy early investors trying to make a quick flip can wreck the price peg

## Example

* FEI \(0x956f47f50a910163d8bf957cf5846d573e7f87ca\)

