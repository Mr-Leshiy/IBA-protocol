# Inter-Blockchain Api Protocol description

## Purpose
Build a protocol for blockchains to communicate with each other in the secure, trustless and transparent way.
IBA provides standatized way how to connect to the whole "Internet of Blockchains" and how to communicate with each other directly.

## Simple use case

Lets consider two separate blockchains for example Ethereum and Bitcoin. These blockchains want to have an ability to share their assets with each other, in our case assets are coins. And of course we want to do it in a secure way.
We need to have an ability to create a new transaction which will transfer Bitcoin coins to the Ethereum one and vice-versa. But we conside an exchange from Bitcoin to Ethereum, so `user1` which will transfer his Bitcoin coins to `user2` will get Ethereum coins from `user2` and `user2` will receive Bitcoin coins.
## Problem statement
To do this we need to solve the folowing problems:
1. **Blockchain connection** - we need to get possibility to connect one blockchain network to another one, so as result we need to get a decentralized connection with the two networks. In our case we do not consider to provide comunication with blockchains throught the another one, we want to avoid this uneeded layer.
2. **Blockchain api standartization** - every blockchain has unique functionality with the unique interface, even for the coin transfering we can have two different functions with the different agrument list, argument type etc. So each blockchain should certainly know how to invoke the fucntionality from the another one. We need to simplify it and provide and standartized scheme how to call an any available function from the any blockchain.
3. **Interaction's security providing** - we need to have a guarantee that interaction between blockchains is secure. every blockchain should know or should have possibility to validate that an action which we have been executed in the another blockchain has been successfully applied or not.

## Inter-Blockchain connection layer
