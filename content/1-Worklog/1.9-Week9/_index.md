---
title: "Worklog Week 9"
date: 2026-06-18
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---

### Week 9 Objectives:

* Conduct comprehensive backend business analysis for the multi-tier hospital workflow and design a robust DynamoDB Single-table database schema.
* Research payment gateway integration (VNPay/MoMo) and architect a secure medical records integrity mechanism anchored on Amazon Managed Blockchain (AMB) / Ethereum.

### Tasks to be Deployed This Week:
| Day | Task Description | Start Date | End Date | Resource Links |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6 | - Analyzed backend business requirements for the entire hospital workflow from registration, examination, lab tests to invoicing and payments. | 12/06/2026 | 12/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Designed the backend domain schema on DynamoDB using a Single-table pattern; defined partition strategies for core entity types (USER, PATIENT, DOCTOR, INVOICE, MEDICAL_LEDGER_BLOCK). | 15/06/2026 | 15/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Standardized data key conventions (`pk`/`sk`) and primary cross-referencing fields (patientId, citizenId, recordId, etc.) to optimize role-based queries. | 16/06/2026 | 16/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Formulated a legacy data migration strategy to transition medical record identifiers to a National ID (`citizenId`) baseline for structural unification. | 17/06/2026 | 17/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Analyzed technical specifications for VNPay/MoMo APIs (paymentUrl, IPN/callbacks) and designed the medical payload hashing pipeline for AMB integration. | 18/06/2026 | 18/06/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Key Results Achieved in Week 9:

* Finalized business analysis and DynamoDB Single-Table schema design:
  * Successfully modeled cross-tier data flows for 12 critical entities within the hospital management system.
  * Formulated an Access Pattern matrix mapping business queries to `pk`/`sk` key pairs, optimizing read/write efficiencies and cost overheads on DynamoDB.
  * Unified medical record anchoring around the National ID (`citizenId`), successfully eliminating historical data fragmentation.

* Engineered payment integration and blockchain security blueprints:
  * Designed definitive Sequence Diagrams for VNPay/MoMo transaction processing, clarifying cryptographic signature validation and IPN handling mechanisms.
  * Completed the mathematical definitions for medical payload hashing and internal ledger block generation prior to anchoring onto Ethereum via Amazon Managed Blockchain (AMB).