---
title: "Week 3 Worklog"
date: "2025-09-22"
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives:

* Complete Module 5
* Help teammates with previous labs
* Redo the labs that are unvailable with free tiers
* Do 2 additional research
* Discuss project idea

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   |- Lab 25: Cannot be done for now, account is on free tier <br> - Upgraded account <br> - Retry lab 25: <br>&emsp; + The given template used runtime nodejs12.x for Lambda functions, which is no longer supported, fixed it by changing it to nodejs20.x <br>&emsp; + Created Fsx file system <br>&emsp; + The S3 bucket endpoint for testing data is only reachable in the US region, so it must be changed to Read-S3Object -BucketName nasanex -KeyPrefix /AVHRR -Folder Z:/nasanex/AVHRR -Region us-west-2 <br>&emsp; + Created file shares <br>&emsp; + Created HDD and SSD Fsx <br>&emsp; + 25.4: The given tool version is outdated, downloaded latest version <br>&emsp; + Successfully tested drive performance with various parameters <br>&emsp; + Monitored performance using CloudWatch: Alarm got triggered, throughput was maxed at  400mb <br>&emsp; + Learnt how to deduplicate file:<br>&emsp;&emsp; • Default dedup schedule is every Saturday <br>&emsp;&emsp; • Initial dedup run optimized nothing due to the default fileAge -> changed to 0 => Optimized half of the files <br>&emsp; + Created shadow copies for backup <br>&emsp; + Learnt how to manage open files and how to close them from the connection <br>&emsp; + Successfully created user quotas to manage storage space <br>&emsp; + Enabled Continuously Available (CA) file share on Amazon FSx to be used by mutiple user at the same time <br>&emsp; + Scaled throughput and storage on AWS Console <br> - Learnt shared responsibility model: Both the provider and the customer have responsibility in security <br> - Module 5-2: Best pratice is to create an admin IAM user rather than using root account <br> - IAM Principal: Access resources in AWS Account <br> - IAM Policy: Identity based and Resource based <br> - IAM Role: A set of rules that control access to resources and services for IAM User <br> - IAM Role can be used to enable cross account | 22/09/2025 | 22/09/2025      | [Lab25](https://000025.awsstudygroup.com/1-introduce/)|
| 3   | - Module 5: <br>- Amazon Cognito: A authentication, permission and user management service, with two main feature: <br>&emsp; + User pool: A collection of user accounts and authentication informations, allowing for 3rd party authentication services <br>&emsp; + Identity pools: A mapping of permissions and credentials that can be applied to users <br> - AWS Organization: Manage many AWS Accounts and resources <br>&emsp; + Organizes accounts by OU and use Service Control Policies to define permissions for user on the organization <br> AWS Identity Center(SSO): Manage AWS Authorizations and Applications: <br>&emsp; + Utilize permission sets <br> - AWS KMS: Create and manage encryption keys: <br>&emsp; + CMK (Customer Managed Key) is the main resource, used to create, encrypt and decrypt Data Key <br> - AWS Security Hub: Scan and test security based and policies and best practices <br>- Continue with lab 14: <br>&emsp; + Created role and S3 Bucket <br>&emsp; + The latest Ubuntu version (25.04) included unsupported kernel version, required reinstallation to proceed <br>&emsp; + Installing Ubutun 24.04: Failed, its kernel is still unsupported <br>&emsp; + Installing Ubuntu 22.04 <br>&emsp; + Successfully imported VM to AWS <br>&emsp; + Successfully connected to EC2 instance created from the AMI using VM's username and password    | 23/09/2025 | 23/09/2025      | |
| 4   | Continue with lab 14: <br>&emsp; + Created export bucket, configured permission <br>&emsp; + Successfully exported instances into .OVA format for usage <br>- Lab 18: Enabled Security Hub and configured AWS Config to record data for analyzing (It can take a long for a score to be calculated) | 24/09/2025 | 24/09/2025      | |
| 5   | - Lab 22: <br>&emsp; + Created Lambda functions for running and stopping EC2 instance based on schedules and tags <br>&emsp; + Logged notification via Slack <br> - Lab 28:<br>&emsp; + Created IAM policies and role, only allowing access from Singapore Region(ap-southeast-1) <br>&emsp; + Restricted access to EC2 from regions outside of policy <br>&emsp; + Restricted creation of EC2 instances without valid tags <br> Lab 30: Restricted IAM user to only use the specified region to access EC2 <br> - Lab 18 (Update): Security finished scanning, got a security score of 85%, 1 critical exposure: IAM User have administrative access policy <br>- Lab 33: <br>&emsp; + Created Key Management Service <br>&emsp; + Setted up Cloudtrail to log data in S3 Bucket <br>&emsp; + Created Athena to query logs <br>&emsp; + KMS successfully denied access to users without authorization   | 25/09/2025 | 25/09/2025      | |
| 6   | - Lab 44: Configured role conditions, restricting access by IP, Time and others <br> - Lab 48:<br>&emsp; + Used IAM access key to upload file to S3 via EC2 Instance <br>&emsp; + Uploaded file to S3 via EC2 Instance without access key by using IAM Roles <br> - Lab 12: <br>&emsp; + Created AWS Organization <br>&emsp; + Created accounts and move them into units <br>&emsp; + Invited accounts to organization <br>&emsp; + Switched roles for accounts under the organization <br>&emsp; + Setted up policies for the accounts under the organization <br>&emsp; + Installed Python to continue with the lab <br>&emsp; + Created and configured users and groups using Identity Store APIs via AWS CLI <br> Labs from AWS for Microsoft Workloads: <br>&emsp; + Managed user and group on Microsoft AD via AWS CLI <br>&emsp; + Learnt how to troubleshoot EC2 instances by detaching the volumes of the errorus instance and attach it to another running instance to configure and fix the problems <br>&emsp; + Learnt how to attach licenses to EC2 instances with Microsoft AD, tried with Microsoft Office  | 26/09/2025 | 26/09/2025      |https://www.youtube.com/playlist?list=PLhr1KZpdzukdJllxulUM7pMB7aJ2_FfTP  |


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
