---
title: "Week 1 Worklog"
date: "2025-09-09"
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---

### Week 1 Objectives:

* Connect with FCJ members and mentors.
* Find out what working in an office is like.
* Install Linux, learn how to properly use Linux.
* Learn the basics of AWS, console and CLI.
* Complete first and second module.


### Tasks to be carried out this week:
| Day |Task| Start Date | Completion Date | Reference Material |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| Mon   | - Read internship rules <br> - Create AWS account <br>  - Learnt what AWS is <br>- Module 1 Lab 1 Done (Learnt how to create AWS account and manage user groups) <br>- Module 1 Lab 7 Done (Learnt how to create budgets of using the service) <br>- Lab 7-3 (Usage Budget) cannot be done, error in usage type dropdown, showing nothing <br>- Module 1 Lab 9 Done (Learnt about AWS Support Services, Its type, benefits and how to request supports) | 08/09/2025 | 08/09/2025 | [Create new AWS Account](https://000001.awsstudygroup.com/1-create-new-aws-account/) <br><br> [MFA for AWS Accounts](https://000001.awsstudygroup.com/2-mfa-setup-for-aws-user-root/) <br><br> [Create Admin Group and Admin User](https://000001.awsstudygroup.com/3-create-admin-user-and-group/) <br><br> [Account Authentication Support](https://000001.awsstudygroup.com/4-verify-new-account/) <br><br> [Explore and Configure AWS Management Console](https://000001.awsstudygroup.com/5-explore-and-configure-the-aws-management-console/) <br><br> [Creating Support Cases and Case Management in AWS](https://000001.awsstudygroup.com/6-support-cases/) |
| Tue   | - Get started on Module 2 theory: <br>&nbsp; + Learnt about VPC (Amazon Virtual Private Cloud)<br>&nbsp; + Learnt about Subnets and Routetable, Security Groups<br>&nbsp; + Learnt about ENI and EIP<br>&nbsp; + Learnt about VPC Peering and Transit Gateway <br>&nbsp; + Learnt about Elastic Load Balancing<br>&nbsp; + Learnt about EC2<br> - Setup site for workshop report <br> - Installed Hugo <br> - Successfully write worklog using markdown and Hugo | 09/09/2025 | 09/09/2025 | <https://cloudjourney.awsstudygroup.com/> |
| Wed   | - Complete Module 2's labs <br> - Lab 3: <br>&nbsp; + Learnt about the resources necessary to create and run EC2 instances <br>&nbsp; + Successfully configured and run EC2 instances <br>&nbsp; + Successfully connect and ping to EC2 instances <br>&nbsp; + Created NAT Gateway to allow private EC2 connections <br> - Lab 10: <br>&nbsp; + Learnt how to create and use keypair for security <br>&nbsp; + Learnt how to configure security group to manage connections <br>&nbsp; + Successfully connect and use RDP via EC2 <br>&nbsp; + Set up hybrid DNS with Route 53 Resolver (In progress, Cloud Formation template didn't create security group to proceed with the lab) <br> - Lab 19: <br>&nbsp; + Successfully created VPC Peering Connection <br> &nbsp; + Learnt how to configure Network ACLs <br> &nbsp; + Enabled Cross-Peer DNS to resolve private host names <br> - Downloaded and used MobaXTerm to connect to EC2 instances <br> - Downloaded and used Putty to configures keypairs    | 10/09/2025 | 11/09/2025 | <https://cloudjourney.awsstudygroup.com/> |
| Thu   | - Lab 20: <br>&nbsp; + Successfully created AWS Transit Gateway to allow for connection between VPCs via a common hub <br>&nbsp;&nbsp; * The Cloud Formation template yaml file isnt up to date, creation failed <br>&nbsp;&nbsp; * Fixed template file, changed EC2 instance type to t3.micro <br> - Learnt the hard way why you need to clean up resources after a lab, got charged 12$ credits <br> - Verified the cost and budget plans worked as intended, notified over email | 11/09/2025 | 11/09/2025 | <https://cloudjourney.awsstudygroup.com/> |
| Fri   | - Get started on Module 3 theory <br> - Lab 13 <br> - Lab 24 <br> - Lab 57| 12/09/2025 | 12/09/2025 | <https://cloudjourney.awsstudygroup.com/> |


### Week 1 Achievements:

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
