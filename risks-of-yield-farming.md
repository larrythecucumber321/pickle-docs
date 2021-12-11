# Risks of Yield Farming

### Introduction <a href="#docs-internal-guid-bafba6df-7fff-2867-4c2b-ff461c0bac20" id="docs-internal-guid-bafba6df-7fff-2867-4c2b-ff461c0bac20"></a>

Yield Farming, and DeFi in general, contains risk. There are many different types of risks, and as a participant in this space it is your duty to be as aware of these as possible. This is not an exhaustive list, but the most common or notable risks associated with Decentralized Finance.&#x20;

* You could lose your keys or get hacked.&#x20;
* The protocol could get hacked
* A lending platform could be hit by a wave of defaults
* A stablecoin could lose its peg and become not-so-stable.&#x20;
* Liquidity Pools are advanced (but important) topics and you should fully understand them.
* Any project, or any Liquidity Pool with that project’s token, could turn out to be a rug-pull or scam.

### Losing your Keys / Getting Hacked

Losing your seed phrase, private key, or getting hacked and having those critical credentials stolen are risks that anyone involved in DeFi or Cryptocurrencies more generally should be aware of. The loss of these credentials will cause you to permanently lose access to all of your funds, with absolutely no method to reclaim them. Much has been written about these topics, and we encourage all of our users to do their research on how best to protect themselves against permanent and catastrophic loss.&#x20;

### Protocol Hacks

Any protocol can be hacked. Savvy hackers can analyze a contract for any opportunity to steal funds. Users should be aware that while Pickle Finance is audited and takes every possible step to secure user funds, the unthinkable can and has happened throughout the DeFi ecosystem.

Pickle Finance is currently working on a “Safety Module” / insurance program to help insure against losses. It is not yet released, however, even when it is released and fully functional, there is no guarantee all funds will be returned in a timely manner.&#x20;

### Lending Platforms and Defaults

Lending Platforms make loans to other customers, usually based on some deposited collateral. If the value of the collateral drops below a certain Loan-To-Value ratio, these lending platforms will engage several mechanisms to liquidate the collateral and reclaim the value. Each lending platform may perform this task differently, and each platform may be more or less subject to losses during bear markets. Users are encouraged to be aware of which lending platform they are interacting with, become familiar with their liquidation procedures, and decide if they are comfortable with the liquidation procedures or the trustworthiness of the platform generally. While most lending platforms today have procedures that can withstand even significant market downturns, each of these platforms may be affected differently by flash crashes or severe downturns.&#x20;

### Stablecoins - Loss of Peg

Whether they are involved in a liquidity pool or just a general stablecoin lending platform investment, users should be aware that all stablecoins may theoretically be at risk of going off peg for a period of time. This “loss of peg” occurs when the stablecoin fails to maintain the value it is designed to match. If a stablecoin fails to maintain peg, or fails to quickly regain peg after such an occurrence, the token may begin to lose favor in the marketplace or depreciate rapidly. When involved in any stablecoin investment, users should be aware of how the stablecoin works, what the collateral or reserves in its treasury are used for, and the mechanism the token uses to maintain its peg. Investing in all stablecoins carry some level of risk. Investing in novel stablecoins with untested mechanisms to maintain their peg likely carries more.&#x20;

### Liquidity Pools: ~~Impermanent Loss~~ Divergence Loss

Divergence Loss is the much more accurate name for what many are calling “Impermanent Loss”, and is defined as “the difference in profit between holding an asset versus providing liquidity in that asset.” In short, Divergence Loss is how much you make (or lose) when joining a liquidity pool for two tokens, compared to how much loss or gain you would have had if you had simply held the tokens directly. The reason this is appropriately called “Divergence Loss” is because this difference in value gets larger as tokens diverge from each other compared to when liquidity was initially provided. The more two tokens move relative to each other, the larger the difference in value between holding the tokens versus providing liquidity to those tokens. \


As a quick example, take the case of a user that has $500 in ethereum, and $500 in DAI. If Ethereum goes up 500%, and DAI stays flat (as stablecoins do), simply holding these tokens would result in the user having $3000 in Ethereum, and $500 in DAI, for **a total value of $3500** and **a gain of $2500** (or 250%). If, on the other hand, the user deposits these tokens into a DAI-ETH liquidity pool, the user would have a total value of only **$2482.47**, representing a gain of **$1482.47** (or 148%).&#x20;

The DIFFERENCE of these two values is the divergence loss. In the above case, the user has experienced a **divergence loss of $1017.53**. Divergence loss does not imply a real loss has occurred (but it also does not mean a real loss has NOT occurred either).&#x20;

Any losses other than one calculated as above **is not** an “Impermanent Loss” or a “Divergence Loss”. They are more likely to be a loss in “Opportunity Cost” (“I had money in Pickle-Eth liquidity pool, but if I had only ETH I would have made way more money!”) or normal losses on tokens depreciating (both Pickle and ETH dropped and I lost money).&#x20;

Remember, Divergence Loss is **the difference in profit of holding tokens versus providing liquidity for those tokens.** Divergence loss is directly caused by the liquidity pool function of “buying the dip” and “selling the pop”. As a token goes sharply up, the liquidity pool is selling it (and thus, not capturing the full rise of the token). As a token goes sharply down, a liquidity pool is buying more of it (and buying the dip when more dips are coming can lead to larger losses).&#x20;

This does not mean Liquidity Pools are bad investments. It just means that investors should be confident in your choice of which pools and which tokens you want to provide liquidity to. You should also stay vigilant for developments in these tokens and know under what circumstances you would no longer be willing to provide liquidity for the pair. In short, if you like both tokens, and want to buy the dips and sell the pops, and get paid fees to do so, a liquidity pool might be right for you.&#x20;

### Liquidity Pools: Normal Losses On Tokens

When entering a liquidity pool, your losses are not limited to “Divergence Loss”.  While “Divergence Loss” is defined as the difference between holding two tokens and providing liquidity for them, normal losses on tokens also occur. If you simply held the equal value of two tokens outside of a liquidity pool (for example, $500 worth of DAI and $500 worth of ETH), and one of them drops by 50%, you will lose 25% of your investment. If both tokens drop, you may lose more. The same is true when you provide liquidity for a pair. Your tokens may lose value and you may experience losses.&#x20;

### Liquidity Pools: Getting Rugged

Users should be aware that losses in a liquidity pool are not limited to only the “volatile” token. Some users believe that investing in a liquidity pool consisting of a volatile token paired with a stablecoin limits their losses to only half of their investment. This is not true.&#x20;

Because a liquidity pool will consistently “buy the dip”, if a user enters a **stablecoin-shitcoin** liquidity pool, and one token enters a downward spiral to zero, the users entire investment is likely to be held in that decreasing coin. The liquidity pool will buy the dip over and over and over until all of its funds are either gone or invested in a coin that is headed to zero.&#x20;

Users should not be scared of liquidity pools in their entirety, but rather should carefully analyze the tokens they are investing in and whether one of those tokens may be subject to such a downward spiral.
