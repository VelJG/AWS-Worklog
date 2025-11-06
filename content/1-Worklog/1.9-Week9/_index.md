---
title: "Week 9 Worklog"
date: "2025-09-09"
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---
### Week 9 Objectives:

* Connect and get acquainted with members of First Cloud Journey.
* Understand basic AWS services, how to use the console & CLI.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - AWS Architecture revised: <br>&emsp; + Removed AWS Detective <br>&emsp; + Updated with Step Function Workflow instead of a singular AWS Lambda Function <br>&emsp; + Added Custom Dashboard: A static custom dashboard website hosted with S3 and use Athena to query from data lake <br> - School subject: <br> &emsp; + KS57: Completed Quản trị dự án và duy trì đổi mới trong chuyển đổi số  | 03/11/2025 | 03/11/2025 | [Quản trị dự án và duy trì đổi mới trong chuyển đổi số](https://www.coursera.org/account/accomplishments/verify/IC06JCSZ7AVG) |
| 3   | - Successfully exported Guard Duty Findings to S3 Bucket <br> - Experimented with AWS Glue Crawler: <br>&emsp; + Failed on Cloudwatch and CloudTrail logs, schema too complicated for Crawler (Have to research on an alternative way) <br>&emsp; + Ran succesfully on exported Guard Duty Findings: Had to update KMS Policy to allow Crawler to decrypt data <br> - Researching ETL Pipeline for logs| 04/11/2025 | 04/11/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Team meetings: Progress report: <br>&emsp; + IR Workflow: Halfway done, EC2 quarantine function is finished, not tested with findings yet <br>&emsp; + Assigned task for dashboard frontend design <br>&emsp; + Assigned task for Glue ETL Pipeline research <br>&emsp; + Signed up for VPBank Cloud Day 2025 with team members |
| 5   |- Team meetings <br> - Researched on ETL Pipeline approach: <br>&emsp; + Instead of using Glue ELT Jobs, we use custom Lambda ELT pipeline for CloudTrail and CloudWatch  logs <br>&emsp; + Store raw logs into a Raw Log S3 Bucket then use ETL Lambda to process the data and write it to a Proccesed Data S3 to then be Crawled <br> - AWS Architecture revised: Added a new group: DATA PREP group which contain the Raw Log S3 Bucket and the ETL Lambda <br>- School subject: <br> &emsp; + ENW493c: Completed Advanced Writing | 06/11/2025 | 06/11/2025      | [Advanced Writing](https://www.coursera.org/account/accomplishments/verify/EDQ1NY2UG063) |
| 6   || 07/11/2025 | 07/11/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 9 Achievements:

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
