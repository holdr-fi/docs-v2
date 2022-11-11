# How Gauges Work

## Voting

Liquidity Mining emissions are distributed among different Gauges according to veHLDR voting. **All veHLDR voting happens on Aurora.** veHLDR holders can vote for one or more Gauges, choosing the percentage of their voting power to allocate to a specific Gauge.

## Staking

Each pool eligible for Liquidity Mining has a Gauge contract associated with it. In order for Liquidity Providers to be eligible for Liquidity Mining, they must stake their Holdr Pool Tokens (HLDRs) in the pool's corresponding Gauge.

## Multi-Token Liquidity Mining

Each pool's Gauge contract can distribute up to 8 different kinds of tokens. This allows for multiple partners/protocols/DAOs to incentivize a given pool by adding their own tokens.

In order to prevent spam tokens from occupying those 8 slots and blocking out legitimate tokens, Holdr Governance has the power to allow addresses to be able to add tokens to a Gauge using the Authorizer.

## Dividing a pool's LM among LPs

To be eligible for a given pool's HLDR emissions, a user must stake their corresponding LP tokens to that pool's gauge. Their share of the HLDR emission scales with their proportional stake of LP tokens for that pool.

#### Additional veHLDR Boost

On Aurora, a user's claimable HLDR also depends on their amount of veHLDR. This extra boost is determined just as [Curve's CRV boost is calculated](https://curve.readthedocs.io/dao-gauges.html#boosting).
