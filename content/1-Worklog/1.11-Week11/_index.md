---
title: "Worklog Week 11"
date: 2026-07-02
weight: 1
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

* Resolve medical record synchronization defects, finalize live financial transaction processes with VNPay/MoMo gateways, and implement an internal Medical Integrity Ledger.
* Engineer database backfill mechanisms for block state resets and integrate cryptographic transaction broadcasting onto the AMB/Ethereum network.

### Tasks to be Deployed This Week:
| Day | Task Description | Start Date | End Date | Resource Links |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6 | - Rectified backend-to-frontend medical record desynchronization errors, standardizing on National ID (`citizenId`) formatted identifiers. | 26/06/2026 | 26/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Completed live transaction backend routines for VNPay/MoMo integrations (payment request handling, SHA256/HMAC checksum signatures, IPN parsing). | 29/06/2026 | 29/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Implemented rigorous payment status verification filters (signature check, invoice matching, amount checking) to sync PAYMENT, INVOICE, and APPOINTMENT states. | 30/06/2026 | 30/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Designed and developed the internal Medical Integrity Ledger module (payload canonicalization, hash linking utilizing `previousHash` and `blockHash`). | 01/07/2026 | 01/07/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Constructed ledger backfill utilities for seed dataset resets; extracted node credentials securely from AWS Secrets Manager to broadcast transactions to AMB. | 02/07/2026 | 02/07/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Key Results Achieved in Week 11:

* Resolved structural defects and finalized financial processing engines:
  * Terminated front-end record mismatch bugs by enforcing National ID configurations across all nested clinical items.
  * Successfully deployed HMAC-SHA256 signature signing algorithms, securely parsing `returnUrl` parameters and asynchronous `IPN` webhooks to reflect real-time payment updates.

* Deployed internal cryptographically linked ledger and cloud-blockchain connectivity:
  * Built a tamper-proof cryptographically chained internal ledger module guarding medical document events against illicit alterations.
  * Developed robust backfill functions to reconstruct the chained ledger blocks instantly following dataset resets.
  * Established Web3 node runtime integrations, retrieving private keys via AWS Secrets Manager to commit transaction hashes and block numbers directly onto Amazon Managed Blockchain.