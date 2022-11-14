# Liquidity Mining with the veHLDR and Gauge System

## How does liquidity mining in the Gauge system work?

You can see which pools receive liquidity mining incentives by the 3 star icon next to the pool position on [https://app.holdr.fi/#/](https://app.holdr.fi/#/) :

![Example of a gauge receiving BAL incentives as well as other incentives as well as swap fees indicated on the tooltip when hovering over the 3 star symbol](<../../.gitbook/assets/image (1).png>)

## What does Min. HLDR and Max. HLDR APR mean?

{% hint style="info" %}
All APRs are extrapolated estimates based on recent data; they are not guaranteed.
{% endhint %}

Holdr has a boosting system which allows veHLDR holders to increase their liquidity mining distributions on mainnet pools based on their locked veHLDR and locked liquidity position.

* The Min. APR is the minimal APR a user can expect when staking any amount of liquidity in a gauge while not holding any veHLDR
* The Max. APR is the max. theoretically achievable APR of 2.5x the Min. APR.

If you want to better understand the relationship between the Min. and Max. APR boost and your liquidity position relative to your veHLDR holdings, we recommend to consult the [community boosting calculator](https://balancer.tools/boost).

## How are incentives directed to the Gauges?

The flow of incentives are now fully controlled by veHLDR holders. Following rules apply

* A pool may receive liquidity mining only if it is eligible for voting. To be eligible to vote, a pool has to be allowlisted through a community proposal and vote
* Incentives for the running week have been voted upon on the previous week
* Voting epochs last between Thu-Thu 00:00 UTC.

## What do I have to be aware of when voting?

The voting system enables full control over how incentives are distributed; however, not all mechanisms are directly clear to the user. Please be aware of following mechanisms when voting:

* Voting involves a 10 day cool-down period
  * Changing a vote on a certain gauge also imposes a 10 day cooldown on that gauge
* If you increase your veHLDR position, **make sure to revote** to fully register your newly acquired veHLDR
