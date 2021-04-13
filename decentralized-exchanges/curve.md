# Curve

## What is Curve?

Curve is a DEX that specializes in trading tokens of the same value. Curve started out with stablecoins that track the US Dollar, and has now expanded to trade tokens that represent the same things.

Examples of tokens that can trade with each other:

* USD Stablecoins: DAI, USDC, USDT, BUSD
* Euro Stablecoins: SEUR, EURS
* Bitcoin-Pegged Tokens: wBTC, renBTC, sBTC
* Ether-Pegged Tokens: ETH, WETH, SETH

## How does Curve determine price?

The novelty of Curve is that it does not use a constant product formula like Uniswap. Curve, instead, uses the StableSwap formula, outlined in their [whitepaper](https://www.curve.fi/stableswap-paper.pdf). 

This formula allows for far lower \(claimed ~100x lower\) price slippage than constant product formulas. This works so well on Curve because you can only trade between assets that have the same approximate value.



