---
title: "Week 7 Worklog"
date: "2025-10-20"
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---
### Week 7 Objectives:

* Connect and get acquainted with members of First Cloud Journey.
* Understand basic AWS services, how to use the console & CLI.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Learnt the basics of Guard Duty with "Getting Hands on with Amazon GuardDuty - AWS Virtual Workshop" <br> - Got familiarized with Guard Duty by using Amazon Q to generate a basic lab: <br> &emsp; + Created sample finding via setting <br> &emsp; + Learnt the finding interface <br> &emsp; + Test EC2 by port scanning scanme.nmap.org <br> &emsp; + Simulated DNS exfiltration on EC2 <br> &emsp; + GuardDuty did not alert findings from VPC Flow Logs as expected <br> &emsp; + Triggered GuardDuty findings through CloudTrail by accessing API ListPolicies with root credentials <br> - Learnt more by doing Guard Duty workshops <br> - Online team meeting: Assign members to research the services to be used in the workshop  | 20/10/2025 | 20/10/2025| [Getting Hands on with Amazon GuardDuty - AWS Virtual Workshop](https://www.youtube.com/watch?v=eq3_H-aiHhk) <br><br> [Guard Duty Workshop](https://catalog.workshops.aws/security/en-US) |
| 3   | - Succesfully triggered GuardDuty sample alerts with various severities and types via CloudShell CLI => Easier testing environment <br> - Created a custom threat list of IPs and domain names for GuardDuty via CloudShell commands although it did not work  | 21/10/2025 | 21/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Team meeting: <br> &emsp; + Quick AWS Services knowledge revision <br> &emsp; + Conversed about changes in the proposal <br> - Updated AWS Architecture: Added AWS Detective <br> - Revised proposal: <br> &emsp; + Added the usage of AWS Detective <br> &emsp; + Added plan for CDK after finishing the workshop <br> - Mentor reccommendations: <br> &emsp; + Visualize data but without using Quicksight, instead make a custom-coded dashboard (Researching) <br> &emsp; + Save GuardDuty findings in S3 bucket for analyzing (Researching) <br> - Succesfully configured EventBridge to trigger upon specific GuardDuty findings and: <br> &emsp; + Sent SNS emails to all of team members <br> &emsp; + Triggered a simple Lambda script <br> - Fomulated an idea to add to workshop: Make a simple data graphing page hosted in S3 and use API Gateway and Lambda to pull forensics data from Amazon Athena (Researching)| 22/10/2025 | 22/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Tried out AWS Card Clash with team members: Surprisingly good for learning services and their functions, their placement in Architectures <br> - Reviewed AWS Services Knowledge for Mid-Term: Using Google Gemini to generate quizzes based on the given requirements| 23/10/2025 | 23/10/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Successfully configured GuardDuty threat list to trigger findings from EC2 Instance activities | 08/15/2025 | 08/15/2025 <br> - School subject: <br> &emsp; + KS57: Completed Pháp luật và đạo đức trong công nghệ số  |[Pháp luật và đạo đức trong công nghệ số](https://www.coursera.org/account/accomplishments/verify/7JELDK2MGGKL) |


### Week 7 Achievements:

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
