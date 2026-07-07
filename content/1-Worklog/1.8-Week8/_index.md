---
title: "Worklog Week 8"
date: 2026-06-11
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 Objectives:

* Understand core concepts and implementation workflows for Continuous Integration and Continuous Deployment (CI/CD) within the AWS cloud environment.
* Research and practice orchestrating AWS CodePipeline, AWS CodeBuild, and AWS CodeDeploy to completely automate software compilation, packaging, and deployment stages, achieving zero-downtime application updates.

### Tasks to be Deployed This Week:
| Day | Task Description | Start Date | End Date | Resource Links |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 6 | - Explored theoretical foundations of CI/CD pipelines; researched scheduling and automating software release lifecycles on AWS. | 05/06/2026 | 05/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Studied AWS CodeBuild services; authored `buildspec.yml` configuration files to automate source code compilation and software packaging. | 08/06/2026 | 08/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Examined AWS CodeDeploy capabilities; authored `appspec.yml` files and studied safe deployment strategies (In-place, Blue/Green). | 09/06/2026 | 09/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - **Hands-on Practice:** <br>Configured AWS CodePipeline to stitch together multiple stages (Source, Build, Deploy) into a fully automated delivery workflow. | 10/06/2026 | 10/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - **Hands-on Practice:** <br>Committed code changes to trigger the pipeline automatically; verified zero-downtime deployment features and finalized the report. | 11/06/2026 | 11/06/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Key Results Achieved in Week 8:

* Mastered architectural mindsets for building automated software release pipelines:
  * Acquired a thorough comprehension of each stage within a standard cloud-native CI/CD model and the advantages of automating deployment testing frameworks.
  * Distinctly understood the individual responsibilities and integration workflows between CodeBuild (CI), CodeDeploy (CD), and CodePipeline (Orchestrator).

* Gained proficiency in automated compilation and artifact packaging via AWS CodeBuild:
  * Successfully authored and optimized a production-ready `buildspec.yml` file to declare execution environments, install runtime dependencies, and output artifacts ready for deployment.

* Managed secure application delivery execution via AWS CodeDeploy:
  * Configured `appspec.yml` parameters accurately to govern application deployment lifecycle hooks on targeted compute infrastructure (EC2/ECS).
  * Evaluated and incorporated sophisticated deployment strategies aimed at maintaining uninterrupted system availability (Zero-downtime deployment).

* Successfully constructed and validated an End-to-End CI/CD Pipeline:
  * Established a functional AWS CodePipeline instance triggered instantly upon a developer performing a `git push` to the code repository.
  * Monitored the seamless progression through all pipeline execution stages, verifying that the live environment updated without requiring any manual intervention.
  * Completed the Week 8 progress report for the AWS FCAJ course on schedule.
