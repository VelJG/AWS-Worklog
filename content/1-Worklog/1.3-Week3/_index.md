---
title: "Week 3 Worklog"
date: "2025-09-22"
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:

* Complete Module 5
* Do 2 additional research
* Discuss project idea

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   |- Lab 25: Cannot be done for now, account is on free tier <br> - Upgraded account <br> - Retry lab 25: <br>&emsp; + The given template used runtime nodejs12.x for Lambda functions, which is no longer supported, fixed it by changing it to nodejs20.x <br>&emsp; + Created Fsx file system <br>&emsp; + The S3 bucket endpoint for testing data is only reachable in the US region, so it must be changed to Read-S3Object -BucketName nasanex -KeyPrefix /AVHRR -Folder Z:/nasanex/AVHRR -Region us-west-2 <br>&emsp; + Created file shares <br>&emsp; + Created HDD and SSD Fsx <br>&emsp; + 25.4: The given tool version is outdated, downloaded latest version <br>&emsp; + Successfully tested drive performance with various parameters <br>&emsp; + Monitored performance using CloudWatch: Alarm got triggered, throughput was maxed at  400mb <br>&emsp; + Learnt how to deduplicate file:<br>&emsp;&emsp; • Default dedup schedule is every Saturday <br>&emsp;&emsp; • Initial dedup run optimized nothing due to the default fileAge -> changed to 0 => Optimized half of the files <br>&emsp; + Created shadow copies for backup <br>&emsp; + Learnt how to manage open files and how to close them from the connection <br>&emsp; + Successfully created user quotas to manage storage space <br>&emsp; + Enabled Continuously Available (CA) file share on Amazon FSx to be used by mutiple user at the same time <br>&emsp; + Scaled throughput and storage on AWS Console <br> - Learnt shared responsibility model: Both the provider and the customer have responsibility in security | 08/11/2025 | 08/11/2025      | [Lab25](https://000025.awsstudygroup.com/1-introduce/)|
| 3   | | 08/12/2025 | 08/12/2025      | |
| 4   | | 08/13/2025 | 08/13/2025      | |
| 5   | | 08/14/2025 | 08/15/2025      | |
| 6   | | 08/15/2025 | 08/15/2025      | |


### Week 3 Achievements:

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
