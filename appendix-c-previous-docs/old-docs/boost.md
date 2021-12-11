---
description: Earn PICKLE by pickling your ptokens in the Farms.
---

# Boosted Rewards

## Boosting

One of the main incentives for DILL is the ability to boost your PICKLE rewards on our Pickle Farms ([https://app.pickle.finance/farms](https://app.pickle.finance/farms)). Depositors are able to earn a **max boost of up to 2.5x**.&#x20;

The following considerations govern how much of a boost you obtain:

* Your proportional **share of the total DILL supply**
  * If you own a larger share of the total supply, you will obtain a larger boost.
* Your proportional **share of a particular Farm**&#x20;
  * If your deposit in a particular Farm is small relative to the total deposits, it will be easier for you to obtain the max boost. The opposite is true if you comprise a large share of the deposits in a Farm (i.e. more DILL is needed for max boost).
  * e.g. if the total deposits in a Farm is $100,000 a smaller DILL balance is required to obtain the max boost if your deposit size was $1,000 compared to if your deposit size was $20,000.

In summary, your DILL balance applies to all Farms equally but may produce different boosts of up to 2.5x based on your share of deposits in the Farm.

$$
DerivedBalance = UserBalanceInFarm * 0.4
$$

$$
AdjustedBalance = \frac{TotalDepositedInFarm * UserDillBalance}{DillTotalSupply} *0.6
$$

$$
BoostFactor = \frac{min(DerivedBalance +AdjustedBalance, UserBalanceInFarm)}{UserBalanceInFarm}
$$

A calculator is provided here to estimate how much DILL is required for obtaining certain boosts given the specific conditions of each of the Farms [http://app.pickle.finance/dill](http://app.pickle.finance/dill).&#x20;

### Reward Range

You may notice that each Farm displays an APR _range_. Which APR, within the range, you will receive works as follows:

* If you have no DILL balance, you will receive the APR at the lower end of the range. This is the **base APR** that all unboosted users receive.
* If you hold DILL, you will receive a **boosted APR**. Your current boost can be checked with the calculator [here](http://app.pickle.finance/dill).
* The higher end of the range displayed on each Farm shows the APR with the 2.5x boost.&#x20;
* Once you stake your pTokens in the Farm, your exact APR will be displayed next to the APR range on the "my APR" indicator.

![](<../../.gitbook/assets/image (31).png>)

####
