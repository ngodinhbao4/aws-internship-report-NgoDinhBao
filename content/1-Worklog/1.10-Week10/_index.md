---
title: "Worklog Week 10"
date: 2026-06-25
weight: 1
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives:

* Build foundational backend REST APIs supporting Patients, Doctors, Medical Records, and initial Invoicing workflows.
* Enforce Role-Based Access Control (RBAC) utilizing Amazon Cognito User Groups and prepare mock dataset scripts for comprehensive integration testing.

### Tasks to be Deployed This Week:
| Day | Task Description | Start Date | End Date | Resource Links |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6 | - Implemented foundational patient and user management APIs (profile retrieval, personal records updating, appointment scheduling). | 19/06/2026 | 19/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Developed backend endpoints for the Doctor module: Shift scheduling, examination queue management, and National ID-based patient lookups. | 22/06/2026 | 22/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Constructed core medical operation APIs including clinical reports, digital prescriptions, and laboratory requests mapped to a unique `recordId`. | 23/06/2026 | 23/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Developed the initial invoice processing sub-module APIs (invoice creation from appointments/services, payment status queries). | 24/06/2026 | 24/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Configured secure API routing access using Amazon Cognito User Groups; authored and executed database seed scripts via the AWS CLI. | 25/06/2026 | 25/06/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Key Results Achieved in Week 10:

* Constructed and bundled core operational business APIs:
  * Successfully deployed API routes for Patients and Doctors, ensuring queue operations and National ID lookups operate seamlessly.
  * Bundled healthcare transactional endpoints (prescriptions, clinical examinations, lab requests), guaranteeing comprehensive metadata cross-referencing.
  * Finished initial invoice state tracking engines on DynamoDB.

* Advanced security containment and testing frameworks:
  * Integrated Cognito Group-based Authorizers effectively, cleanly isolating endpoints across system roles (Admin, Doctor, Staff, Patient).
  * Authored and validated automated data seeding scripts; inspected item schemas using the AWS CLI to ensure flawless data rendering for frontend clients.