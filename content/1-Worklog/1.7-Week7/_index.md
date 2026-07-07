---
title: "Worklog Week 7"
date: 2026-06-04
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives:

* Learn foundational containerization concepts using Docker (Containers, Images, Dockerfiles) and cloud registry management via Amazon ECR.
* Study the architecture and cluster management mechanisms of Amazon ECS, and conduct hands-on labs to containerize an application, push it to ECR, and deploy it live on Amazon ECS.

### Tasks to be Deployed This Week:
| Day | Task Description | Start Date | End Date | Resource Links |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 5 | - Researched core Docker concepts (Containers, Images, Dockerfiles); created sample Dockerfiles to containerize applications. | 29/05/2026 | 29/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Studied Amazon ECR services; performed hands-on creation of Private Repositories and managed Docker images. | 01/06/2026 | 01/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Explored foundational concepts and architectural components of Amazon ECS (Clusters, Task Definitions, Services, Fargate/EC2 launch types). | 02/06/2026 | 02/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - **Hands-on Practice:** <br>Containerized a complete web application into a Docker image, tagged, and pushed the image to Amazon ECR. | 03/06/2026 | 03/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - **Hands-on Practice:** <br>Deployed and executed the web application on Amazon ECS infrastructure using the ECR image; finalized technical docs and submitted the report. | 04/06/2026 | 04/06/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Key Results Achieved in Week 7:

* Mastered basic containerization technologies with Docker:
  * Acquired a clear understanding of the operational differences between Docker Images and Docker Containers.
  * Successfully authored optimized Dockerfiles to containerize web applications with efficient multi-layer structures.

* Gained proficiency in cloud-based image storage and registry management:
  * Successfully provisioned Private Repositories on Amazon ECR.
  * Utilized AWS CLI seamlessly to authenticate, tag, and push local Docker images to Amazon ECR securely.

* Comprehended Amazon ECS architecture and application deployment workflows:
  * Clearly distinguished key components within the ECS ecosystem: Task Definitions (blueprints), Tasks (running instances), Services (task controllers), and Clusters.
  * Grasped the structural differences, use cases, and trade-offs between the EC2 and AWS Fargate (Serverless) launch types.

* Executed production-ready deployments and completed reporting:
  * Successfully launched and verified the live web application on ECS infrastructure, ensuring stable access via public endpoints.
  * Finalized container operations documentation and submitted the Week 7 progress report for the AWS FCAJ course on schedule.