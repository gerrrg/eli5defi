# Aave

## What is Aave?

Aave is a lending platform. It provides lending and borrowing for collateralized loans as well as uncollateralized loans.

## What is a Flash Loan?

While much of DeFi tries to replicate financial tools that exist in TradFi, Flash Loans are a new tool made possible by programming guarantees. Flash Loans require no collateral because they must be returned in whole \(plus interest\) immediately. This guarantee is enforced by the fact that if the loan can't be paid back, it is never issued. 

To take out a Flash Loan, users must submit a single transaction that outline exactly everything what will happen with the money. An example of a successful Flash Loan transaction chain would be one that:

1. Get a loan for 3,000,000 DAI on Aave
2. Trade 3,000,000 DAI for 5,000 TokenA on Balancer
3. Trade 5,000 TokenA for 3,050,000 DAI on 1INCH
4. Return loan + interest of 3,002,700 USDC on Aave
5. Profit = $47,300 \(minus gas fees\)

## What are the collateralized interest rates?

Interest rates are set by the market. The more borrowing, the higher the interest rates become. 

## How much collateral is needed?

Collateral is determined by [risk parameters](https://docs.aave.com/risk/asset-risk/risk-parameters). 

## When are loans liquidated?

Liquidation is determined by the Health Factor, which represents the safety of your loan. The Health Factor is a ratio of how collateralized your loan is. When Health = 1, the value of the amount borrowed \(plus fees\) is equal to you value of your collateral \(with a safety factor\).

