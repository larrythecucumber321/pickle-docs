---
description: Put your tokens into a PickleJar and earn without losing your principal.
---

# What are Pickle Jars?

The PickleJars can be found at [https://app.pickle.finance/jars](https://app.pickle.finance/jars)

![https://app.pickle.finance/jars](<../../.gitbook/assets/image (16).png>)

### Intro to PickleJars

![How picklejar works (Thanks Fennec)!](<../../.gitbook/assets/image (43).png>)

Each PickleJar (or pJar) employs a different alpha seeking strategy, but fundamentally works in a similar manner:

1. Creating the input tokens in relevant project, for example ALCX/ETH
2. Users deposit the 10 ALCX/ETH sLP (Sushi Liquidity Provider) tokens into pJar 0.99x and receive 10pTokens (if one deposits in the beginning of the jar's creation. Otherwise it depends on the ratio or the underlying asset which has appreciated).\
   2.1. PICKLE protocol will collect the ALCX reward with 20% performance fee\
   2.2.  which half of it will be sold for ETH, and reinvested back to the sLP. Your pToken will not increase, but when you exit the jar, the ALCX/ETH sLP will be worth more depending when you exit.
3. You can deposit your pTokens into the pickle farm.\
   3.1. and the farm will give you PICKLE token in addition to your compounding Jar.\
   3.2. You can sell your PICKLE\
   3.3. Or you can lock your PICKLE for DILL (1 PICKLE = 1 DILL if locked 4 years) for the protocol revenue sharing!

### What are the different PickleJars?

A total of 23 PickleJars have been deployed so far:

1. pJar 0a: A Curve strategy for [sUSDv2 pool](https://www.curve.fi/susdv2/deposit) (sUSDv2 pool employs a basket of 4 stablecoins to peg to US$1 and the switching between them to be stable at $1, learn more about [sUSD](https://docs.synthetix.io/litepaper)). CRV reward is sold for more LP.
2. pJar 0b: A Curve strategy for [renBTC pool](https://www.curve.fi/ren/deposit) (renBTC pool employs a basket of renBTC and WBTC to peg to 1BTC. Learn more about [renVM](https://github.com/renproject/ren/wiki#tldr) and [WBTC](https://wbtc.network/)). CRV reward is sold for more LP.
3. pJar 0c: A Curve strategy for [3poolCRV pool](https://www.curve.fi/3pool/deposit) (3poolCRV pool employs the 3 most popular stablecoins to peg to US$1 and the switching between them to be stable at $1, learn more about [DAI](https://makerdao.com/en/), [USDC](https://www.circle.com/en/usdc), and [USDT](https://tether.to/)). CRV reward is sold for more LP.
4. pJar 0d: A Curve strategy for [stETH pool](https://www.curve.fi/steth/deposit) (stETH pool aims to peg the staked ETH in LIDO and making stETH liquid and peg it to 1ETH. Learn more about [LIDO](https://www.lido.fi/)). LIDO and CRV reward is sold for more LP.
5. pJar 0.99a: A Sushiswap strategy for [ETH:DAI](https://exchange.sushiswapclassic.org/#/add/0x6b175474e89094c44da98b954eedeac495271d0f/ETH) ([V](https://exchange.sushiswapclassic.org/#/add/0x6b175474e89094c44da98b954eedeac495271d0f/ETH)ery straight forward, an LP of ETH/[DAI](https://makerdao.com/en/) - ~~0% performance fee~~) (Sushiswap has removed vesting, so we have reimplemented 20% performance fee back). SUSHI reward is sold for more LP.
6. pJar 0.99b: A Sushiswap strategy for [ETH:USDC](https://exchange.sushiswapclassic.org/#/add/0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48/ETH) (an LP of ETH/[USDC](https://www.circle.com/en/usdc) - ~~0% performance fee~~). SUSHI reward is sold for more LP.
7. pJar 0.99c: A Sushiswap strategy for ETH:[USDT](https://exchange.sushiswapclassic.org/#/add/ETH/0xdac17f958d2ee523a2206206994597c13d831ec7) (an LP of ETH/[USDT](https://tether.to/) - ~~0% performance fee~~). SUSHI reward is sold for more LP.
8. pJar 0.99d: A Sushiswap strategy for [ETH:WBTC](https://exchange.sushiswapclassic.org/#/add/0x2260fac5e5542a773aa44fbcfedf7c193bc2c599/ETH) (an LP of ETH/[WBTC](https://wbtc.network/) - ~~0% performance fee~~). SUSHI reward is sold for more LP.
9. pJar 0.99e: A Sushiswap strategy for [ETH:YFI](https://exchange.sushiswapclassic.org/#/add/0x0bc529c00C6401aEF6D220BE8C6Ea1667F6Ad93e/ETH) (an LP of ETH/YFI - ~~0% performance fee.~~ YFI is [yearn.finance](https://yearn.finance) governance token). SUSHI reward is sold for more LP.
10. ~~pJar 0.99f: A Uniswap strategy for seignorage token~~ [~~BAC~~](https://app.uniswap.org/#/add/0x3449FC1Cd036255BA1EB19d65fF4BA2b8903A69a/0x6B175474E89094C44Da98b954EedeAC495271d0F) ~~(an LP of BAC/DAI. BAC is a decentralized stablecoin with an algorithmic Central Bank. BAC aims to peg to US$1. Read more~~ [~~here~~](https://docs.basis.cash/mechanisms/stabilization-mechanism) ~~about how its mechanism works.)~~ retired due to upgrade.
11. ~~pJar 0.99g: A Sushiswap strategy for seignorage token MIC~~ (retired, due to migration and required whitelist of yield aggregator)
12. ~~pJar 0.99h: A Sushiswap strategy for seignorage token MIS~~ (retired, due to migration and required whitelist of yield aggregator)
13. ~~pJar 0.99i: A Sushiswap strategy for~~ [~~ETH/yveCRV~~](https://sushiswap.fi/pair/0x10b47177e92ef9d5c6059055d92ddf6290848991) ~~(A unique collaboration of Curve, Yearn, Sushi and Pickle. CRV is deposited for yield boost in yearn, which the yveCRV token can be staked together with ETH in sushiswap which yields SUSHI, and Pickle will be selling the SUSHI reward to be sold and compounded to LP tokens.~~ \
    ~~There is a zap in both~~ [~~Yearn~~](https://yearn.finance/vaults) ~~and~~ [~~Pickle~~](https://app.pickle.finance/) ~~website that helps automagically transform your ETH or CRV into the PickleJar.~~\
    ~~**Warning: yveCRV cannot be converted back to CRV, because the CRV is perpetually staked in Curve's voting escrow. So, CRV =/= yveCRV in term of price;** each has their own value which can be found on Coingecko.~~ [~~**CRV**~~](https://www.coingecko.com/en/coins/curve-dao-token) ~~and~~ [~~**yveCRV**~~](https://www.coingecko.com/en/coins/vecrv-dao-yvault) ~~**** price. So if the price of either token is off-peg, you may want to DYOR on how to put in the pJar.~~ retired, upgraded to yvBOOST, see below.\
    ~~**Reminder:** only 1/3 of SUSHI that will be harvested and reinvested. To date, there is no way for smart contract (yield aggregator) to claim the 2/3 of SUSHI. To make up for this, the pJar can be staked in pickle farm to earn additional pickle)~~ Vesting has been removed from Sushiswap.
14. pJar 0.99j: A Uniswap strategy for [BAS:DAI](https://app.uniswap.org/#/add/0x106538cc16f938776c7c180186975bca23875287/0x6B175474E89094C44Da98b954EedeAC495271d0F) (an LP of DAI:BAS. Basis Share (BAS) is a medium of governing the protocol, and receiving seigniorage rewards through the Boardroom. How it works is explained in the [whitepaper](https://github.com/rmsams/stablecoins/blob/master/paper.pdf)). retired due to upgrade.
15. pJar 0.99k: A Uniswap strategy for [UST:MIR](https://app.uniswap.org/#/add/0x09a3ecafa817268f77be1283176b946c4ff2e608/0xa47c8bf37f92aBed4A126BDA807A7b7498661acD) (an LP of UST:MIR. UST is the stablecoin in [Terra network](https://terra.money/#1) while [MIR](https://docs.mirror.finance/protocol/mirror-token-mir) is the governance token of Mirror protocol.) MIR reward is sold for more LP.
16. pJar 0.99l: a Mirrored TSLA (mAsset) strategy for [UST:MTSLA](https://app.uniswap.org/#/add/0x21cA39943E91d704678F5D00b6616650F066fD63/0xa47c8bf37f92aBed4A126BDA807A7b7498661acD) (an Uniswap LP of UST:MTSLA). MTSLA is a mirrored [Tesla Inc. Common Stock](https://www.nasdaq.com/market-activity/stocks/tsla), using a decentralized oracles from Band protocol, which updates every 15 seconds on the Band chain. Read more [here](https://medium.com/mirror-protocol/mirror-protocol-partners-with-band-protocol-to-secure-issuance-of-synthetic-stocks-and-etfs-1a12181b6cdc). MIR reward is sold for more LP.
17. pJar 0.99m: a Mirrored APPL (mAsset) strategy for [UST:MAAPL](https://app.uniswap.org/#/add/0xd36932143F6eBDEDD872D5Fb0651f4B72Fd15a84/0xa47c8bf37f92aBed4A126BDA807A7b7498661acD) (an Uniswap LP of UST:MAAPL). MAAPL is a mirrored [Apple Inc. Common Stock](https://www.nasdaq.com/market-activity/stocks/aapl). MIR reward is sold for more LP.
18. pJar 0.99n: a Mirrored QQQ (mAsset) strategy for [UST:MQQQ](https://app.uniswap.org/#/add/0x13B02c8dE71680e71F0820c996E4bE43c2F57d15/0xa47c8bf37f92aBed4A126BDA807A7b7498661acD) (an Uniswap LP of UST:MQQQ). MQQQ is a mirrored [Invesco QQQ Trust](https://www.nasdaq.com/market-activity/funds-and-etfs/qqq). MIR reward is sold for more LP.
19. pJar 0.99o: a Mirrored SLV (mAsset) strategy for UST:MSLV (an Uniswap LP of UST:MSLV) MSLV is a mirrored [iShare Silver Trust](https://www.nasdaq.com/market-activity/funds-and-etfs/slv). MIR reward is sold for more LP.
20. pJar 0.99p: a Mirrored BABA (mAsset) strategy for UST:MBABA (an Uniswap LP of UST:MBABA) MBABA is a mirrored [Alibaba Group Holding Limited](https://www.nasdaq.com/market-activity/stocks/baba). MIR reward is sold for more LP.
21. pJar 0.99q: a Sushiswap strategy for [ETH:SUSHI](https://app.sushi.com/pair/0x795065dcc9f64b5614c407a6efdc400da6221fb0) (An LP of ETH/SUSHI). SUSHI reward is sold for more LP.
22. pJar 0.99r: an Uniswap strategy for [FEI:TRIBE](https://app.sushi.com/pair/0x795065dcc9f64b5614c407a6efdc400da6221fb0) ("FEI is a highly scalable, decentralized, and reserve-backed stablecoin". Read more about FEI [here](https://medium.com/fei-protocol/what-you-should-know-about-fei-3ccffd4a4bb6). TRIBE is the governance token that manages the protocol.) TRIBE reward is sold for more LP.
23. pJar 0.99u: an Uniswap strategy for [ETH:LUSD](https://app.uniswap.org/#/add/0x5f98805A4E8be255a32880FDeC7F6728C6568bA0/ETH). LUSD is the stablecoin of Liquity, a borrowing protocol allowing users to borrow interest-free loans against their ETH collateral. Read more about Liquity and LUSD [here](https://www.liquity.org/). LQTY reward is sold for more LP.
24. pJar 0.99x: a Sushiswap strategy for [ETH:ALCX](https://app.sushi.com/add/0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2/0xdbdb4d16eda451d0503b854cf79d55697f90c8df). ALCX is the governance token for Alchemix Finance. Taken from their website "Alchemix Finance is a future-yield-backed synthetic asset platform and community DAO. The platform gives you advances on your yield farming via a synthetic token that represents a fungible claim on any underlying collateral in the Alchemix protocol.". Read more about Alchemix [here](https://alchemix-finance.gitbook.io/alchemix-finance/). ALCX reward is sold for more LP.
25. pJar 0.99y: a Sushiswap strategy for ETH:YVBOOST. yvBOOST is the upgraded version of yveCRV, which incorporate the weekly reward from CRV automatically. SUSHI reward is sold for more LP.

Detailed information on each PickleJar can be found below:

{% content-ref url="pjar-0.md" %}
[pjar-0.md](pjar-0.md)
{% endcontent-ref %}

{% content-ref url="pjar-0.69.md" %}
[pjar-0.69.md](pjar-0.69.md)
{% endcontent-ref %}

{% content-ref url="pjar-0.88.md" %}
[pjar-0.88.md](pjar-0.88.md)
{% endcontent-ref %}

{% content-ref url="pjar-0.99.md" %}
[pjar-0.99.md](pjar-0.99.md)
{% endcontent-ref %}

