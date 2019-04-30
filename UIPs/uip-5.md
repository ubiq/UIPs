---
uip: 5
title: Escher to become an Escher Hub on the Cosmos Network with ESCH as the native staking token
author: Julian Yap
status: Draft
created: 2018-04-30
---

## Simple Summary

The following is a proposal for Escher (ESCH) to transition from an UBQ token to the base unit and native staking token of an Escher Hub on the Cosmos Network. This will retain Escher governance functionality as well as provide Ubiq with the benefits of running a  Hub on the Comos Network, enabling technologies such as Inter-Blockchain Communications (IBC).

From the outset, Escher was built as the governance token of the Ubiq network which fuels and directs proposals (development and otherwise). It was always envisioned that Escher would also provide additional utility to the Ubiq ecosystem.

## Motivation

Ubiq is an independent blockchain network with its own mining network, mining algorithm, monetary policy, tokens and ecosystem.

Ubiq (UBQ) will retain its primary use as being used as gas, smart contracts, tokens and dApps.

Escher (ESCH) will retain its governance aspects but will also be given added utility such as staking and gas.

In this vision, the Ubiq blockchain and Escher Hub will not compete with each other but form a symbiotic relationship.

Ubiq blockchain:
* Proof of Work chain
* 88 second block time suitable for mining and running a full node on a single-board computer

Escher Hub:
* Tendermint Core-based Proof of Stake
* Faster block times (the main Cosmos Hub with base units ATOM has 6 second block times)

As an Escher Hub will enable Inter-Blockchain Communications (UBQ and UBQ tokens can freely flow between chains), this will enable complementary technologies to the Ubiq ecosystem.

Some of the added benefits of a Tendermint Core chain compared to an Ethereum EVM compatible chain include:
* Finality. Tendermint chains are considered to have 1-block finality.
* Faster and more predictable block times.
* Gateway for UBQ and UBQ tokens to other Cosmos Network Hubs. Allows transfers to a Cosmos DEX.
* Alternative dApp model targeting the Cosmos SDK.
* Governance functionality built-in.

## Specification and Implementation

The Ubiq community will test and implement an Escher Hub on the Cosmos Network with ESCH as the base unit and staking token.

An associated Peg-Zone will be tested and implemented to allow the flow of UBQ and UBQ tokens between the Ubiq blockchain and the Escher Hub blockchain.

Ubiq Smart Contract Platform <> Peg-Zone <> Escher Hub

Further technical specifications such as rate of inflation, block times, maximum number of validators will be drawn up once community testing is complete.

## References

Understanding the Escher Token system https://blog.ubiqsmart.com/understanding-the-escher-token-system-80dcae231324

What is Cosmos? https://cosmos.network/intro


