# Hardhat Sample Project (Web3)

This page is dedicated to help developers in getting started with our sample hardhat project which utilizes our web3 hardhat plugin to connect hardhat with Thor. This enables developers to be able to deploy and test smart contracts on Thor in a seamless manner using all the known tools provided by hardhat.

## Prerequisites

```bash
git
npm
typescript
```

## Setup

First, clone the sample project from our repository

```bash
git clone git@github.com:vechain/hardhat-plugin-sample-web3.git
cd hardhat-plugin-sample-web3
```

Then install the required node modules by running

```bash
npm install
```

### Install VeChain's Web3 library

```bash
npm i @vechain/web3-providers-connex
```

### Install VeChain's Hardhat plugin

```bash
npm i @vechain/hardhat-vechain
npm i @vechain/hardhat-web3
```

## Start Thor

To be able to run the tests on VeChain you need Thor installed, which is VeChain's node implementation. We have a detailed guide on how to do that [here](https://github.com/vechain/vechain-docs/blob/main/developer-resources/frameworks-and-ides/hardhat-and-vechain/broken-reference/README.md).

## Running the tests

```bash
npx hardhat test --network vechain
```
