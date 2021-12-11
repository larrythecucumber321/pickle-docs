# Security

Security is paramount in DeFi, where a large amount of trust must be placed on properly coded smart contracts and on other safety measures.

## **Smart Contract Audits**

### MixBytes Audit

An audit of the full suite of Pickle Finance smart contracts by [MixBytes](https://mixbytes.io) commenced on October 3, 2020.&#x20;

To date, the all of the PickleJar [**strategy** ](strategies.md)contracts have been audited.&#x20;

No critical or major issues were found in the strategy contracts. Minor issues have been fixed. The audit report warned of suspicious proxy functions (which the Pickle Finance developers explained were necessary and were protected by a 12 hour timelock). The full report can be viewed [**here**](https://github.com/pickle-finance/protocol/blob/master/audits/MixBytes\_Audit\_All\_Strategies.pdf).

An audit of the remaining contracts is underway and is expected to complete shortly.

### **Haechi Audit**&#x20;

An audit of the full suite of Pickle Finance smart contracts by [Haechi](https://audit.haechi.io) commenced on October 20, 2020.&#x20;

Haechi has completed a preliminary audit of our smart contracts. We are currently working through remediations, at which point a final report will be issued.

## **Timelocks & Multisig**

All key admin functions on the [MasterChef ](https://etherscan.io/address/0xbD17B1ce622d73bD438b9E658acA5996dc394b0d)contract, which controls the emission of PICKLEs to the [Farms](farms.md) are controlled by a [**24 hour timelock contract**](https://etherscan.io/address/0x0040E05CE9A5fc9C0aBF89889f7b60c2fC278416).&#x20;

All key admin functions relating to the [PickleJars](jars.md) are controlled by a [**12 hour timelock contract**](https://etherscan.io/address/0xD92c7fAa0Ca0e6AE4918f3a83d9832d9CAEAA0d3).

Each of the above timelock contracts must be executed through a 2/5 community [**multisig wallet**](https://etherscan.io/address/0x9d074E37d408542FD38be78848e8814AFB38db17). The current multisig keyholders are as follows:

![](<../../.gitbook/assets/image (22).png>)

Polygon multi-sig wallet.\


![](<../../.gitbook/assets/image (46).png>)
