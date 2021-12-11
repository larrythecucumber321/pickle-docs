# Jars and Farms Walkthrough

## Jars and Farms Walkthrough <a href="#docs-internal-guid-d3d04a56-7fff-e457-9259-a74112081285" id="docs-internal-guid-d3d04a56-7fff-e457-9259-a74112081285"></a>

Below are walkthroughs for joining Pickle Jars and Farms.&#x20;

### Navigating the Jars page

![](https://lh4.googleusercontent.com/nl9W2aEzdY3wxlhtGGpPyXYswMI-krQ\_OUho319QmWrjvVjygVA1NKzSfJmoaPRwLZ4OBFXqq-PQZ3FXqdCcp3xbWOmfxOg\_5-CyVtbXt\_48QUyM2Crtnl5quFCQ8nbsf-1ACX5N)

**Jars page**

Jars, sometimes called vaults, are basically pools of funds with an associated strategy for maximizing returns on the asset. When a user puts his LP tokens into the jar, they will receive a pickle receipt for that specific LP which can be claimed at a later date along with the accrued earnings. The strategy involves selling specific reward tokens in order to reinvest into the LP.. You can check manually how much you have earned by following a guide written by a community member: [Vertex’s guide](https://vertex7.medium.com/how-to-calculate-pickle-finance-farm-profit-9c5648a57141).

For example, ALCX/ETH jars will claim the reward tokens (in this case, ALCX & Sushi tokens) and re-invest both tokens to buy more ALCX-ETH LP tokens, increasing and compounding your original investment. Specifically, all Sushi and some ALCX will be sold for ETH and more LP tokens will be purchased.&#x20;

\
Example of reinvestment

![](https://lh5.googleusercontent.com/4BsJIkgq1sA1s8qyPN\_OVso8CW54OuuJfRGXX1ytBW3R5aQEVhRTVt7VFgzTkYMyV5GYjmUxJ9SV71Y6XfcaW3uOZ9XvlpRzDbhHylz3RbkdAVEOISqA\_uMzOzkTiCUTcOIyuUwc)

When depositing, users will have to approve 2 transactions, one to approve the Pickle Finance site as an approved user of your tokens, and the other to actually deposit those tokens into a jar. Once a user has deposited into the jar, that's it! The compounding (selling the specific rewards) is automatic. Some jar strategies will compound daily, while others may have to wait a few days to be compounded due to low balances, high gas costs, or lower APY. .

On the Jar page, if you hover over the displayed APY %, you can see the breakdown of where your yield comes from. The tooltip will show you the base APR, and how much comes from each of the reward tokens.&#x20;



### Navigating the Farm Page

![](https://lh3.googleusercontent.com/srcHiIwD2AsTVllRRH9PyuVstwY4M7iWfsqiuXco4CuaB9mGk6q6kqGZb7R6hfvRDDlCw3iprzO7pbvevh8jWzDS7FW8d0dHcJFNd6Ud7AyiF\_-M2GIl9ltMNbfQeXk5Ji-igE-h)

**Farm page**

Farms, sometimes called gauges, involve staking your Pickle Jar tokens in the platform in order to earn a share of PICKLE token emissions.&#x20;

The farm page contains a lot of numbers and it may get confusing. Let's look at the ALCX/ETH jar as an example.

**pSLP ALCX/ETH** is the name of the strategy, it stands for pickled Sushiswap Liquidity Provider for Alchemix and Ether.

**APY Range**: 640.69%-644.37% is the amount you will get in a year if all things are constant. The range is based on the pickle reward, which can be boosted up to 2.5x by locking DILL.

**Your APY**: 644.37% is the APY you get in this strategy. This number takes your boost into account to come up with your personal yield.&#x20;

**Earned**: 0.281 is the PICKLE token reward you have already earned by staking in the Farm. You may claim these at any time, but it’s often a good idea to wait until you have earned enough to justify the gas cost of claiming these rewards.

**Balance**: 0 is the amount you can stake in the farm. In this example, the value is 0 because the user has already staked all of the ALCX-ETH LP Pickle Jar tokens that he had. He has none left to put into the Farm. If you have not deposited any of your Pickle Jar tokens into the Farm yet, the number of pJar tokens you own will be shown here. These would be eligible to be deposited.&#x20;

**Staked**: 0.52505... This figure represents how many Pickle Jar tokens you have already staked into the Farm. This unit for this number is pJar tokens.&#x20;

**Value Staked**: $2,675.52 This figure represents the US Dollar value of your underlying assets. As your LP grows from compounding the rewards, so will this figure. It may also decrease if the underlying value of the LP (and thus, the two tokens in the LP, namely ALCX and ETH) have fallen.

**Approve And Stake**: This button will prompt you to approve Pickle Finance to access your pJar tokens, and then stake them into the farm.

**Unstake**: This button will let you take some or all of your pJar tokens out of the farm and back into your wallet. To actually get your money, though, you’d still need to withdraw from the Jar itself, and then go withdraw from the Liquidity Pool on Sushiswap. Then, you’ll have the cash you need to bring your family out for a sushi dinner. This action will not claim earned pickle.

**Harvest**: Claim your earned pickle token for snacks.

**Harvest and exit**: You’ve gotten rich and finally want to leave us. That’s ok. We’ll miss you. This action will withdraw your pJar tokens from the Farm \*and\* claim your earned PICKLE token rewards. After you withdraw from the jar and from Sushi, you can go buy a boat (and you’ve got PICKLE snacks for your boat ride, too!)

For an in-depth profit page, you can visit the [profit page](https://app.pickle.finance/info/earn).
