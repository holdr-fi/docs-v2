# veHLDR and Gauges

{% hint style="warning" %}
<mark style="color:orange;">**veHLDR and Gauges are not yet live for Hodlr**</mark>
{% endhint %}

The veHLDR and Gauge system is designed to promote long-term token-holder alignment, decentralize Liquidity Mining allocation, and facilitate fair protocol revenue distribution. This system is based heavily on Curve's veCRV system.

## veHLDR Overview

veHLDR (vote-escrow HLDR) is a vesting and yield system based on [Curve’s veCRV mechanism](https://curve.readthedocs.io/dao-vecrv.html) which locks 80/20 wNEAR/HLDR Holdr Pool Tokens for a maximum of 1 year.

{% content-ref url="vebal/" %}
[vebal](vebal/)
{% endcontent-ref %}

## Gauges Overview

Gauges are a class of contracts that determine how Liquidity Mining (LM) is allocated.

There are a few Gauge Types to handle a few scenarios; some Gauge Types require voting with veBAL to give specific Gauges a higher weighting, while others are fixed-amount distribution channels. These per-Gauge-Type amounts can be changed by Governance vote.

**Examples**

* Voting with veBAL: Allocating LM to specific Ethereum mainnet pools
* Fixed-Amount: Amounts designated for the LM Committee to allocate as they see fit

{% content-ref url="gauges/" %}
[gauges](gauges/)
{% endcontent-ref %}
