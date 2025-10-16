---
title: "Proposal"
date: "2025-10-16"
weight: 2
chapter: false
pre: " <b> 2. </b> "
---
# Proposal: Automated AWS Incident Response and Forensics Workshop

### 1. Executive Summary
The Automated Incident Response and Forensics Workshop is designed to provide security and operations teams with hands-on experience building an AWS-native, cost-optimized security automation pipeline. The architecture leverages Amazon GuardDuty's machine learning for detection, instantly contains threats via AWS Lambda orchestrated by Amazon EventBridge, and utilizes AWS Glue and Athena for cost-efficient forensic analysis. The system is configured for minimal operational cost, making it ideal for an enterprise pilot.

### 2. Problem Statement
#### What’s the Problem?
Traditional security operations rely on manual log review and human intervention, leading to high Mean Time To Respond (MTTR) and potentially devastating breaches. Manual incident investigation is slow and expensive due to unoptimized querying of massive log files.

#### The Solution
The proposed solution implements a complete Detection-to-Containment-to-Forensics lifecycle using serverless AWS services:
- **Detection**: Managed threat intelligence via GuardDuty eliminates the need for complex custom rule writing.
- **Orchestration**: Amazon EventBridge ensures the GuardDuty finding instantly triggers multiple response actions.
- **Containment**: Lambda is triggered by EventBridge to instantly quarantine compromised EC2 instances and disable suspicious IAM keys.
- **Forensics**: S3, Glue, and Athena form a highly cost-optimized data lake, allowing analysts to run fast, targeted SQL queries on historical logs (VPC Flow Logs, CloudTrail) to generate comprehensive incident reports.

#### Benefits and Return on Investment
- **Reduced MTTR**: Containment time drops from minutes/hours (manual) to **seconds** (automated Lambda).
- **Cost Efficiency**: AWS Glue optimizes S3 logs into partitioned, columnar data (Parquet), drastically cutting the data scanned and thus minimizing Athena query costs.
- **Security Insight**: Provides an immutable, centralized data foundation for all security investigations.
- **Monthly Costs**: Estimated minimal recurring cost of **~$10.79 USD**, demonstrating responsible cloud financial management.

### 3. Solution Architecture
The architecture implements a serverless, event-driven pipeline that covers the entire IR lifecycle.

![AWS Incident Response and Forensics Architecture](/images/2-Proposal/AWSWorkshopArchitecture.jpg)
_AWS Incident Response and Forensics Architecture_

#### AWS Services Used
| Service | Purpose in IR Lifecycle |
|---|---|
| **AWS GuardDuty** | **Detection**: Analyzes CloudTrail & VPC Flow Logs for threats, generates high-fidelity findings. |
| **Amazon EventBridge** | **Event Routing**: Receives GuardDuty findings and routes them to multiple response targets (Lambda and SNS). |
| **Main Lambda (IR Orchestrator)** | **Containment**: Executes immediate response actions (Quarantine EC2, Disable IAM Key). |
| **AWS SSM (Forensic)** | **Forensics**: Provides secure remote execution to collect evidence inside the EC2 OS. |
| **Amazon SNS** | **Alerting**: Publishes GuardDuty findings for multi-channel delivery. |
| **Notification Lambda (Alert Dispatch)** | **Custom Channel**: Translates SNS alerts into messages for a 3rd party platform (e.g., Telegram). |
| **EC2 Instance** | **Target**: The asset being monitored and quarantined. |
| **Amazon S3** | **Storage**: Immutable Data Lake for all historical log data. |
| **AWS Glue (Crawler)** | **Optimization**: Catalogs log data, enabling efficient, low-cost querying. |
| **Athena** | **Analysis**: Serverless SQL engine for querying S3 logs during forensics. |

### 4. Technical Implementation
#### Implementation Phases (6 Weeks)
The workshop focuses on deploying the automation and optimization layers over six weeks:
- **Week 1-2 (Foundation)**: Enable core logging (CloudTrail, VPC Flow Logs, EC2 logs to CloudWatch). Activate GuardDuty and monitor initial findings.
- **Week 3-4 (Automation)**: Develop and deploy the two Lambda functions (Main Logic and Notification Logic). Configure EventBridge rules to connect GuardDuty to the Lambdas and SNS. Finalize AWS SSM runbooks for forensic data collection.
- **Week 5-6 (Optimization & Launch)**: Configure AWS Glue Crawler to run weekly on S3 log data. Test complex forensic queries using Athena to validate cost-efficiency. Conduct a full simulation of an intrusion and automated response.

#### Technical Requirements
- **Detection**: GuardDuty configuration for high/medium severity findings.
- **Response Logic**: Python/Node.js SDK knowledge within Lambda to call the EC2 and IAM APIs. Configuration of EventBridge rules for event routing.
- **Forensics**: Proficiency in setting up S3 and Glue for a data lake (including partitioning) and using standard SQL queries in Athena.
- **Best Practice**: EC2 instance runs only as needed (e.g., 168 hours/month) to minimize operational costs.

### 5. Timeline & Milestones
| Timeline | Key Milestones and Achievements |
|---|---|
| **Week 1-2: Logging & Detection** | <ul><li>All foundational logging (CloudTrail, VPC Flow Logs) enabled.</li><li>Amazon GuardDuty fully enabled and generating sample findings.</li><li>Initial S3 log archiving policies created.</li></ul> |
| **Week 3-4: Automation & Alerting** | <ul><li>Main Lambda deployed and tested (Quarantine EC2 action validated).</li><li>Notification Lambda deployed and integrated with Telegram.</li><li>AWS SSM configured for secure remote forensic data collection.</li></ul> |
| **Week 5-6: Forensics & Optimization** | <ul><li>AWS Glue Crawler configured and running weekly to catalog S3 logs.</li><li>Athena queries validated against optimized log data for cost efficiency.</li><li>Full simulation of intrusion → detection → containment → forensics completed.</li></ul> |

### 6. Budget Estimation
The budget assumes a lab environment operating under a paid tier model, demonstrating cost control.

The budget estimate was calculated on [AWS Pricing Calculator](https://calculator.aws/#/estimate?id=131622a3245dca4f1c3a5b934a9dbbf210470fc9).


| Infrastructure Costs | Assumption | Cost/Month (USD) |
|---|---|---|
| EC2 Instance (t3.micro) | 168 hours/month (7 days runtime) | $2.88 |
| Amazon GuardDuty | Continuous monitoring, minimal log volume | ~$2.08 |
| AWS Glue (Crawler) | 4 weekly runs @ 15 min each | $0.44 |
| Amazon CloudWatch  | 1000 GetMetric calls | $2.34 |
| Amazon S3 | 5gb free + 3gb extra | $0.21 |
| AWS Lambda  | 1 million free requests + compute charges | $0.02 |
| Amazon Athena  | 50 queries per month and 1gb of data scanned per query | $0.24 |
| **TOTAL ESTIMATED MONTHLY COST** | | **~$8.21 USD** |
| **TOTAL ESTIMATED ANNUAL COST** | | **~$98.52 USD** |

### 7. Risk Assessment
| Risk | Impact | Probability | Mitigation Strategies |
|---|---|---|---|
| **GuardDuty Cost Spike** (Due to high event volume) | Medium | Medium | Implement strict budget alarms; utilize the 30-day Free Trial to establish a cost baseline. |
| **Logic Failure** (Lambda fails to quarantine) | High | Low | Robust error handling and logging in Lambda; Main Lambda will log failure to a Dead-Letter Queue (DLQ) for investigation and re-execution. Immediate manual intervention via the EC2 console. |
| **Unoptimized Athena Query** | Medium | Medium | Strict requirement to use AWS Glue partitioning and Parquet conversion to minimize data scanned. |

### 8. Expected Outcomes
#### Technical Improvements:
- Achieve an **Automated MTTR** (Mean Time To Respond) for EC2 quarantine measured in seconds.
- Establish an AWS-native, cost-optimized **Security Data Lake**.
- Gain hands-on expertise with key security and analysis tools: GuardDuty, Lambda, SSM, Glue, and Athena.

#### Long-term Value:
- Provides a reusable, security-hardened **reference architecture** for future production cloud environments.
- Generates a foundational dataset of security logs suitable for **AI/ML security research** (anomaly detection model training).