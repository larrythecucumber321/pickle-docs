# Farm APR Explained

### Farm APR  <a href="#docs-internal-guid-dbde2362-7fff-4839-f137-83732064cafb" id="docs-internal-guid-dbde2362-7fff-4839-f137-83732064cafb"></a>

While relatively simple, the calculation to determine how much pickle emissions you are entitled to is not entirely trivial. It can be broken down into a few steps. It is important to realize that the Pickle app calculates a PICKLE APR based on real-time conditions for each Farm. This display APR is unstable, as conditions may change, sometimes rather quickly.



#### What are the current emissions?

The first step is determining what the total emissions are. This is known as the picklePerBlock and can be queried from the PICKLE token contract. The current emissions are 0.3 pickles per block. 0.2 pickles per block for Ethereum network, and 0.1 pickles per block for polygon network.

Hovering over the Total Supply will show you the current emissions. This emissions schedule is to last until 31 December 2021, and to be decided by DILL holders on the next emissions.\


![](https://lh5.googleusercontent.com/n5M4wgDw9KApYrhAzbDQKfVyTmimSD5CROjJ5J\_KuOFuB8uwKCUDwvaa4cDmazeHHSho-HsWfI3sJSs46sVCahe6tKKCB5N1uo\_kqzP\_uu-lrQipUYTBhxNgdN-YZ\_nhw94ac0o-)

#### How much emissions is a specific farm entitled to?

A farm is entitled to its weight multiplied by the picklePerBlock. If a given farm has a 10% weight, and the current emissions are 0.2 pickles per block, then that farm is receiving 0.02 PICKLEs per block, to be split pro-rata throughout its farm holders. You can see current emissions at [Tokenomics and Emission Schedule](pickle-token/tokenomics-and-emission-schedule.md).\


#### How much emissions does each pToken in the farm get?

The amount of emissions a single pToken in a farm is entitled to is calculated by dividing the amount of emissions allocated to that farm by the number of pTokens in that farm. For example, if the Farm is receiving 0.02 PICKLEs / block, and there are 10,000 pTokens staked on the Farm this block, each pToken receives 0.000003 PICKLEs / block. The farms with the best emission payouts are the ones with a high weight and a low pool size. This means more rewards are divided over lower dollar amounts, and can contribute tremendously to yield. \


#### What is the current price of the PICKLE token?

Since yield is a function of both principal (your pToken deposit) and returns (the PICKLE rewards), both affect the resulting APR. The higher the price of the PICKLE token, the more those rewards count towards your APR.&#x20;



#### But why is the APY a range?

![](https://lh4.googleusercontent.com/I56BIKq6c6ZKturGmHURl0xh7RBLen9OnnRFBeSaaqIqHoO1fGHOVgpUQce-a8W72-GEna19BotfzddjZTay3tD6sGjBCvd2mbql7HuvUYXIXFueumKEEUDaSqffKEdZyDvrRXEM)

You may notice that each Farm displays an APR range. Which APR, within the range, you will receive works as follows:

* If you have no DILL balance, you will receive the APR at the lower end of the range. This is the base APR that all unboosted users receive.
* If you hold DILL, you will receive a boosted APR. Your current boost can be checked with the calculator[ here](http://app.pickle.finance/dill).
* The higher end of the range displayed on each Farm shows the APR with the 2.5x boost.
* Once you stake your pTokens in the Farm, your exact APR will be displayed next to the APR range on the "my APR" indicator.

One of the main incentives for locking PICKLE tokens as DILL is the ability to boost your PICKLE rewards on our [Pickle Farms](https://app.pickle.finance/farms). Depositors are able to earn a max boost of up to 2.5x.

The following considerations govern how much of a boost you obtain:

* Your proportional share of the total DILL supply
  * If you own a larger share of the total supply, you will obtain a larger boost.
* Your proportional share of a particular Farm
  * If your deposit in a particular Farm is small relative to the total deposits, it will be easier for you to obtain the max boost. The opposite is true if you comprise a large share of the deposits in a Farm (i.e. more DILL is needed for max boost).
  * e.g. if the total deposits in a Farm is $100,000 a smaller DILL balance is required to obtain the max boost if your deposit size was $1,000 compared to if your deposit size was $20,000.

In summary, your DILL balance applies to all Farms equally but may produce different boosts of up to 2.5x based on your share of deposits in the Farm.

![](https://lh3.googleusercontent.com/7xTrrJfTWthmdEDQTEkZNZ7OMFSkkT8nArCDC8FslqROqy5Ym0uKF-l8EZk7DsMQ695B7GI\_gXmEGZ16MQopvdpt8tATQ5Jd6IvwkroYZbwScl7YKGHfEPVHnpL14d60eFCovE5k)

A [calculator](http://app.pickle.finance/dill) is provided here to estimate how much DILL is required for obtaining certain boosts given the specific conditions of each of the Farms.
