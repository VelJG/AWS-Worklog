---
title: "Week 10 Worklog"
date: "2025-09-09"
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---
{{% notice warning %}} 
⚠️ **Note:** The following information is for reference purposes only. Please **do not copy verbatim** for your own report, including this warning.
{{% /notice %}}


### Week 10 Objectives:
* Fully research and test all of the components and ready to add together to build the workshop

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Assisted in building ETL Pipeline for CloudWatch logs with team member <br> -  Updated proposal:<br>&emsp; + Included updated Architecture and Services <br>&emsp; + Recalculated prices | 10/11/2025 | 10/11/2025      ||
| 3   | - Finished building ETL Pipeline for CloudWatch logs <br> - Fixed ETL Pipeline for CloudTrail logs: Processed logs from different dates cause schema error due to randomized field order in struct data type <br> - Successfully used AWS SSM to get EC2 info after IR Responses <br> - Succesfully intergrated threat notification chatbots in Slack and Telegram <br> - Successfully shown formatted notifications based on live threat findings <br> Got sent over 1000 mails because team member triggered all GuardDuty sample findings combined with multiple test SNS <br> - Team member suggested adding SES (Simple Email Service) to format emails and send| 11/11/2025 | 11/11/2025 ||
| 4   |- Did research into CloudTrail Lake: Good for future usage specifically for in-depth CloudTrail log analysis, deemed unnecessary for current project due to it being CloudTrail exclusive <br> - Updated CloudTrail ETL Lambda: promoted fields in request parameters into collumns for better query and less schema crawling errors => Reliably crawled proccessed data between days <br> - Team members started on designing dashboard site, suggested intergrating Grafana <br> - Got started on updating proposal to the new format| 08/13/2025 | 08/13/2025      ||
| 5   | | 08/14/2025 | 08/15/2025      ||
| 6   | | 08/15/2025 | 08/15/2025      ||


### Week 10 Achievements:

