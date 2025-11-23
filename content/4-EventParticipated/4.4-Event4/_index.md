---
title: "Event 4"
date: "2025-11-17"
weight: 1
chapter: false
pre: " <b> 4.4. </b> "
---

# Summary Report: “AWS Cloud Mastery Series #2 - DevOps on AWS”

### Event Objectives

- Introduce AWS DevOps Services – CI/CD Pipeline
- Introduce Infrastructure as Code (IaC) and related tools
- Introduce Container Services on AWS
- Ensure Monitoring and Observability capabilitiy using AWS Services

### Speakers

- **Truong Quang Tinh** – AWS Community Builder, Platform Engineer - TymeX
- **Bao Huynh** – AWS Community Builder
- **Nguyen Khanh Phuc Thinh** – AWS Community Builder
- **Tran Dai Vi** – AWS Community Builder
- **Huynh Hoang Long** – AWS Community Builder
- **Pham Hoang Quy** – AWS Community Builder
- **Nghiem Le** – AWS Community Builder
- **Dinh Le Hoang Anh** - Cloud Engineer Trainee, First Cloud AI Journey

### Key Highlights

## DevOps Mindset

**- Culture:** Collaboration, Automation, Continuous Learning and Measurement
**- DevOps Roles:** DevOps Engineer, Cloud Engineer, Platform Engineer, Site Reliability Engineer
**- Success Metrics:**
    + Ensure deployment health
    + Improve agility
    + System stability
    + Optimize customer Experience
    + Justify techonology investments

| DO | DON'T |
| :--- | :--- |
| Start with Fundamentals | Stay in Tutorial Hell |
| Learn by Building Real Projects | Copy-paste blindly |
| Document Everything | Compare Your Progress to Others |
| Master one thing at a time | Give Up After Failures |
| Soft Skills Enhancement | |

**- Continuous Integration:** Team members integrate their work frequently, aims for continous Delivery and  Deployement

## Infastructure as Code (IaC)

**-Benefits:** Automation, Scalabililty, Reproductibility and better Collaboration

# AWS CloudFormation

AWS's own built in IaC tool, use templates written with YAML or JSON, can build every AWS Infastructure automatically

**- Stack:** A set of AWS Resources defined in a template, can be used by CloudFormation to create, update or delete said resources

**- CloudFormation Template:** A YAML/JSON file that define an AWS Infastructure, act like a blueprint to deploy and configure resources

**- How it works:** Create template -> Store in S3 Bucket or Local storage -> Use CloudFormation to create Stacks based on template -> CloudFormation built resources 

**- Drift Detection:** Detect changes in the infastructure compared to the Stack => Update Stack or revert change, useful for versioning 

# AWS Cloud Development Kit(CDK)

Open-source software development framework, support IaC using real programming languages(Python,Java,C#.Net, Type/JavaScript and Go)

**- Construct:** Building blocks, comprised of components that represent AWS Resources and their Configuration, have 3 construct level:
  + L1 Construct: Low-level resources maps directly to a single AWS CloudFormation resource
  + L2 Construct: Provide a higher-level abstraction through an intuitive intent-based API,encapsulate best practices and security defaults 
  + L3 Construct: Complete architecture patterns with multiple resources, opinionated implementation and fast deployment

# AWS Amplify

AWS platform that makes it easy to build, deploy, and scale web and mobile apps, uses CloudFormation under the hood: Stacks deployed to built infastructure programmatically 

# Terraform

IaC tool, start by defining infastructure in Terraform code and plan then apply the infastructure on multiple cloud platforms like Azura, AWS, Google Cloud, etc..

**- Strength:** Multi-Cloud support, State tracking with the same configuration

# How to choose IaC Tools?
**-Criteria:**
  + Plan using one Cloud or many?
  + Role as Developer or Ops?
  + Does the Cloud and Ecosystem support the tool?

## Container Services on AWS

# Dockerfile

A Dockerfile defines how to build a container image, which describe the environment, dependencies, build steps, and final runtime configuration, ensuring that the application run consistently across any system that support Dockers

**- Images:** A packaged blueprint of an application, build from a Dockerfile using layered file system, used to create containers consistently across environments

**- Workflow:** Dockerfile build a Docker Image which can be used to run Container and push to ECR/Docker Hub

# Amazon ECR

A fully managed container registry that make it easy to store, manage, and securely share Docker container image.
AWS's own secure and scalable private container registry

**-Features:** 
  + Image Scanning
  + Immutable Tags
  + Lifecycle Policies
  + Encryption & IAM

**- Orchestration:** Orchestrate many containers processes: restart containers, scale up automatically under high load, distribute traffic efficiently, manage where containers are placed and run

# Kubernetes
Open source, automates deployment, scaling, healing, and load balancing
**- Components:**
  + Master Node: Control Plane, manage worker nodes and pods
  + Worker Node: Run application workloads inside pods
  + Pod: Smallest deployable unit, can contain one or more containers
  + Service

ECS vs EKS

# App Runner

Suitable for quick deployment of web applications and REST APIS, ideal for small to medium production workload

## Monitoring & Observability

# CloudWatch
- Monitor AWS Resources and Apllications running on AWS in real time
- Provide observabilty
- Alarms and automated responses
- Dashboard to help with operational and cost optimization

### Event Experience

#### Some event photos
![Group picture during the event](/images/4-Event/TheBois-AIDLC.jpg)