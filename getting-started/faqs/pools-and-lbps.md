# Pools and LBPs

## What kind of pools exist of Holdr?

Holdr enables customizable AMM logic by creating a launchpad for teams to innovate with different AMM strategies. This means if you want to launch a new style of trading pool, you can focus on the high-level concepts without having to worry about low-level token transfers, balance accounting, security checks and order routing. With Holdr, this all comes out of the box.

Some existing pool types are:

* **Weighted Pools** - 8-token pools with custom weighting
* **Stable Pools** - Pools with 2-5 tokens that use a StableSwap equation, and contain tokens of similar value. For example, DAI/USDC/USDT, and WBTC/renBTC/sBTC
* **Liquidity Bootstrapping Pool** - A 2-4 token pool with the ability to enable and disable trading, and change weights. Only the creator can add liquidity.

## Can I have nested pools?

Yes, you can create Holdr pools of Holdr pools. This can fill the need of products that want to aggregate across many different products — imagine a project which tokenizes real estate and has separate Holdr pools for each city — a composed version of that pool could represent a whole state.

## What is an LBP?

For V1 LBPs, see [this FAQ](https://docs.balancer.fi/v/v1/smart-contracts/smart-pools/liquidity-bootstrapping-faq).\
\
It is a smart pool that dynamically changes the token weighting (e.g 1%/99% ETH/$TOKEN to 99%/1% ETH/$TOKEN), allowing founders to create a liquidity bootstrapping pool with minimal capital requirements. The result is that the token price continually experiences downward pressure throughout the sale. When this is mixed with modest buying demand, the price stays stable throughout the sale, as whales/bots are disincentivized to buy it all at once. PrimeDAO is building the IDO Launchpad, which will streamline the process for a smoother experience. Other partners are building UIs as well.

## How long do LBPs last?

LBPs can live as long as the creators decide they should. In general, pool creators tend to run them for less than 2 weeks.

## How does the pricing in LBP work?

At the creation of an LBP the team should set up a price that is significantly higher than what they think is a market price. After the launch, the token price continually experiences downward pressure throughout the sale, until it reaches the right market price. When this is mixed with modest buying demand, the price stays stable throughout the sale, as whales/bots are disincentivized to buy it all at once.

## Should I join an LBP as soon as it launches?

No, this is not the point. Prices are _supposed_ to start intentionally high and then come down. If you join early may end up paying way more than if you wait for the price to stabilize.
