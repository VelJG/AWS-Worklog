---
title: "Week 12 Worklog"
date: "2025-11-24"
weight: 2
chapter: false
pre: " <b> 1.12. </b> "
---
### Week 12 Objectives:

* Connect and get acquainted with members of First Cloud Journey.
* Understand basic AWS services, how to use the console & CLI.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Successfully installed AWS CDK with AWS CLI <br> Completed the tutorial for creating a first application with CDK: <br>&emsp; + Deployed stacks on AWS Accounts <br>&emsp; + Used diff to compare changes <br>&emsp; + Destroyed stack after finishing <br> - Created a Github Organization for the team | 08/11/2025 | 08/11/2025      |[CDK Tutorial](https://docs.aws.amazon.com/cdk/v2/guide/hello-world.html)|
| 3   | - Added to IR Step Functions: Added a Map State to illiterate isolated Instances and trigger SSM Lambda for those Instances to collect logs from them for forensics <br> - Succesfully helped with creating auto export CloudWatch logs: Used Lambda to parse subcription filter form log stream to Raw Log S3 bucket, will have to modify CloudWatch ETL Lambda to work with the new auto export rather than the batch export job <br> - Update CloudTrail ETL Lambda: Noticed the usually high storage cost in the Processed CloudTrail Log bucket => The current Lambda Function save files as unzipped .jsonl => Updated the function so that the files is compressed by gzip before saving <br> - CloudTrail ETL Lambda have some spiking and error invocations when multiple people is interacting with the account => Raised timeout limit <br> CDK: Moved the CDK testing environment to a new account <br> - CDK: Created a Stack that enables GuardDuty and CloudTrail and the Raw Log S3 Bucket   | 08/12/2025 | 08/12/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | | 08/13/2025 | 08/13/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | |
| 6   | | 08/15/2025 | 08/15/2025      | <https://cloudjourney.awsstudygroup.com/> |


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
