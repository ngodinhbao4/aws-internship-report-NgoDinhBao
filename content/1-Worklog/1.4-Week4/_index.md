---
title: "Week 4 Worklog"
date: 2026-05-14
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:
* Master core theories of infrastructure Auto Scaling and High Availability (HA) architectures.
* Successfully configure a Launch Template derived from an existing EC2 Amazon Machine Image (AMI).
* Deploy an Auto Scaling Group (ASG) within a VPC network and seamlessly integrate it with Elastic Load Balancing (ELB).
* Implement automated Scaling Policies governed by predefined AWS CloudWatch Alarm thresholds.

### Tasks to Implement This Week:
| Day | Task | Start Date | Completion Date | Document Sources |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6 | - Study theoretical fundamentals of Auto Scaling (Vertical vs. Horizontal scaling mechanics). <br> - Explore design principles for building High Availability (HA) infrastructures. | 08/05/2026   | 08/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Create a custom Amazon Machine Image (AMI) from a running EC2 instance. <br> - Initialize a Launch Template embedded with instance types, key pairs, and security groups using that AMI. | 11/05/2026   | 11/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Configure an Auto Scaling Group (ASG) partitioned across a Custom VPC network. <br> - Define capacity boundary metrics (Desired, Minimum, and Maximum capacity constraints). | 12/05/2026   | 12/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Bind Elastic Load Balancing (ELB) target distributions with the newly provisioned ASG. <br> - Research dynamic scaling policy implementations (Target Tracking and Step Scaling). | 13/05/2026   | 13/05/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - **Hands-on Lab:** <br>Formulate and execute dynamic Scaling Policies tied to CloudWatch Alarm parameters, followed by performing stress testing on the cluster. | 14/05/2026   | 14/05/2026      | <https://cloudjourney.awsstudygroup.com/> |


### Week 4 Key Achievements:
* **Architectural Insights:** Developed a profound understanding of implementing High Availability frameworks (Multi-AZ deployment) to successfully eradicate Single Points of Failure (SPOF).
* **Configuration Standardization:** Built a production-ready Launch Template from a Custom AMI, enabling swift and automated server replication capabilities.
* **Infrastructure Automation:** Deployed an elastic Auto Scaling Group that adaptively controls instance fleet counts matching live system load requirements in the VPC.
* **Elastic System Integration:** Successfully unified ASG and ELB workflows; engineered dynamic scaling policies that scale out or scale in instances accurately response to AWS CloudWatch Alarm triggers.