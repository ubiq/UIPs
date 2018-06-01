---
uip: 1
title: Independent Proof-of-Work algorithm
author: Julian Yap
status: Draft
created: 2018-05-30
---

## Simple Summary

The following is a proposal for an independent proof-of-work algorithm for Ubiq. Sharing a proof-of-work algorithm with the larger Ethereum network opens us up to potential mining rig rental attacks. 

## Motivation

Ubiq is an independent blockchain network with its own mining network, monetary policy, tokens and ecosystem. Ubiq is the first and only Ethereum fork to have a modified proof-of-work difficulty algorithm enabling 88 second block times. Having its own independent proof-of-work algorithm is a further extension of this philosophy.

Changing the proof-of-work algorithm will also allow for increased independence in market fluctuations as this will eliminate short term Ethash profit switching orientated miners from entering the mining network.

## Specification

Ubiq will test and implement a new proof-of-work algorithm. A hard fork block will be announced.

The new proof-of-work algorithm will either be ProgPow (described in EIP-1057) or preferably a minor change in the current Ethash that will allow for easy adoption.

## Implementation

To reduce any possible risks the preference is towards changing the Keccak-256 and Keccak-512 algorithms used in Ethash with other standardized and secure hashing algorithms.

Testing and implementation involves:

1. Test the client works with the new Ethash.
2. Implement and test a hard fork from Ethash to new Ethash.
3. Fork some more GPU miner repositories to implement new Ethash and test.

Also get some hashing and verification benchmark numbers along the way.

## Backwards Compatibility

Any adopted algorithm would not be backwards compatible with the existing Ethash and will require a hard fork for adoption.

Depending on the algorithm adopted, factors such as network hashrate would proportionally change.

## References

Ethash https://github.com/ethereum/wiki/wiki/Ethash

EIP-1057 https://github.com/ethereum/EIPs/blob/master/EIPS/eip-1057.md


