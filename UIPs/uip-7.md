---
uip: 7
title: Permanently disable Escher minting
author: Luke Williams
status: Draft
created: 2019-05-30
---

## Simple Summary

With the original 8 planned airdrops drawing to an end, it's time to evaluate how to move forward with the Escher (ESCH) token. Continue as originally planned, or..?

## Motivation

Due to the nature of the airdrop schedule, the Escher ERC20 token was deployed with an owner address that has escalated permissions within the contract allowing it to:

* mint escher (this is used for the airdrops)
* transfer ownership to a different address
* permanently disable minting (this can only be called once, there is no re-enable)

The address that currently has this ownership role is: `0xda904bc07fd95e39661941b3f6daded1b8a38c71`

This proposal is to continue with the original plan, permanently disable minting. This locks the total supply in at 450,454,965.391453439756557953 ESCH, while also removing any meaningful functionality the ownership role has.

## Implementation

If passed (disable), address `0xda904bc07fd95e39661941b3f6daded1b8a38c71` will call the [finishMinting](https://github.com/ubiq/escher-contracts/blob/master/token/ERC20/Escher.sol#L42) function within the Escher ERC20 contract (`0xcf3222b7FDa7a7563b9E1E6C966Bead04AC23c36`), permanently disabling minting.

If rejected (keep enabled), a second UIP will be submitted to determine how to manage the ownership role/keys.

## References

Escher token contract: https://github.com/ubiq/escher-contracts/blob/master/token/ERC20/Escher.sol

About Escher: https://blog.ubiqsmart.com/understanding-the-escher-token-system-80dcae231324

Escher Airdrops: https://ubiqsmart.com/escher/airdrops/historic
