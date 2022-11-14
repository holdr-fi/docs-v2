# Weighted Pools

## Overview

Weighted Pools are highly versatile and configurable pools. Weighted Pools use [Weighted Math](../../concepts/math/weighted-math.md), which makes them great for general cases, including tokens that don't necessarily have any price correlation (ex. DAI/WETH). Unlike pools in other DeFi protocols that only provide 50/50 weightings, Holdr Weighted Pools enable users to build pools with different token counts and weightings, such as pools with 80/20 or 60/20/20 weightings.

![](https://lh5.googleusercontent.com/0GwiW7l34zVaJGBEHl3UATWh1U4IrzUjeYOzdCA4aUuAZWbaAnv8o6AF7CuLbkIuUAEX\_NpbLCYdChkgTb17x28Ra1M6xqqnhuAj4Uo4ZpBnwWPfEloTu6xS\_ujMznZJFWpYp5sD=s0)

## Advantages

### Exposure Control

Weighted Pools allow users to choose their levels of exposure to certain assets while still maintaining the ability to provide liquidity. The higher a token's weight in a pool, the less impermanent loss it will experience in the event of a price surge.

For example if a user wants to provide liquidity for WBTC and WETH, they can choose the weight that most aligns with their strategy. A pool more heavily favoring WBTC implies they expect bigger gains for WBTC, while a pool more heavily favoring WETH implies bigger gains for WETH. An evenly balanced pool is a good choice for assets that are expected to remain proportional in value in the long run.

![Variable pool weight allows for fine-tuned exposure to assets](https://lh4.googleusercontent.com/VwAkBtoNQLfuRFb3Wmb6YdEJwFyyR2WNXcEAkZGgJ7teCaYHeFK-ZEwC7kLYPiTdFWSjjRQA2y550pFkMqimjS5CZW2IKQ6A-RNPKzG27Ja2xK\_efAZkU63ZC5vq29EyCUaEVDzo=s0)

#### Impermanent Loss

Impermanent Loss is the difference in value between holding a set of assets and providing liquidity for those same assets.

Some people find the word "Impermanent" misleading and prefer to call it "Divergence Loss" or "Rebalancing Loss" because one token may perpetually out-value another token, and the loss may become... permanent.

For pools that heavily weight one token over another, there is far less impermanent loss, but this doesn't come for free; very asymmetric pools do have higher slippage when making trades due to the fact that one side has much less liquidity. 80/20 pools have emerged as a happy medium when balancing liquidity an Impermanent Loss mitigation.

![](../../.gitbook/assets/1\_riTMWg3dE3ewaL3A3Hko\_Q@2x.png)

### Trading Pairs

Since each token in a pool can be traded with any other token in a pool, the number of trading pairs grows significantly with each additional token. By providing more trading pairs, pools are able to facilitate more swaps, giving them more opportunities to collect fees.

The number of trading pairs in a pool follows the combinations equation $$_nC_r = \frac{n!}{r!(n-r)!}$$. Where $$n$$​ is 2 and $$r$$​is the number of tokens in the pool.

![](<../../.gitbook/assets/Screen Shot 2021-10-08 at 2.16.03 PM.png>)
