# Composable Stable Pools

## Overview

Composable Stable Pools are designed for assets that are either expected to consistently trade at near parity, or at a known exchange rate. Composable Stable Pools use [Stable Math](../../concepts/math/stable-math.md) (based on StableSwap, popularized by Curve) which allows for trades of significant size before encountering substantial price impact, vastly increasing capital efficiency for like-kind and correlated-kind swaps.

### Ideal For

* **Pegged Tokens** - tokens that trade near 1:1, such as two stablecoins of the same currency (eg: DAI, USDC, USDT), or synthetic assets (eg: renBTC, sBTC, WBTC)
* **Correlated Tokens** - tokens that trade near 1:$$R$$ with some slowly changing exchange rate $$R$$, like derivatives (eg: wstETH, wETH)

### Stable Swaps Under the Holdr Umbrella

One of the key advantages to having Composable Stable Pools on Holdr specifically is that they are plugged into the same protocol as all other pools. Swapping between stablecoins is frequently used for arbitrage when one token is paired with two different stablecoins in different pools. By leveraging Batch Swaps on Holdr, these trades can be combined into a single, gas-efficient transaction.

## What Does Composable Mean?

A pool is **composable** when it allows swaps to and from its own LP token. Putting its LP token into other pools (or "nesting") allows easy Batch Swaps from nested pool tokens to tokens in the outer pool.

#### Example

With `ComposableStablePool[DAI, USDC, USDT]`, we can directly pair the LP token, or BPT, against WETH in a `WeightedPool[WETH, CSP-BPT]`. This nesting allows us to consolidate liquidity into some of the most common groupings, which results in deeper liquidity and better prices throughout Holdr. In this example, it also saves you the trouble of making 3 WeightedPools `[WETH, DAI]`, `[WETH, USDC]`, `[WETH, USDT]`.

### Pre-minting

These pools mint an effectively infinite amount of their LP tokens at the time of pool creation. This help reduce gas costs because instead of using the mint/burn mechanism to join a pool, it uses a transfer on a join/exit, which is more efficient.

## Predecessors

**Composable Stable Pools** are a **superset of all previous Stable-type pools** (Stable Pools, MetaStable Pools, StablePhantom Pools, and StablePool v2) and therefore obsolete all previous pools.
