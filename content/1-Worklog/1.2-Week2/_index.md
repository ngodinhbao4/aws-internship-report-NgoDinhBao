---
title: "Week 2 Worklog"
date: 2026-04-30
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---



### Week 2 Objectives:

* Understand core networking concepts (VPC, Subnet) and secure Internet connectivity methods (IGW, NAT).
* Differentiate and practically apply network infrastructure security layers (Security Groups & NACLs), deploy object storage services (S3), and set up relational databases (RDS).s

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 6   | - Learn networking concepts and set up a Custom VPC (Configure Public/Private Subnets)                                                                                                | 24/04/2026 | 24/04/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 2   | - Understand and configure Internet Gateway (IGW) & NAT Gateway                                   | 27/04/2026 | 27/04/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 3   | - Differentiate and configure Security Groups & Network ACLs (NACLs). | 28/04/2026 | 28/04/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Explore S3 Bucket (Policies) & Set up and manage Amazon RDS.      | 29/04/2026 | 29/04/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - **Hands-on Lab:** <br>Design and build a comprehensive Multi-tier Network Architecture.                                                               | 30/04/2026 | 30/04/2026      | <https://cloudjourney.awsstudygroup.com/> |


### Week 2 Achievements:

* Mastered core AWS networking concepts and successfully configured a customized network infrastructure, including:
  * Initializing a Custom VPC and assigning appropriate IP ranges (CIDR Blocks).
  * Setting up and clearly distinguishing between Public Subnets and Private Subnets.
  * Configuring custom Route Tables to properly direct network traffic for each zone.

* Successfully configured network connectivity and routing mechanisms:
  * Attached an Internet Gateway (IGW) to enable outbound and inbound internet access for Public Subnets.
  * Deployed a NAT Gateway within the Public Subnet to grant secure, outbound-only internet connectivity for instances in Private Subnets.

* Gained the ability to manage and flexibly apply infrastructure security layers:
  * Deeply understood the behavioral differences between Security Groups (Stateful - Instance level) and NACLs (Stateless - Subnet level).
  * Formulated robust Inbound/Outbound security rules to isolate and protect cloud resources.

* Successfully managed storage and database services:
  * Created S3 Buckets and mastered configuring Bucket Policies for secure file access management.
  * Provisioned and managed an Amazon RDS relational database instance securely isolated inside a Private Subnet.

* Completed the comprehensive integration milestone:
  * Successfully designed, deployed, and validated a functional **Multi-tier Network Architecture**, ensuring secure communication paths among presentation, application, and database tiers.