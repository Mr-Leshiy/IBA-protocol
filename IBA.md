# Inter-Blockchain Api Protocol description

## Purpose
To get an easy to implement protocol for any blockchain to communicate with each other in the trustless and transparent way.
IBA provides an easy and standart way how to connect to the whole Internet of blockchains and standart how to communicate with each other.

## Simple use case

Lets consider two separate blockchains for example Ethereum and Bitcoin. These blockchains want to have an ability to share their assets with each other, in our case assets are coins. And of course we want to do it in a secure way. 

## Problem statement
To do this we need to solve such problems:
1. **Blockchain connection** - we need to get possibility to connect one blockchain network with the another blockchain network to get a decentralized connection with the two networks. In our case we do not consider to provide comunication with blockchains throught the another one, we want to avoid this uneeded layer.
2. **Blockchain api standartization** - every blockchain has unique functionality with the unique interface, even for the coin transfering we can have two different functions to do this with the different agrument list, argument type etc. With the case of the interaction each blockchain should certainly know how to invoke the fucntionality from the another blockchain. So we need to simplify it and provide and easy scheme how to invoke an any available function from the any blockchain.
3. **Interaction's security providing** - we need to have a guarantee that interaction between blockchains is secure. every blockchain should know or should have possibility to validate that action which we have been executed in the another blockchain has been successfully applied or not.