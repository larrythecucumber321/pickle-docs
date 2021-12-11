---
description: Earn additional PICKLE rewards
---

# What are Pickle Farms?

The Pickle Finance Farms are located here: [https://app.pickle.finance/farms](https://app.pickle.finance/farms)

The Farms allows users to to farm PICKLE token rewards based on staking various assets.&#x20;

![](<../../.gitbook/assets/image (17).png>)

Each of these farms require a different token to be staked.&#x20;

The first of these farming pools, the **Pickle Power** pool, requires staking Uniswap **PICKLE/ETH LP tokens** (guide [here](powerpool.md)).

The rest of the farming pools require staking pTokens obtained from depositing in a **Pickle Jar** (guide [here](lock-pickles/pickle-jars.md)).&#x20;

### Displayed Returns

The APY that is displayed for each farming pool represents the combination of ALL the different yields you would get. This includes returns from PICKLE rewards, PickleJar returns, Uniswap or Sushiswap LP fees, etc. Hovering over the APY number will show you the breakdown.

![Hover over the APY to see the breakdown](<../../.gitbook/assets/image (18).png>)

### PICKLE APR

The APR (annual percentage rate) of the PICKLE component of each of the farms depends on a number of factors:

* The **velocity** **(tokens/block)** at which PICKLEs are accruing to that particular Farm.  This in turn the result of the PICKLE emission rate (`picklePerBlock`) _times_ the relative weight of the Farm. For example, if `picklePerBlock` is 0.10 and the Farm's `weight` is 0.10 then the Farm as a whole is receiving 0.01 PICKLEs every Ethereum block.&#x20;
  * All things equal, the higher the `weight` , the higher the PICKLE APR.
* The **number of pTokens currently staked** on the Farm. For example, if the Farm is receiving 0.01 PICKLEs / block, and there are 10,000 pTokens staked on the Farm this block, each pToken receives 0.000001 PICKLEs / block.
  * All things equal, the lower the number of pTokens, the higher the PICKLE APR.
* The price of PICKLE and the price of the pToken (based on the price of the underlying assets). Since yield is a function of both principal (your pToken deposit) and returns (the PICKLE rewards), both affect the resulting APR.
  * All things equal, the higher the PICKLE price, the higher the APR.
  * All things equal, the higher the value of the pTokens, the lower the APR.
* The user's DILL boost factor, as explained [here](boost.md).

The Pickle app calculates a PICKLE APR based on real-time conditions for each Farm. This **display APR** is unstable, as conditions may change, sometimes rather quickly.&#x20;
