---
title: "Week 4 Worklog"
date: "2025-09-09"
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---



### Week 4 Objectives:


### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   |- Module 6: Database Concept review: &emsp; + Database &emsp; + Session &emsp; + Primary/Foreign Key&emsp; + Index &emsp; + Partitions &emsp; + Execution/Query Plan &emsp; + Log & Buffer &emsp; + RDBMS (Relational Database Manangement System) &emsp; + NOSQL <br> ![Database](/images/1-Worklog/Database.png) &emsp; + OLTP(Online Transaction Processing): For payments, transactions &emsp; + OLAP (Online Analytical Processing): Analyze data, predict trends and patterns <br> - AWS RDS (Relational Database Serive): Include Aurora, MySQL, Postgres SQL , MSSQL, Oracle , Maria &emsp; + Automatic backup &emsp; + Generate read replica &emsp; +Read replica can be turned into primary code &emsp; + Auto Fail Over/Multi AZ (Backups on mutiple AZs) &emsp; + Commonly used for OLTP &emsp; + Encrypt data while at rest/in transit &emsp; + Protected my Security Group and NACL &emsp; + Can change instance size &emsp; + Storage Auto SCaling <br> - Amazon Aurora: Optimized underlying storage infrastructure, uses MySQL and PostgreSQL &emsp; + Back track: revert to previous state &emsp; + Clone &emsp; + Global Database (Multi Region) &emsp; + Multi Master: Many Master Databases <br> - Amazon Redshift: Data warehouse service: PostgreSQL core, optimized for OLAP &emsp; + Uses MMP Database: data is partitioned and saved at computer nodes, a Leader node is used to coordinate and compile queries &emsp; + Stores data in a columnar storage format, useful for OLAP applications <br> ![Columnar](/images/1-Worklog/Columnar.png) &emsp; + Uses SQL and drivers like JDBC and ODBC &emsp; + Provide cost effective services (Transient Cluster/ Redshift spectrum) <br> - Amazon ElastiCache: Creates Cluster Caching Engines (Redis/Memcached) &emsp; + Detects and replaces failed nodes &emsp; + Put before CSDL layer in order to cache data &emsp; + Recommended to use Redis for new workloads &emsp; + Using ElastiCache requires caching logic on applications, not recommended to use default system caching <br> - Formulated a proposal for workshop with teammates  | 08/11/2025 | 08/11/2025      |
| 3   |- Lab 43: Guide is broken, the link doesnt go anywhere, going by video &emsp; + Downloaded Schema Conversion Tool &emsp; + Downloaded MSSQL in EC2 Instance &emsp; + No SQL script was given, trying with custom basic MSSQL Database &emsp; + No CloudFormation Stack was given, skipping Oracle Database connection &emsp; + Installed MySQL on EC2 Instance &emsp; + Migrated custom MSSQL Database to MySQL Database using AWS Schema Conversion Tool &emsp; + Created custom RDS to test migration task &emsp; + Attempted to migrate from local machine to RDS &emsp; + Tried to use AWS Replication Agent: Unsuccessful due to it being made for Window/Linux server only, not OS &emsp; + Tried to portforward PC to be used as an endpoint &emsp; + Failed portforwarding, skipping this step for now &emsp; +   | 08/12/2025 | 08/12/2025      | https://docs.aws.amazon.com/mgn/latest/ug/what-is-application-migration-service.html |
| 4   |- Found out AWS account's credits are all expired from doing lab 12 <br> - Wrote a support case <br> - Stopping labs for now <br> - Focus on research about team's proposal| 08/13/2025 | 08/13/2025      | <https://cloudjourney.awsstudygroup.com/> |
| 5   |- Continued doing labs by aquiring help from team member: Created an IAM User with admin privilege for me to log in and use their account <br> - Lab 35: <br> - Translate first blog| 2/10/2025 | 2/10/2025      | https://aws.amazon.com/blogs/apn/achieve-excellence-in-aftermarket-service-with-syncron-and-aws/ |
| 6   |- Joined the AI-Driven Development Life Cycle: Reimagining Software Engineering event <br> - Translate second and third blog| 08/15/2025 | 08/15/2025      | <https://cloudjourney.awsstudygroup.com/> |


### Week 4 Achievements:

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
