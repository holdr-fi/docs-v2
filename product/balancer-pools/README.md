---
cover: ../../.gitbook/assets/bannerPools (1).png
coverY: 0
---

# Pools

## Overview

Pools are the fundamental building blocks of the Holdr Protocol; they are smart contracts that define how traders can swap between tokens on Holdr. What makes Holdr Pools unique from those of other protocols is their limitless flexibility. While other exchanges have pools with constrained parameters, Holdr can accommodate pools of any composition and underlying math. Holdr's architecture allows for anyone to develop their own pool type, opening the door for customized pricing functions in trading pools.

## Pools At A Glance

### [Weighted Pools](weighted-pools.md)

Designed for general cases, including tokens that don't necessarily have price correlation (ex. DAI/WETH).

### [Stable Pools](broken-reference)

Ideal for soft-pegged tokens with strong correlation (ex. DAI/USDC/USDT).

### [Liquidity Bootstrapping Pools](liquidity-bootstrapping-pools-lbps.md)

Ideal for shifting liquidity of one token into another (ex. AKITA/ETH).

## Comparison

| Pool                        |     Math | Max # Tokens | Uses Oracle | Can _Be_ Oracle | Time-dependent pricing |
| --------------------------- | -------: | -----------: | ----------: | --------------: | ---------------------: |
| **Weighted**                | Weighted |            8 |          No |             Yes |                     No |
| **Stable**                  |   Stable |            5 |          No |              No |                     No |
| **Liquidity Bootstrapping** | Weighted |            4 |          No |              No |                    Yes |
