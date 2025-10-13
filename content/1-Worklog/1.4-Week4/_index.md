---
title: "Week 4 Worklog"
date: "2025-09-29"
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---



### Week 4 Objectives:
- Complete Module 6
- Started on proposal

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   |- Module 6: Database Concept review: &emsp; + Database &emsp; + Session &emsp; + Primary/Foreign Key&emsp; + Index &emsp; + Partitions &emsp; + Execution/Query Plan &emsp; + Log & Buffer &emsp; + RDBMS (Relational Database Manangement System) &emsp; + NOSQL <br> ![Database](/images/1-Worklog/Database.png) &emsp; + OLTP(Online Transaction Processing): For payments, transactions &emsp; + OLAP (Online Analytical Processing): Analyze data, predict trends and patterns <br> - AWS RDS (Relational Database Serive): Include Aurora, MySQL, Postgres SQL , MSSQL, Oracle , Maria &emsp; + Automatic backup &emsp; + Generate read replica &emsp; +Read replica can be turned into primary code &emsp; + Auto Fail Over/Multi AZ (Backups on mutiple AZs) &emsp; + Commonly used for OLTP &emsp; + Encrypt data while at rest/in transit &emsp; + Protected my Security Group and NACL &emsp; + Can change instance size &emsp; + Storage Auto SCaling <br> - Amazon Aurora: Optimized underlying storage infrastructure, uses MySQL and PostgreSQL &emsp; + Back track: revert to previous state &emsp; + Clone &emsp; + Global Database (Multi Region) &emsp; + Multi Master: Many Master Databases <br> - Amazon Redshift: Data warehouse service: PostgreSQL core, optimized for OLAP &emsp; + Uses MMP Database: data is partitioned and saved at computer nodes, a Leader node is used to coordinate and compile queries &emsp; + Stores data in a columnar storage format, useful for OLAP applications <br> ![Columnar](/images/1-Worklog/Columnar.png) &emsp; + Uses SQL and drivers like JDBC and ODBC &emsp; + Provide cost effective services (Transient Cluster/ Redshift spectrum) <br> - Amazon ElastiCache: Creates Cluster Caching Engines (Redis/Memcached) &emsp; + Detects and replaces failed nodes &emsp; + Put before CSDL layer in order to cache data &emsp; + Recommended to use Redis for new workloads &emsp; + Using ElastiCache requires caching logic on applications, not recommended to use default system caching <br> - Formulated a proposal for workshop with teammates  | 29/09/2025 | 29/09/2025      |
| 3   |- Lab 43: Guide is broken, the link doesnt go anywhere, going by video &emsp; + Downloaded Schema Conversion Tool &emsp; + Downloaded MSSQL in EC2 Instance &emsp; + No SQL script was given, trying with custom basic MSSQL Database &emsp; + No CloudFormation Stack was given, skipping Oracle Database connection &emsp; + Installed MySQL on EC2 Instance &emsp; + Migrated custom MSSQL Database to MySQL Database using AWS Schema Conversion Tool &emsp; + Created custom RDS to test migration task &emsp; + Attempted to migrate from local machine to RDS &emsp; + Tried to use AWS Replication Agent: Unsuccessful due to it being made for Window/Linux server only, not OS &emsp; + Tried to portforward PC to be used as an endpoint &emsp; + Failed portforwarding, skipping this step for now &emsp; +   | 30/09/2025 | 30/09/2025      | [Lab 43](https://000043.awsstudygroup.com/) <br><br> [Application Mirgation Service Guide](https://docs.aws.amazon.com/mgn/latest/ug/what-is-application-migration-service.html) |
| 4   |- Found out AWS account's credits are all expired from doing lab 12 <br> - Wrote a support case <br> - Stopping labs for now <br> - Focus on research about team's proposal| 01/10/2025 | 01/10/2025      | |
| 5   |- Continued doing labs by aquiring help from team member: Created an IAM User with admin privilege for me to log in and use their account <br> - Translate first blog| 02/10/2025 | 02/10/2025      | [Blog 1](content/3-BlogsTranslated/3.1-Blog1/_index.md) |
| 6   |- Joined the AI-Driven Development Life Cycle: Reimagining Software Engineering event <br> - Translated second and third blog| 03/10/2025 | 04/10/2025 | [Blog 2](content/3-BlogsTranslated/3.2-Blog2/_index.md) <br><br> [Blog 3](content/3-BlogsTranslated/3.3-Blog3/_index.md) | 


### Week 4 Achievements:

* Completed a comprehensive review of core database concepts including RDBMS, keys, indexes, partitioning, OLTP/OLAP, and AWS-specific database services.

* Gained theoretical knowledge of the features and use cases for AWS RDS, Amazon Aurora (e.g., Backtrack, Global Database), Amazon Redshift (Data Warehouse for OLAP), and Amazon ElastiCache (caching with Redis/Memcached).

* Database Migration: Attempted a complex database migration lab, demonstrating resourcefulness by:

  *  Sourcing a custom MSSQL Database and installing necessary services on an EC2 instance due to broken lab guides.

  *  Successfully migrating the custom MSSQL database to MySQL using the AWS Schema Conversion Tool (SCT).

* Identified and addressed the issue of expired AWS credits by raising a support case.

* Secured continuation of lab work by setting up an IAM User with admin privileges on a team member's account.

* Formulated a proposal for the team's upcoming workshop with teammates.

* Completed the translation of three blogs.

* Attended the AI-Driven Development Life Cycle: Reimagining Software Engineering event.