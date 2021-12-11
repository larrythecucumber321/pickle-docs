# pJar 0.88 (Inactive)

### **What is pJar 0.88?**

We're going back to basics with pJar 0.88, allowing users to deposit base-currencies such as DAI, USDT, USDC, etc. The first pJar 0.88a will support **DAI**, and will be launched with a **leveraged** **COMP** mining [strategy](https://etherscan.io/address/0xCd892a97951d46615484359355e3Ed88131f829D)**.**

Using the deposited base-currency tokens, pJar 0.88 receives and re-invests COMP for you so you end up having more of the underlying base currency.

### How does leveraging COMP mining work?

Leveraging mining COMP is achieved by recursively supplying and borrowing a single asset. Note that the act of supplying or borrowing assets on compound will yield us COMP tokens.

For example, if DAI has a collateral factor of 0.75, and we have supplied 100 DAI, we can borrow out a maximum of 75 DAI. We can resupply our borrowed 75 DAI, giving us a total of 175 supplied DAI and 75 borrowed DAI. We can now borrow an additional 56.25 DAI (175 \* 0.75 - 75) and resupply it. We can keep repeating this supply and borrow loop until we hit a certain threshold.

The formula for calculating the maximum amount of leverage we can achieve is

$$
1 + (1 * 0.75) + (1 * 0.75^2) + (1 * 0.75^3) + .... + (1 * 0.75^n)
$$

Which can be expressed as an infinite geometric series:

$$
Max\ Leverage = \frac{a_1}{1-r} = \frac{1}{1-0.75} =4
$$

However, **leverage mining COMP at max leverage is** **incredibly dangerous** due **** to the difference in the supply/borrow interest rates. As such, the strategies launched will be employing an initial safety buffer of 0.10 collateral factor. Meaning the maximum safe leverage will be rougly 2.86.

$$
Safe \ Max\ Leverage = \frac{1}{1-0.65} = 2.85714286
$$

####
