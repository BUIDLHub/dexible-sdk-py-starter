# Dexible SDK Python Starter

## Overview
This sample project is a good starting point for interacting with Dexible through its SDK. The 'twap' example shows how to construct the order algo/policies and various settings you can tweak to create and submit an order. For more in-depth examples, see the [dexible-sdk-py](https://github.com/buidlhub/dexible-sdk-py) project examples package.

## Prepare

You should have the dexible SDK installed in your environment or in `PYTHONPATH`.  Just run `pip install dexible` to cover all.  

## Environment
The following environment variables should be set at runtime. Having `python-dotenv` installed allows you to place those in a .env file at the project root. This file is sensitive and should never be committed back to any github repo.

|               |                                                                                            |
|---------------|--------------------------------------------------------------------------------------------|
| `INFURA_PROJECT_ID` | Used to create a web3 provider that the SDK uses for on-chain interactions                                          |                             |
| `WALLET_KEY`  | The private key to a wallet you want to use for trading. Obviously sensitive so please handle with care. |

## SDK Config
The config.py file has some basic SDK settings such as the network/chain you want to use (kovan or mainnet only) and whether spend allowances should be automatically adjusted when submitting orders.

## TWAP Example
The twap.py script is just an example. There are many other policy configurations that you can create to build up your own trading strategy/algorithm. 
