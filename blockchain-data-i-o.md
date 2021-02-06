# Blockchain Data I/O

## What data do you want to put on the blockchain?

Often times, there is a desire to have a on-chain data that different contracts can reference. For example, if your contract needs to know the current price of ETH in USD, you might need to ask someone or something else what that price is. Data like that would come from an on-chain **oracle**.

## What data do you want to get off the blockchain?

For just about any website, app, or data stream related to the blockchain, you'll want to look up things like "How many of Token A does wallet 0xabc...0 have?" Since each block is just a series of changes this might not be as easy as you might think to see the "state" of an address. 

[The Graph](https://thegraph.com/blog/) is a protocol that makes querying decentralized data simple. This streamlines other crypto projects by allowing developers to query The Graph \(and specifically, their project's sub-graph\) instead of reading the whole blockchain, analyzing the data, and building their own infrastructure for shoving that data into their system. 

