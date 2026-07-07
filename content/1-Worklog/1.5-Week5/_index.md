---
title: "Worklog Week 5"
date: 2026-05-21
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:

* Gain a foundational understanding of dynamic infrastructure scaling (AWS Auto Scaling Groups) and resource monitoring mechanisms (Amazon CloudWatch Alarms).
* Implement hands-on configurations and execute real-world stress testing to verify and evaluate the system's ability to automatically scale out (expand) and scale in (shrink), ensuring cost optimization and High Availability (HA).

### Tasks to be Deployed This Week:
| Day | Task Description | Start Date | End Date | Resource Links |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6 | - Researched and configured dynamic Auto Scaling Policies triggered by AWS CloudWatch alarm thresholds (e.g., CPU Utilization > 70%). | 15/05/2026 | 15 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Installed the `stress` tool on EC2 instances; defined testing scenarios and initiated CPU stress simulation to test the Scale-out feature. | 18/05/2026 | 18/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Monitored, verified, and evaluated the system's capacity to automatically launch new instances under heavy load; inspected ASG activity logs. | 19/05/2026 | 19/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Terminated the stress simulation; monitored and verified the automatic reduction (Scale-in) feature to remove redundant instances. | 20/05/2026 | 20/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - **Hands-on Practice:** <br>Verified the accuracy of the cooldown timer; confirmed the system automatically scaled back down to its Desired capacity, and consolidated testing metrics. | 21/05/2026 | 21/05/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Key Results Achieved in Week 5:

* Mastered core concepts and workflows of dynamic auto-scaling on AWS:
  * Successfully configured metric-based CloudWatch alarm thresholds and seamlessly linked them to the Auto Scaling Group (ASG).
  * Acquired a deep understanding of core sizing parameters: Minimum, Maximum, and Desired capacity.

* Demonstrated proficiency in workload simulation and Scale-out validation:
  * Utilized the `stress` tool effectively on EC2 instances to drive CPU utilization beyond the defined alarm thresholds per the test cases.
  * Verified that the system accurately detected CloudWatch alarms and successfully executed the Scale-out process (provisioning new EC2 instances) to sustain system performance.

* Validated cost optimization via the automatic Scale-in mechanism:
  * Confirmed that the ASG correctly identified the load reduction after terminating the simulation, properly triggering the cooldown period countdown.
  * Ensured the Scale-in feature functioned flawlessly; redundant EC2 instances were safely terminated to restore the infrastructure to its initial desired state, significantly optimizing resource costs.

* Completed performance evaluation and technical documentation:
  * Consolidated testing metrics, evaluated overall scaling efficiency, and finalized operational documentation for architecting High Availability (HA) systems.
  * Completed the Week 5 progress report for the AWS FCAJ course on schedule.