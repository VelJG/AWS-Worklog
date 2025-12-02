---
title: "Week 13 Worklog"
date: "2025-12-01"
weight: 2
chapter: false
pre: " <b> 1.13. </b> "
---
### Week 13 Objectives:
Complete the project and submit
### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Removed Map State in Steps Function <br> - Created Lambdas to add policies to EC2 Instance for SSM automation in IR Step Functions <br> - Reconfigured Quarantine SG: Added Outbound rule for HTTPS for SSM connection <br> - Replaced Lambdas with Step Functions provided States: Used DescribeIamInstanceProfileAssociation, AttachRolePolicy, DetachRolePolicy and StartAutomationExecution <br> - CDK: Created EventBridge and Topics with subscription emails stored in cdk-context <br> - Team meetings: Planned and reassigned task to meet the new deadline | 01/12/2025 | 01/12/2025      |[CDK Tutorial](https://docs.aws.amazon.com/cdk/v2/guide/hello-world.html)|
| 3   | - CDK: Added SES alert for GuardDuty findings <br> - CDK: Added ENI ETL into ETL Pipeline <br> - Assisted in upgrading dashboard <br> Updated Event Participated and overall Worklog update fix and improvement <br> - Researched more on how to optimize pipeline, currently the S3 Get Request is higher than expected do to Athena query low size but many objects | 02/12/2025 | 02/12/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | | 03/12/2025 | 03/12/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | | 04/12/2025 | 04/12/2025      |  |
| 6   | | 05/12/2025 | 05/12/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 12 Achievements:

* Understood what AWS is and mastered the basic service groups: 
  * Compute
  * Storage
  * Networking 
  * Database
  * ...

* Successfully created and configured an AWS Free Tier account.

* Became familiar with the AWS Management Console and learned how to find, access, and use services via the web interface.

* Installed and configured AWS CLI on the computer, including:
  * Access Key
  * Secret Key
  * Default Region
  * ...

* Used AWS CLI to perform basic operations such as:

  * Check account & configuration information
  * Retrieve the list of regions
  * View EC2 service
  * Create and manage key pairs
  * Check information about running services
  * ...

* Acquired the ability to connect between the web interface and CLI to manage AWS resources in parallel.
* ...
