# Ethereum Basics

## What is Ethereum?

Ethereum is a network of computers running a blockchain\*, and is similar to the technology that powers Bitcoin. Taking the concept of Bitcoin a step further though, Ethereum allows anybody to run programs on the network called Smart Contracts. 

\*A blockchain is decentralized ledger -- a public record of all transactions and balances that anyone can look at and verify. It runs on thousands of computers around the world, validating and synchronizing data.

## What is Ether \(ETH\)?

Ether \(ETH\) is the native asset of the Ethereum network. It is used to pay transaction fees, and has a market-defined value.

## What is an Ethereum Wallet?

A [wallet](https://ethereum.org/en/wallets/) is a unique address that allows a user to interact with the blockchain. It maintains your ETH balance and has your transaction history. 

Each wallet has two parts: a public and private key. Think of these as account and password. To move ETH from one account to another, a user needs to sign a "send" transaction with their private key. Users also approve transactions interacting with Smart Contracts.

## Is Ethereum free to use?

It is free in the sense that anyone is _allowed_ to use it, but there are transaction fees, called gas, associated with the network.

## What is gas? Why are the fees so high?

Ethereum miners make the network run by validating transactions and recording them on the blockchain; they don't, however, do this for free.

**Gas** is how you quantify the amount of work that an Ethereum Miner has to do to process your transaction. More complex calculations and increases in storage take more work, so gas amount increases. With all things being equal, the _amount_ of gas for a specific action will remain the same over time.

**Gas Price**, however, can change over time. Ethereum users must compete with each other to get their transactions processed. Users can use high gas prices to pay their way to the front of the line of pending transactions. When the network gets crowded, gas prices rise as users push to get their transactions validated faster.

**Failed Transactions** also get charged gas fees. It's a bummer, but it's necessary; otherwise, malicious users could spam the network for free. A transaction may fail for a variety of reasons, but a common reason is that trade prices change between when you _sign_ the transaction and when it _executes_. It's important to note that when a transaction fails, the gas fees go to the Ethereum network \(specifically the miners\), not whatever app you're using.

Gas fees are paid in ETH. Websites like [Eth Gas Station](https://ethgasstation.info/) publish current gas prices denoted in Gwei \(1 \* 10e-9 ETH\).

## What's a seed phrase?

A seed phrase is a string of characters used to generate a private key. Most commonly, it is a list of 24 random words. You should never store your seed phrase on your computer -- you should write it down on a piece of paper and hide it somewhere memorable but secure. Whoever has this list of words has direct control over your Ethereum wallet.

## A quick note about security...

There are many people out there who want to make quick money by stealing your assets. Scammers have been making convincing websites that look like DeFi pages, but they ask you to enter your private key or seed phrase. You should not give out your private key or seed phrase to anyone. When interacting with DeFi websites, you should use a wallet provider. The most common one is called MetaMask.

If you want to go a step further, you can use a hardware wallet. This is a small device that looks like a USB flash drive. The private key is generated and stored on the device, not on your computer. When you send a transaction, the raw transaction is sent over USB to the hardware wallet for signing, and the approved transaction is sent back over USB to your computer. This never exposes your private key to anyone, even if they have access to your computer.

## Deep Dive on Ethereum

If you want a good resource for learning the nitty gritty of how Ethereum works, check out [Mastering Ethereum](https://github.com/ethereumbook/ethereumbook/blob/develop/book.asciidoc), available for free on GitHub.





