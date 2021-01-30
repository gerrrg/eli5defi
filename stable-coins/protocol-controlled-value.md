# Protocol Controlled Value

## Self-stabilizing, no collateral IOU

While most protocols offer rewards to keep your assets in their ecosystem, Protocol Controlled Value doesn't give you much of a choice. When you buy the stablecoin from the protocol, the protocol deploys that asset you just gave it \(along with more of the stablecoin\) as liquidity in a secondary market \(DEX\).

This means that when someone wants to buy more of the stablecoin, they can either go to the secondary market, or to the protocol itself, whichever is cheaper.

If the price gets too high in the secondary market \(supply deficit\), reasonable people will buy the token direct from the protocol, which increases supply. If the stablecoin price gets too low in the secondary market \(supply surplus\), the protocol itself can correct this using a technique like:

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
* Protocol stabilized the price itself 

## Cons

* Still needs to be proven in the market
* Crypto-asset backing locked in liquidity pool

## Example

* FEI \(has not been deployed at time of writing\) \([read the whitepaper!](https://fei.money/static/media/whitepaper.7d5e2986.pdf)\)

