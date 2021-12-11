---
description: >-
  A description of the different strategies employed by Pickle Finance's
  PickleJars.
---

# Pickle Jar Strategies

## Introduction

Each PickleJar employs a Strategy contract to earn yield for its depositors. In this document, we explore the types of Strategies being employed and how these work under the hood.

The PickleJar system is largely based on Yearn's v1 [yVault](https://yearn.finance/vaults) system, and therefore the most relevant function is the `harvest()` function, which is what executes the profit-generating steps.

All Strategy contracts are being developed under the [`src/strategies`](https://github.com/pickle-finance/protocol/tree/master/src/strategies) directory of the [protocol](https://github.com/pickle-finance/protocol) repository. For a listing of all currently deployed Strategy contracts, see the [contracts](https://github.com/pickle-finance/contracts#pickle-jars-pjars) repo.

All pickle jars have 20% performance fee. The displayed APY% is the net APY after the fees.
