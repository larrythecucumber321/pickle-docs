---
description: >-
  A description of the different strategies employed by Pickle Finance's
  PickleJars.
---

# Pickle Jar Strategies

## Introduction

Each PickleJar employs a Strategy contract to earn yield for its depositors. In this document, we explore the types of Strategies being employed and how these work under the hood.

The PickleJar system is largely based on Yearn's [yVault](https://yearn.finance/vaults) system, and therefore the most relevant function is the `harvest()` function, which is what executes the profit-generating steps.

All Strategy contracts are being developed under the [`src/strategies`](https://github.com/pickle-finance/protocol/tree/master/src/strategies) directory of the [protocol](https://github.com/pickle-finance/protocol) repository. For a listing of all currently deployed Strategy contracts, see the [contracts](https://github.com/pickle-finance/contracts#pickle-jars-pjars) repo.

All pickle jars have 20% performance fee except Sushi jars (Excluding USDT/MIC & USDT/MIS). The displayed APY % is the net APY after the fees.

![](<../../.gitbook/assets/image (24).png>)

## CRV-based Strategies

These Strategies are based on farming CRV tokens, and then selling them for more of the deposit tokens (usually Curve LP tokens).

### Steps

In broad strokes, this is what the CRV-based Strategies do:

1. Farmed CRV tokens are collected and converted to the stablecoin offering the most premium.
2. A portion of the farmed CRV may be locked up as veCRV for future voting and boosting
3. The stablecoin from Step 1 is then supplied back into the Curve pool to get more of the PickleJar's deposit token (i.e. Curve LP tokens).

The reason for the focus on converting to the most premium stablecoin is because Curve gives a bonus for providing the most premium stablecoin to its pools.

**Note:** The sCRV Strategy has an additional step to collect farmed SNX and convert that to the most premium stablecoin.

### Reference

The relevant Strategy contracts are located in the `src/strategies/curve` [directory](https://github.com/pickle-finance/protocol/tree/master/src/strategies/curve). All CRV-based Strategies begin with `StrategyCurve` and you may reference this [README](https://github.com/pickle-finance/contracts#pickle-jars-pjars) to see which PickleJars are using this Strategy.

{% content-ref url="pjar-0.md" %}
[pjar-0.md](pjar-0.md)
{% endcontent-ref %}

## UNI-based Strategies (Inactive)

These Strategies are based on farming UNI tokens, and then selling them for more of the deposit tokens (usually Uniswap v2 LP tokens).

### Steps

In broad strokes, this is what the UNI-based Strategies do:

1. Farmed UNI tokens are collected.
2. A portion of the farmed UNI may be locked up for future voting and boosting
3. The remaining UNI is sold for WETH.
4. Half of this WETH is sold for the other token in the Uniswap pair. For example, this would be DAI for the DAI/WETH pair.
5. Supply both tokens into Uniswap for more of the deposit token (aka LP token).
6. Stake the additional deposit token to earn even more UNI.

**Note:** Extra dust is donated to the Pickle Finance community-controlled Treasury.

### Reference

The relevant Strategy contracts are located in the `src/strategies/uniswap` [directory](https://github.com/pickle-finance/protocol/tree/master/src/strategies/uniswapv2). All UNI-based Strategies begin with `StrategyUni` and you may reference this [README](https://github.com/pickle-finance/contracts#pickle-jars-pjars) to see which PickleJars are using this Strategy.

{% content-ref url="pjar-0.69.md" %}
[pjar-0.69.md](pjar-0.69.md)
{% endcontent-ref %}

## COMP-based Strategies (Inactive)

We're going back to basics with pJar 0.88, allowing users to deposit base-currencies such as DAI, USDT, USDC etc. The first pJar 0.88a supports **DAI**, and utilizes a **leveraged** **COMP** mining [strategy](https://etherscan.io/address/0xCd892a97951d46615484359355e3Ed88131f829D)**.**

{% content-ref url="pjar-0.88.md" %}
[pjar-0.88.md](pjar-0.88.md)
{% endcontent-ref %}

## SUSHI-based Strategies

These Strategies are based on farming SUSHI tokens, and then selling them for more of the deposit tokens (usually Sushiswap v2 LP tokens). The SUSHI 23.33% shown in the pJars are the 1/3 that is claimable instantly. The remaining 2/3 vested tokens are still in discussion on how they are to be used. Instead, there are no performance fee for these SUSHI-based strategies!

![](<../../.gitbook/assets/image (24).png>)

### Steps

In broad strokes, this is what the SUSHI-based Strategies do:

1. Farmed SUSHI tokens are collected.
2. The SUSHI token is sold for WETH.
3. Half of this WETH is sold for the other token in the Sushiswap pair. For example, this would be DAI for the DAI/WETH pair.
4. Supply both tokens into SUSHIswap for more of the deposit token (aka LP token).
5. Stake the additional deposit token to earn even more SUSHI.

### Reference

The relevant Strategy contracts are located in the `src/strategies/sushiswap` [directory](https://github.com/pickle-finance/protocol/tree/master/src/strategies/sushiswap). All SUSHI-based Strategies begin with `StrategySushi` and you may reference this [README](https://github.com/pickle-finance/contracts#pickle-jars-pjars) to see which PickleJars are using this Strategy.
