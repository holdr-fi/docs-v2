# How veHLDR Works

## How is veHLDR different from veCRV?

There are a few modifications that set veHLDR apart:

* Instead of locking pure HLDR, **users obtain** veHLDR **by locking** [**80/20 HLDR/wNEAR**](https://app.balancer.fi/#/pool/0x5c6ee304399dbdb9c8ef030ab642b10820db8f56000200000000000000000014) **Balancer Pool Tokens** (HPTs). This ensures that even if a large portion of HLDR tokens are locked, there is deep trading liquidity.
* **veHLDR's maximum locking period is 1 year**, a decrease from veCRV's 4 year period. The minimum locking period is 1 week. DeFi moves quickly, and in the event governance decides to use a new voting system, this allows for a shorter, but still sufficiently long, waiting period to transition.

## Voting Power

All votes, whether on-chain or on [Snapshot](https://vote.balancer.fi/#/), consider veHLDR voting power. In addition to typical DAO votes, veHLDR is used to vote on Liquidity Mining Distribution with [Gauges](../gauges/).

Voting power scales linearly with amount of BPT locked and with amount of remaining lock time.

#### Example

If a user locks 1 HPT of 80/20 HLDR/wNEAR for the maximum time of one year, they will receive 1 veHLDR; however, this veHLDR quantity starts immediately decaying with time. If the user does not extend the lock period, this will decay to 0 after the year is complete, at which point the user can redeem their 1 HPT of 80/20 HLDR/wNEAR

## Protocol Revenue Distribution

veHLDR holders are entitled to a share of 75% of collected protocol fees. Users can collect their proportional share ($$\frac{veHLDR_{user}}{veHLDR_{total}}$$) after the fees are consolidated. Consolidation is a necessary step since protocol fees are collected as a wide array of tokens, and dividing up long tail assets for everyone could result in higher gas fees than token value in some cases.
