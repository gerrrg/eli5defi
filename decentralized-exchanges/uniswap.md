# Uniswap

## What is Uniswap?

Uniswap is a decentralized exchange that allows anyone to trade ERC-20 tokens. As of this writing, it is the most widely used DEX.

## How does providing liquidity work?

As LPs add their liquidity to pools, they get a placeholder token in return. On Uniswap, this is a UNI token specific to that pool. These UNI tokens are effectively vouchers that denote that person's share of that pool. When the LP "cashes in" their UNI tokens and takes out their tokens, they are not guaranteed \(or expected\) to receive the same amounts they put in for a couple reasons.

1. The pools accumulate trade fees. 0.3% of all inputs are collected by the pool.
2. The prices of Token A and Token B have like shifted, changing the value ratio \(and therefore amount ratio\) of A:B

## How are prices determined?

Every Uniswap liquidity pool has a 50/50 distribution, so the value of Token A is \(approximately\) the same as the value of Token B. The price to exchange one token to another can be calculated with a simple "constant product" formula. 

$$
xy = k
$$

_x_ is the amount of Token A in the pool, and _y_ in the amount of Token B in the pool. When you trade a certain amount of Token A, the amount of Token B that you get out is calculated such that _k_ is constant.

For a simple example, let's say Token A is worth 3 times more than Token B, so a pool might have 10 of Token A and 30 of Token B.

$$
10 * 30 = 300
$$

If someone comes along with 3 Token A and wants to trade for Token B, we can determine the amount of Token B out like this:

$$
(10 + 3)*(30-TokenB_{out}) = 300
$$

$$
TokenB_{out} = \frac{30 - 300}{(10+3)} = 6.92
$$

You may be saying to yourself "but 6.92 isn't 3 times more than the 3 Token A" and you would be right. We call this "price slippage." In an AMM, each trade effects the price, but as the liquidity increases, slippage decreases. In our example, the slippage was so high because the trade amount was large compared to the amount in the pool. 

## 

