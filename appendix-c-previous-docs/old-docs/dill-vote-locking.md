---
description: Understand what locking PICKLEs for DILL is all about
---

# DILL Vote Locking

## What is Vote Locking? What is DILL?

Vote-locking is a modified form of governance staking. Governance voters lock their governance tokers to participate in voting. This prevents governance attacks and aligns incentives between voters and long-term holders.&#x20;

PICKLE is the governance token of Pickle Finance. You can vote-lock your PICKLEs for DILL in order to:

1. Participate in [**governance**](governance.md) (1 vote = 1 DILL), including Snapshot voting and on-chain governance.
2. PICKLE farm weight voting rights, DILL holders get to vote on the farm gauges for PICKLE emissions.&#x20;
3. Receive up to **2.5x** [**boost**](boost.md) **in PICKLE rewards.**
4. Receive **45% of the protocol's** [**revenues**](revenue-sharing.md), distributed weekly in market-bought PICKLEs

DILL represents your balance of PICKLEs that have been vote-locked, weighed for the time remaining in the lock.  The longer the time remaining in the lock, the more DILL you will have for the same amount of locked PICKLEs:

| PICKLE x LOCKED DURATION | NUMBER OF DILL        |
| ------------------------ | --------------------- |
| 1 PICKLE x 1 week        | 0.0048 DILL (approx.) |
| 1 PICKLE x 1 year        | 0.25 DILL             |
| 1 PICKLE x 2 years       | 0.50 DILL             |
| 1 PICKLE x 3 years       | 0.75 DILL             |
| 1 PICKLE x 4 years       | 1.00 DILL             |

See [here ](lock-pickles/)for a guide on interacting with DILL on the UI.

## Transferability & Decay of DILL&#x20;

With DILL, the following things are NOT possible:

* Decreasing your lock time
* Decreasing the amount of PICKLEs locked
* Transferring your DILL balance to another wallet

Once a DILL lock is created, the lock will continue until expiry and cannot be transferred or undone in any way. Creating, extending, and increasing locks are _irreversible_ actions.

## Decaying DILL Balance

Your DILL balance decreases linearly over time. Your PICKLE tokens do not decay. All funds are safu. Towards the end of your lock, your DILL balance will approach 0. On expiry of your lock, all of your deposited PICKLE tokens will be released at once – you do not need to perform an "unlock transaction".&#x20;

The only way to mitigate this decay is to extend your lock or increase your lock with more PICKLEs.
