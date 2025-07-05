# DAY 1

1. Intro to Cloud Computing 
2. Cloud Service Models
3. Deployment Models
4. Benefits
5. Risks & Challenges
6. Use Cases
7. Cloud Providers
8. Cloud-Native Architecture
9. Security 
10. Future Trends
11. Certifications & Careers
12. Glossary


Learning and Practicing AWS

1	IAM (Identity & Access Management)
2	VPC & Networking (Subnets, NAT, IGW, SG, NACL, Route Tables)
3	EC2 & EBS (Instances, Volumes, AMIs, Auto Scaling)
4	S3 (Buckets, Storage Classes, Lifecycle, Encryption)
5	Load Balancing (ALB, NLB, Target Groups)
6	RDS & Aurora (PostgreSQL, MySQL, Backups, Replication)
7	DynamoDB (NoSQL, TTL, Streams, GSI/LSI)
8	Lambda + API Gateway (Serverless Architecture)
9	CloudWatch & CloudTrail (Monitoring, Logging, Alarms)
10	SNS, SQS, EventBridge (Notifications & Messaging)
11	Systems Manager (SSM, Parameter Store, Patch, Session)
12	CloudFormation & CDK (Infrastructure as Code)
13	ECS & Fargate (Docker Container Orchestration)
14	EKS (Kubernetes on AWS)
15	CodePipeline + CodeBuild + CodeDeploy (CI/CD DevOps)
16	Route 53 (DNS, Health Checks, Failover Routing)
17	Secrets Manager & KMS (Secrets & Encryption Keys)
18	AWS Organizations & SCPs (Multi-Account Governance)
19	Cost Optimization & Budgets (Cost Explorer, Savings Plans)
20	GuardDuty, Macie, Inspector, Detective (Security Intelligence)
21	SSO / IAM Identity Center (Enterprise Access Control)
22	Cognito (User Pools, Federated Identity)
23	Elastic Beanstalk (Managed App Deployment)
24	CloudFront & WAF (CDN & Web Security)
25	Migration & Hybrid Tools (DMS, Snow, Storage Gateway)
26	Backup, Disaster Recovery & Cross-Region Setup
27	Trusted Advisor & Well-Architected Framework
28	Analytics Stack (Athena, Glue, QuickSight, Redshift)
29	Machine Learning Stack (SageMaker, Rekognition, Comprehend)
30	IoT Core & Greengrass (IoT on AWS)

---------------------------------------------------------------------
1. IAM (Identity & Access Management)
IAM Users, Groups, Roles, and Policies
Inline vs Managed Policies
Policy Evaluation Logic (Explicit Deny, Permission Boundaries)
IAM Best Practices (MFA, Least Privilege)
STS and Temporary Credentials
IAM Policy Simulator
Resource-based vs Identity-based Policies
Service-linked Roles

2. VPC & Networking
VPC Basics (CIDR blocks, IP ranges)
Subnets (Public vs Private)
Route Tables and Route Propagation
Internet Gateway (IGW)
NAT Gateway vs NAT Instance
Network ACLs vs Security Groups
VPC Peering vs Transit Gateway
VPC Endpoints (Interface vs Gateway)
DHCP Options Sets, Elastic IPs
Bastion Hosts

3. EC2 & EBS
EC2 Instance Types & Families
Launch Templates vs Launch Configurations
EBS Volume Types (gp3, io2, etc.)
Snapshots, Backup and Restore
Elastic IP, ENI (Elastic Network Interface)
Auto Scaling Groups (ASG) and Policies
Spot Instances, Spot Fleets, Savings Plans
EC2 Placement Groups (Cluster, Spread, Partition)
AMIs: Create, Share, Use

4. S3 (Simple Storage Service)
Bucket Configuration and Access Control
Object Lifecycle Management (Transition, Expiration)
Storage Classes (Standard, IA, Glacier, Deep Archive)
Bucket Policies vs IAM Policies
S3 Versioning, Logging, and Replication
Multipart Uploads, Pre-signed URLs
S3 Encryption (SSE-S3, SSE-KMS, SSE-C)
S3 Access Points and Object Lambda

5. Load Balancing (ALB, NLB, CLB)
Classic vs Application vs Network Load Balancers
Target Groups and Health Checks
Listener Rules and Host/Path Routing (ALB)
Static IP and TLS Termination (NLB)
Integration with Auto Scaling Groups
Cross-zone Load Balancing
Sticky Sessions and Connection Draining

6. Lambda + API Gateway (Serverless)
Lambda Function Lifecycle and IAM Roles
Event Sources (S3, SNS, SQS, DynamoDB, etc.)
Lambda Layers and Extensions
API Gateway Types (HTTP vs REST vs WebSocket)
Throttling, Caching, Authorizers
Integration with VPC and Private APIs
Deployment Stages and Stage Variables
Versioning and Aliases in Lambda

7. CloudWatch & CloudTrail
CloudWatch Metrics, Logs, Alarms
Log Groups, Log Streams, Filters
CloudWatch Dashboards and Insights
CloudWatch Agent and Embedded Metric Format
CloudTrail Event Types (Management vs Data Events)
Trail Configuration (Multi-region, Organization-wide)
Integration with Lambda and EventBridge
Cost and Retention Considerations

8. SNS, SQS, EventBridge
SNS Topics (Standard vs FIFO), Subscriptions
SQS Queues (Standard vs FIFO), Dead Letter Queues
Message Retention, Visibility Timeout, Delay Queues
EventBridge Rules and Event Patterns
EventBus Types (Default, Custom, Partner)
Integration Patterns (Fan-out, Filtering)
Retry and Error Handling

9. Systems Manager (SSM)
SSM Agent and Role Setup
Session Manager (Shell Access without SSH)
Run Command, Automation Documents (SSM Documents)
Patch Manager and Maintenance Windows
Inventory and Compliance Reports
Parameter Store (Standard vs Advanced)
Secure String Parameters with KMS

10. CloudFormation & CDK
CloudFormation Template Structure (YAML/JSON)
StackSets and Nested Stacks
Change Sets and Drift Detection
Intrinsic Functions and Conditions
AWS CDK Basics (Languages, Constructs)
CDK vs CloudFormation Comparison
Custom Resources and Lambda-backed Functions
Best Practices for IaC

11. ECS & Fargate
ECS Cluster Types (EC2 vs Fargate)
Task Definitions, Services, Task Roles
Load Balancer Integration with ECS
Service Discovery with Cloud Map
Logging and Monitoring ECS
ECR: Elastic Container Registry
Blue/Green Deployments with CodeDeploy

12. EKS (Elastic Kubernetes Service)
Control Plane vs Worker Nodes
EKS Setup with eksctl / CDK
IAM Roles for Service Accounts (IRSA)
Node Groups (Managed, Self-managed, Fargate)
Networking in EKS (CNI, Security Groups, Ingress)
Helm Charts and Add-ons (CoreDNS, VPC CNI, etc.)
Monitoring with CloudWatch Container Insights

13. CodePipeline + CodeBuild + CodeDeploy
CI/CD Overview on AWS
Source Integrations (GitHub, CodeCommit)
CodeBuild Projects and Buildspec
CodeDeploy Application & Deployment Groups
Blue/Green and Canary Deployments
Artifacts Management and Encryption
Integration with Lambda/ECS/CloudFormation
Approval Steps and Notifications

14. Route 53
DNS Record Types (A, AAAA, CNAME, etc.)
Hosted Zones (Public vs Private)
Routing Policies: Simple, Failover, Latency, Weighted, Geolocation
Health Checks and Alarms
Domain Registration and Transfer
DNSSEC and TTL Management

15. Secrets Manager & KMS
Secrets Rotation and Policies
Cross-account Access to Secrets
Secrets Manager vs Parameter Store
KMS Key Types (Customer-managed, AWS-managed)
CMK vs SYK, Key Policies vs IAM Policies
Envelope Encryption, Key Grants, Aliases
Auditing with CloudTrail

16. AWS Organizations & SCPs
Organizational Units (OUs)
Account Creation and Invitations
Service Control Policies (SCP) Best Practices
Permission Guardrails and Inheritance
Consolidated Billing and Tagging
AWS Control Tower Overview
Delegated Admin Access

17. Cost Optimization & Budgets
AWS Pricing Models (On-Demand, Reserved, Spot, Savings Plans)
Cost Explorer and Cost Categories
Budgets and Alerts (Cost, Usage, RI Coverage)
Tag-based Cost Allocation
Trusted Advisor (Cost and Usage Checks)
Compute Optimizer Recommendations
Rightsizing Resources

18. GuardDuty, Macie, Inspector, Detective
GuardDuty Threat Detections
Macie for S3 Sensitive Data Discovery
Inspector for EC2 and Lambda Vulnerability Scanning
Detective for Security Investigation
Integration with Security Hub
Finding Management and Automation

19. SSO / IAM Identity Center
Identity Source Setup (AD, External IdPs, AWS Directory Service)
Permission Sets and Account Assignments
User Groups and Federation
Application SSO (SAML Integration)
Access Auditing and Credential Reports
SCIM Provisioning and Automation

------------------------------------------------------------------

🔐 1. IAM (Identity & Access Management) – Security Backbone

IAM policy evaluation logic (implicit deny, explicit allow, explicit deny)
Least privilege model implementation across environments
IAM roles for EC2, Lambda, ECS, CodeBuild
Cross-account access using IAM roles
Federation via SAML, Cognito, IAM Identity Center (SSO)
Permissions boundaries for delegation of access
Session policies for temporary credentials
Fine-grained permissions with resource-level control
Service-linked roles and use cases (ECS, CodePipeline, etc.)
IAM access analyzer for policy validation
Securing programmatic access with IAM roles and MFA

🌐 2. VPC & Networking – Foundation of Architecture

CIDR design for multi-AZ, multi-region VPCs (non-overlapping for peering)
Public vs private subnet design with NAT Gateway vs NAT Instance
Multi-tier network design for web, app, DB layers
Route table strategies for public/private access
VPC Peering vs AWS Transit Gateway — use cases
AWS PrivateLink vs VPC Endpoints — for secure internal services
Egress and ingress control using NACLs and Security Groups
Bastion host architecture (with Session Manager preferred)
Hybrid connectivity (VPN, Direct Connect)
IPv6 design and compliance needs
Logging with VPC Flow Logs for compliance and troubleshooting

💻 3. EC2 & EBS – Compute Backbone

Instance families and selection (cost-performance match)
Launch templates vs configurations — production ASG templates
EC2 Spot vs On-Demand vs Reserved — capacity planning
AMI design and management (base AMIs, hardening, sharing)
Elastic Network Interfaces (ENIs) and failover design
EBS performance tuning (IOPS, Throughput, EBS-Optimized)
EBS encryption using KMS and cross-region snapshot sharing
Placement groups (cluster for HPC, spread for HA)
Auto scaling policies — predictive scaling, scheduled, dynamic
EC2 lifecycle hooks and scaling lifecycle events

🪣 4. S3 – Backbone of Storage

Bucket policy design (cross-account, VPC-only access)
Pre-signed URLs vs public access — secure sharing
S3 versioning + MFA delete for critical data
Lifecycle policies — intelligent tiering, archiving, expiration
Cross-region replication (CRR) with KMS integration
S3 Access Points and Object Lambda for complex access patterns
Using S3 for static websites and CloudFront origins
Event-driven patterns (S3 → Lambda/SQS)
Logging access with Server Access Logging and CloudTrail
Encryption in transit + SSE-KMS encryption at rest
Performance tuning for large datasets (multipart upload, parallelization)

⚖️ 5. Load Balancing – High Availability Layer

ALB vs NLB vs Gateway Load Balancer: deep use-case comparison
Multi-AZ architecture using ALB with health checks
Target group designs — Lambda, EC2, IP targets
Listener rules for host/path-based routing (microservices)
SSL/TLS offloading at ALB/NLB
Authentication via Cognito or OIDC in ALB
WAF integration with ALB for security
NLB static IPs and use in hybrid environments
Cross-zone load balancing and performance impact

☁️ 6. Lambda + API Gateway – Scalable Serverless

Lambda cold start tuning, memory tuning, concurrency settings
VPC-attached Lambda and subnet planning
Event-driven integrations (SQS, SNS, DynamoDB Streams, EventBridge)
API Gateway (REST vs HTTP vs WebSocket) production configurations
Authentication & Authorization (JWT, Cognito, IAM)
API Gateway throttling, caching, WAF, request validation
Lambda layers and environment variables
Logging and X-Ray tracing
Canary deployments and safe rollouts

🔍 7. CloudWatch & CloudTrail – Observability & Auditing

Custom metrics, metric filters, and embedded metrics
Alarm configuration with SNS, Auto Scaling triggers
Dashboards for app/infrastructure monitoring
CloudWatch Agent on EC2 (logs, metrics, unified configuration)
Log retention policies and cost optimization
CloudTrail multi-region and organizational trails
CloudTrail Lake and advanced queries
Real-time alerting on unauthorized actions or misconfigurations

🔔 8. SNS, SQS, EventBridge – Messaging & Events

SQS long polling and visibility timeout tuning
FIFO queues with deduplication and sequencing
DLQs and retry strategies
EventBridge schema registry and custom event buses
Cross-account event publishing and receiving
SNS encryption with KMS, delivery to multiple protocols
Fan-out pattern (SNS → multiple Lambda/SQS targets)

🛠️ 9. Systems Manager – Infrastructure Control Plane

Session Manager: secure EC2 access without SSH
Parameter Store for secure config management (vs Secrets Manager)
Automation documents for patching, lifecycle, and remediation
Maintenance windows and patch baselines
Inventory and compliance reports (managed instances)
EC2 image builder automation via SSM
Advanced SSM features (OpsCenter, Incident Manager)

🧱 10. CloudFormation & CDK – Infrastructure as Code

Modular stack design with nested stacks
Cross-stack references and exports
Change sets, rollback triggers, and stack policies
Drift detection and auditing
CDK constructs, stacks, and apps (deep dive)
CDK Pipelines and continuous deployment
Custom resources using Lambda-backed implementations
Secret injection, dependency management in IaC

🐳 11. ECS & Fargate – Container Orchestration

ECS launch types: EC2 vs Fargate (cost, flexibility)
Task definitions and IAM roles
Sidecar containers (e.g., for logging, security)
ECS service discovery and internal DNS
Integration with ALB/NLB
Logging to CloudWatch or FluentBit + OpenSearch
CI/CD with ECS Blue/Green deployments (CodeDeploy)
Scaling services with custom metrics

☸️ 12. EKS – Kubernetes on AWS

Cluster provisioning via eksctl, Terraform, or CDK
Node groups: managed vs self-managed vs Fargate
IAM roles for service accounts (IRSA)
Kubernetes network plugins (AWS CNI, Calico)
Monitoring with Prometheus + Grafana + Container Insights
Ingress controllers (Nginx, ALB Ingress)
Service mesh integration (App Mesh, Istio)
Secrets and ConfigMaps management

🚀 13. CI/CD – DevOps with CodePipeline

CodePipeline stages, actions, and cross-account setups
CodeBuild with buildspec.yml for flexible builds
CodeDeploy for EC2 and ECS Blue/Green and Canary deployments
Artifact storage, versioning, and encryption
Manual approval steps and notifications
GitHub Actions vs CodePipeline comparison
Integration with Terraform or CDK for infra deployment

🌍 14. Route 53 – Global DNS

Hosted zones (public/private)
Health checks with failover routing
Latency-based and geolocation routing
Split-horizon DNS with Private Hosted Zones
DNSSEC and record validation
Traffic policies and Route 53 Resolver
Centralized DNS for multi-account setups

🔑 15. Secrets Manager & KMS – Secret & Key Management

Secret rotation (Lambda-backed) and scheduling
Cross-region secret replication
Secrets Manager vs Parameter Store comparison
KMS key rotation, aliases, grants, and audit logging
Envelope encryption and service integrations (S3, EBS, RDS)
Using customer-managed keys with Terraform/CDK

🏢 16. Organizations & SCPs – Multi-Account Architecture

OU design for security, billing, environment isolation
Guardrails via SCPs (deny dangerous actions)
Delegated administrators for services
AWS Control Tower for landing zone setup
Shared services VPC and central logging accounts
Cross-account access with IAM roles and Resource Access Manager

💰 17. Cost Optimization & Budgets

Cost Explorer deep dive and anomaly detection
Budgets for usage, costs, savings plan tracking
EC2 rightsizing and Compute Optimizer insights
Reserved Instance vs Savings Plan comparison
Spot instance tracking and automation
Tagging strategy for chargeback and showback

🔒 18. Security Intelligence Tools

GuardDuty: threat detection with real examples
Macie: sensitive data detection and classification in S3
Inspector: CVE scanning for EC2 and Lambda
Detective: investigation workflows with VPC Flow Logs
Security Hub as central aggregator
Automating security remediation using Lambda or SSM

🔐 19. IAM Identity Center / SSO – Central Access

Integration with Azure AD, Okta (SAML 2.0)
Permission sets and access assignments
SCIM provisioning for automated user/group sync
CLI access using Identity Center credentials
Audit logs and session tracking
Application SSO federation (Cloud, SaaS apps)

--------------------------------------------------------------

🔍 Why This Is Production-Grade Knowledge:
Area	How It's Production-Ready
Depth	Covers internal mechanics, not just surface concepts — e.g., how IAM evaluation logic really works, Lambda cold starts, CIDR design for scaling
Real Use Cases	Includes multi-account, multi-region, hybrid networking, secure cross-account access — these are common in real production setups
Trade-offs & Decisions	Compares options (ALB vs NLB, Parameter Store vs Secrets Manager, ECS vs EKS) — core skill of architects/admins
Security	Emphasizes least privilege, KMS, WAF, GuardDuty, SSO, and IRSA — critical for production-readiness
Scalability	Includes auto scaling, event-driven patterns, modular stacks, and monitoring — required for high-traffic applications
Automation	Focus on IaC (CDK/CloudFormation), CI/CD, patching, drift detection — how real teams deploy and manage infra
Observability	Logging, metrics, dashboards, alerts, X-Ray, centralized CloudWatch/CloudTrail — must-haves in any real environment
Cost & Compliance	Covers budgets, SCPs, tagging strategies, anomaly detection, Governance at scale
Integration & Dependencies	Teaches how to wire services together across accounts/VPCs — common in complex orgs

🔧 Real Problems You’ll Be Able to Handle:
"My EC2 instances can't reach the Internet from private subnet."
→ Solve with NAT Gateway, route tables, SG/NACL.
"I need secure cross-account access from Account A to Account B's S3 bucket."
→ Solve with trust policies, bucket policies, and KMS key grants.
"We want zero-downtime blue/green deployment for our containerized app."
→ Solve with ECS + CodeDeploy or EKS + Argo Rollouts.
"We have 40 accounts and want to restrict developers from creating internet-facing resources."
→ Solve with SCPs in AWS Organizations.
"A data breach happened, how do I investigate and ensure it doesn’t happen again?"
→ Use CloudTrail, GuardDuty, Detective, Config, and IAM Access Analyzer.
"Why is our bill suddenly spiking for S3?"
→ Diagnose with Cost Explorer, analyze lifecycle rules, access patterns, Glacier retrievals.
"We need to expose APIs securely and rate limit access."
→ Use API Gateway + Lambda + WAF + Cognito/Auth, with throttling and caching.

🛠️ If You Go Deep in This Path, You Will Be Able To:
Design resilient, secure, and scalable architectures
Troubleshoot real-world networking, IAM, performance, and cost issues
Build automated deployments with monitoring and recovery plans
Handle compliance, governance, and security investigations
Architect for multi-team, multi-account, and multi-region orgs

--------------------------------------------------------------------------