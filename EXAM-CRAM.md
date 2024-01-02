# Exam Cram: Cloud Computing and AWS

## Introduction

Welcome to the AWS Exam Cram, your quick guide to mastering essential concepts in Cloud Computing and Amazon Web
Services (AWS). Let's dive into key topics that will help you succeed in your AWS certification journey.

---

## Cloud Computing Models

### 1. Infrastructure as a Service (IaaS)

**Explanation:**
IaaS provides managed infrastructure up to the operating system level. Users have control over the operating system and
applications, allowing for greater customization.

**Tip:**
Leverage IaaS for scalable resources without the hassle of managing hardware. Focus on optimizing your applications and
workloads.

### 2. Platform as a Service (PaaS)

**Explanation:**
PaaS offers a managed platform up to the code level, reducing the burden of infrastructure management. Developers can
concentrate on coding and deploying applications.

**Tip:**
Use PaaS to streamline development processes. It's an excellent choice for projects where rapid development and
deployment are crucial.

### 3. Software as a Service (SaaS)

**Explanation:**
SaaS is a consumption-focused model where users access applications over the internet. It eliminates the need for
installation and maintenance.

**Tip:**
Consider SaaS for quick access to applications without worrying about underlying infrastructure. Ideal for businesses
focusing on core functionalities.

---

## Cloud Deployment Models

### 1. Public Cloud

**Explanation:**
Public Cloud, such as AWS, Azure, and GCP, provides services over the internet. It's scalable, cost-effective, and
accessible to the public.

**Tip:**
Utilize public cloud services for flexibility and scalability. AWS, with its vast service portfolio, is a preferred
choice for many enterprises.

### 2. Hybrid Cloud

**Explanation:**
Hybrid Cloud combines public and private clouds, offering flexibility and data control. It's suitable for businesses
with varying workload demands.

**Tip:**
Implement a hybrid strategy for a balance between scalability and data control. AWS provides tools for seamless
integration with on-premise solutions.

### 3. Private Cloud (On-premise)

**Explanation:**
Private Cloud is hosted on-premise, giving organizations direct control over resources. Common platforms include
Hyper-V, OpenStack, and VMware.

**Tip:**
Consider private cloud for sensitive data or specific regulatory requirements. AWS Outposts is a service that extends
AWS infrastructure to your on-premise location.

### 4. Multicloud

**Explanation:**
Multicloud involves using services from multiple cloud providers. It enhances redundancy and mitigates the risk of
vendor lock-in.

**Tip:**
Ensure compatibility and data portability when adopting a multicloud strategy. AWS provides services designed to work
seamlessly with various cloud providers.

---

## Fundamentals of Pricing

### Compute, Storage, and Outbound Data Transfer

**Explanation:**
AWS pricing revolves around compute resources (CPU/RAM), storage, and outbound data transfer. Understanding usage
patterns is crucial for cost optimization.

**Tip:**
Utilize AWS cost management tools to monitor and optimize resource consumption. Leverage reserved instances for
predictable workloads.

---

## AWS Global Infrastructure

### Regions, Availability Zones, Local Zones, and Edge Locations

**Explanation:**
AWS infrastructure is structured into regions, each containing multiple availability zones. Local Zones bring services
closer to end-users, while Edge Locations support content delivery.

**Tip:**
Design your architecture for high availability by distributing resources across multiple availability zones. Use AWS
Global Accelerator for optimized global routing.

---

## AWS Shared Responsibility Model

**Explanation:**
AWS follows a shared responsibility model where AWS manages "Security of the Cloud," and customers handle "Security in
the Cloud."

**Tip:**
Understand your responsibilities in the shared model. AWS provides robust security services, but proper configuration is
essential for a secure environment.

---

## Advantages of Cloud Computing

### 1. Trade Capital Expense for Variable Expense

**Explanation:**
Cloud computing allows organizations to pay for resources on a variable, on-demand basis, reducing the need for
significant upfront capital investment.

**Tip:**
Optimize costs by dynamically scaling resources based on demand. Leverage AWS Auto Scaling for automated resource
adjustments.

### 2. Benefit from Massive Economies of Scale

**Explanation:**
Cloud providers benefit from economies of scale, offering cost advantages that individual organizations may struggle to
achieve.

**Tip:**
Explore AWS pricing models, such as spot instances, to take advantage of cost savings during low-demand periods.

### 3. Stop Guessing About Capacity

**Explanation:**
Cloud resources can be scaled up or down based on demand, eliminating the need for organizations to predict future
capacity requirements.

**Tip:**
Implement AWS monitoring and alerting tools to stay informed about resource utilization and performance.

### 4. Increase Speed and Agility

**Explanation:**
Cloud services enable rapid deployment and development, allowing organizations to innovate and respond to market changes
more quickly.

**Tip:**
Leverage AWS DevOps services for continuous integration and continuous delivery (CI/CD) to enhance development speed.

### 5. Stop Spending Money Running and Maintaining Data Centers

**Explanation:**
Cloud computing shifts the burden of infrastructure maintenance to the cloud provider, reducing operational costs for
organizations.

**Tip:**
Consider AWS Managed Services to offload operational tasks, allowing your team to focus on strategic initiatives.

### 6. Go Global in Minutes

**Explanation:**
Cloud providers offer global infrastructure, enabling organizations to expand their reach and serve customers worldwide
with minimal effort.

**Tip:**
Utilize AWS Global Accelerator and Amazon CloudFront for low-latency, global content delivery.

# Exam Cram: Identity and Access Management (AWS IAM)

---

## AWS IAM Overview

### 1. What is AWS IAM?

**Explanation:**
AWS Identity and Access Management (IAM) is a web service designed to securely manage access to AWS resources. It
controls authentication (who is signed in) and authorization (who has permissions) for AWS services.

**Tip:**
IAM is fundamental for securing your AWS environment. Mastering IAM is crucial for managing user access and permissions
effectively.

### 2. Users, Groups, Policies, and Roles

**Explanation:**

- **Users:** Individual accounts for logging into AWS.
- **Groups:** Organize users and apply policies efficiently.
- **Policies:** Define permissions for users and groups.
- **Roles:** Delegated permissions assumed by AWS services.

**Tip:**
Organize users into groups, apply policies to groups, and use roles for efficient permission delegation.

---

## User Authentication and Authorization

### 1. User Logins and Access Keys

**Explanation:**

- Users log in to the AWS Management Console with a username and password.
- Access keys are used for programmatic CLI/API access.

**Tip:**
Secure user accounts by configuring strong passwords. Use access keys for programmatic access and automate tasks.

### 2. Root User and Multi-Factor Authentication (MFA)

**Explanation:**

- The root user is the account creator with full permissions.
- Multi-Factor Authentication (MFA) adds a second factor for enhanced security.

**Tip:**
Secure your root user account, and enable MFA for an extra layer of protection.

---

## Advanced IAM Concepts

### 1. Service Control Policies (SCPs)

**Explanation:**

- SCPs are part of AWS Organizations.
- They control the maximum available permissions in an AWS account.

**Tip:**
Leverage SCPs to enforce organizational security policies. They restrict, but do not grant, permissions.

---

## IAM Best Practices

### 1. General Best Practices

- **Lock away root user access keys:** Secure root user credentials to prevent unauthorized access.
- **Create individual IAM users:** Avoid using the root user for everyday tasks; create and manage individual IAM users.
- **Use groups for permissions:** Group users with similar roles and apply policies at the group level for efficiency.
- **Grant least privilege:** Only provide necessary permissions to users, following the principle of least privilege.

### 2. Policies and Permissions Best Practices

- **Start with AWS managed policies:** Utilize predefined AWS managed policies for common use cases.
- **Use customer managed policies:** Prefer customer-managed policies over inline policies for easier management.
- **Leverage access levels:** Regularly review IAM permissions using access levels (e.g., Read, Write, Full Access).

### 3. Security Best Practices

- **Configure a strong password policy:** Enforce robust password policies to enhance security.
- **Enable MFA:** Implement multi-factor authentication for an additional layer of protection.

### 4. Advanced Security Practices

- **Use roles for EC2 applications:** Assign roles to applications running on Amazon EC2 instances for secure access to
  AWS services.
- **Rotate credentials regularly:** Periodically change access keys and passwords to minimize the risk of compromise.
- **Remove unnecessary credentials:** Clean up unused access keys and IAM users regularly for enhanced security.
- **Use policy conditions:** Implement policy conditions for granular control and extra security.
- **Monitor account activity:** Set up logging and monitoring to track and respond to suspicious activities.

**Tip:**
Regularly review and update IAM configurations to align with evolving security requirements.

---

# Exam Cram: AWS Compute Services

---

## Amazon EC2 (Elastic Compute Cloud)

### 1. What is Amazon EC2?

**Explanation:**
Amazon EC2 is a versatile web service allowing you to run virtual server instances in the cloud. EC2 instances support
various operating systems, including Windows, Linux, and MacOS.

**Tip:**
Understand EC2 as the fundamental compute resource in AWS. Master the creation and management of EC2 instances for
diverse workloads.
Some EC2 instances the customers using AWS services must patch operating systems. **Windows** instance for example.

### 2. Amazon Machine Image (AMI)

**Explanation:**

- An AMI is used to launch EC2 instances.
- It consists of an EBS snapshot, permissions, and configuration settings.

**Tip:**
Create custom AMIs to streamline instance launches with pre-configured settings.

---

## Amazon EC2 Metadata and User Data

### 1. User Data and Metadata

**Explanation:**

- **User Data:** Supplied by users at instance launch as a script.
- **Instance Metadata:** Configurable data about instances.
- Both are not encrypted and accessible at `http://169.254.169.254/latest/meta-data`.

**Tip:**
Leverage User Data for instance customization, and use Instance Metadata for configuration.

### 2. Access Keys on EC2 Instances

**Explanation:**

- Access keys on EC2 instances grant permissions to other AWS services.
- Storing access keys in plaintext is insecure; prefer using IAM roles for enhanced security.

**Tip:**
Opt for IAM roles instead of access keys whenever possible to follow security best practices.

---

## AWS Batch

**Explanation:**
AWS Batch enables efficient execution of large-scale batch computing jobs on AWS. It dynamically provisions the optimal
compute resources based on workload demands.

**Tip:**
Ideal for scenarios requiring scalable batch processing. Master the dynamic resource provisioning aspect of AWS Batch.

---

## Amazon Lightsail

**Explanation:**
Amazon Lightsail is designed for users with limited AWS technical expertise. It simplifies the provisioning of compute,
storage, and networking for websites, applications, and databases.

**Tip:**
Perfect for smaller projects like blogs and websites. Use Lightsail for its straightforward management interface.

---

## Amazon Elastic Container Service (ECS)

### 1. Overview

**Explanation:**
ECS is used for running Docker containers in the cloud. Containers are referred to as tasks in ECS.

**Tip:**
Understand the basics of container orchestration and how ECS facilitates the deployment of containerized applications.

### 2. EC2 Launch Type vs. Fargate Launch Type

- **EC2 Launch Type:** You manage EC2 instances that host the tasks.
- **Fargate Launch Type:** AWS manages the underlying compute, cluster, and scaling for you.

**Tip:**
Choose the launch type based on your preference for managing infrastructure.

### 3. Amazon Elastic Container Registry (ECR)

**Explanation:**
ECR is a private container image registry, providing a secure location to store and manage Docker images.

**Tip:**
Utilize ECR for secure and efficient management of container images within the AWS ecosystem.

---

# Exam Cram: AWS Storage Services

---

## Amazon Elastic Block Store (EBS)

### 1. Persistence and Attachment

**Explanation:**

- EBS volumes persist independently of the instance's lifecycle.
- Multiple EBS volumes can be attached to an instance.
- Multi-attach allows a volume to be attached to multiple instances with constraints.

**Tip:**
Understand the characteristics and use cases of EBS volumes, especially the implications of multi-attach.

### 2. Snapshots

**Explanation:**

- Snapshots capture a point-in-time state of an instance.
- Stored on Amazon S3, snapshots are incremental with periodic snapshots.
- EBS volumes are AZ-specific, but snapshots are region-specific.

**Tip:**
Leverage snapshots for data backup, recovery, and migrating volumes across regions.

### 3. Data Lifecycle Manager (DLM)

**Explanation:**

- DLM automates the creation, retention, and deletion of EBS snapshots and EBS-backed AMIs.
- Ensures regular backup schedules, standardized AMIs, compliance, and reduced storage costs.

**Tip:**
Use DLM to manage the lifecycle of your EBS snapshots efficiently.

---

## Instance Store Volumes

**Explanation:**

- Instance store volumes are high-performance local disks attached to the host computer.
- Data on instance stores is ephemeral and lost when the instance is powered off.

**Tip:**
Ideal for temporary storage needs like buffers, caches, or scratch data. Not suitable for persistent data.

---

## Amazon Elastic File System (EFS)

**Explanation:**

- File-based storage system using the NFS protocol.
- Supports many EC2 instances concurrently, even across multiple AZs.
- Exclusive to Linux instances, and connections can be made from other VPCs.

**Tip:**
Consider EFS for scalable and shared file storage across multiple EC2 instances.

---

## Amazon Simple Storage Service (S3)

### 1. Basics

**Explanation:**

- S3 stores any file type with sizes ranging from 0 bytes to 5 TB.
- Offers unlimited storage with a unique global namespace for bucket names.

**Tip:**
Understand S3 basics, including bucket creation within a specific region.

### 2. Storage Classes

- **S3 Standard:** Durable, immediately available, frequently accessed.
- **S3 Intelligent-Tiering:** Automatically moves data to the most cost-effective tier.
- **S3 Standard-IA:** Durable, immediately available, infrequently accessed.
- **S3 One Zone-IA:** Lower cost for infrequently accessed data with less resilience.
- **S3 Glacier:** Archived data with retrieval times in minutes or hours.
- **S3 Glacier Deep Archive:** Lowest-cost storage class for long-term retention.

**Tip:**
Choose the appropriate storage class based on access patterns and cost considerations.

### 3. Additional Features

- **Transfer Acceleration:** Speeds up uploads using CloudFront.
- **Requester Pays:** The account requesting objects pays.
- **Events:** Trigger notifications to SNS, SQS, and Lambda.
- **Static Website Hosting:** Set up a static website.
- **Encryption:** Encrypt objects in the bucket.
- **Replication:** Replicate within (SRR) or across (CRR) regions.

**Tip:**
Leverage additional features for enhanced functionality and security.

### 4. S3 Versioning and S3 Object Lock

**Explanation:**

- **Versioning:** Keep multiple variants of an object, aiding in recovery from accidental deletion or overwrite.
- **Object Lock:** Enforce a write-once-read-many (WORM) model for fixed time or indefinite periods.

**Tip:**
Enable versioning for added protection against accidental changes. Use Object Lock for compliance and data retention.

### 5. S3 Glacier Retrieval Options

**Explanation:**

- Glacier offers two classes: Glacier and Glacier Deep Archive.
- Retrieval times vary based on the chosen option: Expedited, Standard, or Bulk.

**Tip:**
Understand the retrieval times and costs associated with each Glacier option.

---

## AWS Storage Gateway

**Explanation:**

- Hybrid cloud storage service enabling access to cloud storage from on-premises applications.
- Provides access to proprietary object storage (S3) using standard protocols.
- Use cases include moving backups to the cloud, using on-premises file shares backed by cloud storage, low-latency
  access to data in AWS, and disaster recovery.

**Tip:**
Understand the three types of gateways (File, Volume, Tape) and their respective use cases.

---

# Exam Cram: DNS, Elastic Load Balancing, and Auto Scaling

---

## Amazon Route 53

### 1. Overview

**Explanation:**

- Route 53 is AWS's Domain Name Service (DNS).
- Three main functions: Domain registration, DNS translation, and Health checking.

**Tip:**
Understand Route 53's role in managing domain names, translating them to IP addresses, and performing health checks.

### 2. Routing Policies

- **Simple:** Associates an IP address with a name.
- **Failover:** Routes to a secondary endpoint if the primary is down.
- **Geolocation:** Routes based on the geographic location of the request.
- **Geoproximity:** Routes to the closest Region within a geo area.
- **Latency:** Uses the lowest latency route to resources.
- **Multivalue Answer:** Returns several IP addresses.
- **Weighted:** Assigns relative weights (e.g., 80%/20%).

**Tip:**
Choose the routing policy that aligns with your application's requirements and design.

---

## Amazon EC2 Auto Scaling

### 1. Overview

**Explanation:**

- Automates the scaling of EC2 instances based on demand.
- Launches and terminates instances to handle application load.
- Creates collections of instances called Auto Scaling groups (ASG).

**Tip:**
Leverage EC2 Auto Scaling to ensure optimal resource availability and scalability.

### 2. Scaling Policies

- **Target Tracking:** Keeps the group at or close to a specified metric.
- **Simple Scaling:** Adjusts group size based on a metric.
- **Step Scaling:** Adjusts group size based on a metric with adjustments varying based on alarm breach size.
- **Scheduled Scaling:** Adjusts group size at a specific time.

**Tip:**
Choose scaling policies based on your application's performance requirements and scaling triggers.

---

## Amazon Elastic Load Balancing (ELB)

**Explanation:**

- ELB automatically distributes incoming application traffic across multiple targets.
- Can handle varying load in a single Availability Zone or across multiple Availability Zones.
- Features high availability, automatic scaling, and robust security.

**Tip:**
Use ELB to ensure fault tolerance, scalability, and efficient distribution of application traffic.

### 1. Types of ELB

- **Application Load Balancer (ALB):** Layer 7 load balancer routing connections based on request content.
- **Network Load Balancer (NLB):** Layer 4 load balancer routing connections based on IP protocol data.

**Tip:**
Understand the differences between ALB and NLB, and choose the appropriate type based on your application needs.

---

# Exam Cram: Application Services

---

## Serverless Computing

**Explanation:**

- Serverless eliminates the need to manage instances, provision hardware, or handle operating systems.
- Automatic scaling, high availability, and seamless capacity provisioning are intrinsic to serverless.

**Tip:**
Understand the benefits of serverless computing, especially its automatic scaling and cost efficiency.

---

## Serverless Services

**Explanation:**
Serverless services include:

- AWS Lambda
- AWS Fargate
- Amazon EventBridge
- AWS Step Functions
- Amazon SQS
- Amazon SNS
- Amazon API Gateway
- Amazon S3
- Amazon DynamoDB

**Tip:**
Familiarize yourself with the breadth of AWS serverless services, each serving specific use cases in modern application
development.

---

## AWS Lambda Functions

**Explanation:**

- Executes code only when needed and scales automatically.
- Pay only for the compute time consumed; no charges when code is not running.
- No servers to manage, continuous scaling, millisecond billing.

**Tip:**
Leverage AWS Lambda for event-driven, serverless computing tasks and understand its cost-effective, scalable nature.

---

## Amazon Simple Queue Service (SQS)

**Explanation:**

- Reliable, highly-scalable hosted queue for storing messages in transit.
- Used for distributed and decoupled applications.
- Message-oriented API using pull-based (polling) mechanism.

**Tip:**
Consider SQS for building loosely-coupled, distributed applications with reliable message storage and delivery.

---

## Amazon MQ

**Explanation:**

- Message broker service similar to SQS.
- Based on Apache Active MQ and RabbitMQ.
- Useful when industry-standard APIs and protocols are required, especially for migrating existing queue-based
  applications.

**Tip:**
Choose Amazon MQ when migrating existing queue-based applications to the cloud while maintaining industry-standard APIs.

---

## Amazon Simple Notification Service (SNS)

**Explanation:**

- Publisher/subscriber model for building loosely-coupled, distributed applications.
- Provides instantaneous, push-based delivery with simple APIs.
- Pay-as-you-go model with no upfront costs.

**Tip:**
Use SNS for real-time communication in distributed systems, especially when a push-based model is preferred.

---

## AWS Step Functions

**Explanation:**

- Coordinates components of distributed applications as a series of steps in a visual workflow.
- Quickly builds and runs reliable and scalable state machines.

**Tip:**
Leverage Step Functions for orchestrating workflows in distributed applications in a visual and scalable fashion.

---

## Amazon Simple Workflow Service (SWF)

**Explanation:**

- Coordinates work across distributed application components.
- Suited for human-enabled workflows or procedural requests.
- AWS recommends considering Step Functions for new applications.

**Tip:**
Prefer Step Functions for new applications, but understand SWF for scenarios involving human-enabled workflows.

---

## Amazon EventBridge

**Explanation:**

- Serverless event bus for building event-driven architectures.
- Ingests and routes data to target AWS services.

**Tip:**
Use EventBridge to simplify building event-driven architectures with seamless integration with other AWS services.

---

## Amazon API Gateway

**Explanation:**

- Publish APIs on AWS, creating RESTful and WebSocket APIs.
- Fully managed service forwarding connections to AWS services and on-premises applications.

**Tip:**
Leverage API Gateway for creating and managing APIs with ease, facilitating communication between applications.

---

# Exam Cram: Amazon VPC, Networking, and Hybrid

---

## Amazon Virtual Private Cloud (VPC)

**Explanation:**

- A virtual network dedicated to your AWS account, providing complete control over the virtual networking environment.
- Logically isolated from other virtual networks in the AWS Cloud.
- Allows launching AWS resources (e.g., EC2 instances) into your VPC.

**Tip:**
Think of a VPC as your private network within AWS, offering control and isolation.

---

## VPC Configuration

**Explanation:**

- When creating a VPC, specify a range of IPv4 addresses using a Classless Inter-Domain Routing (CIDR) block (e.g.,
  10.0.0.0/16).
- Spans all Availability Zones (AZs) in the region.
- Control access to resources inside your VPC.
- Default limit: Up to 5 VPCs per region.

**Tip:**
Understand CIDR blocks, default VPCs, and the regional span of VPCs.

---

## Security Groups vs. Network ACLs

**Security Groups:**

- Operate at the instance level.
- Allow rules only.
- Stateful.

**Network ACLs:**

- Operate at the subnet level.
- Support both allow and deny rules.
- Stateless, processing rules in order.

**Tip:**
Security Groups for instance-level security, Network ACLs for subnet-level control.

---

## IP Addresses

**Explanation:**

- Public IPs are dynamic and lost when an instance is stopped.
- Private IPs are attached to all EC2 instances and retained when the instance is stopped.
- Elastic IPs are static public addresses, retained when the instance is stopped and can be moved between instances (
  chargeable if not used).

**Tip:**
Understand the characteristics and use cases for public, private, and Elastic IPs.

---

## NAT Instances and Gateways

**NAT Instances:**

- Used for internet access from private subnets.
- Deployed in public subnets (managed by you).

**NAT Gateways:**

- Managed by AWS.
- Also used for internet access from private subnets.

**Tip:**
NAT instances and gateways enable private subnets to access the internet securely.

---

## VPC Peering, AWS Managed VPN, AWS Direct Connect

**VPC Peering:**

- Routes between VPCs using private IP addresses.

**AWS Managed VPN:**

- VPN connection between on-premises sites and AWS.
- Uses the public Internet.

**AWS Direct Connect:**

- Private connection from on-premises to AWS.
- Avoids the public Internet.

**Tip:**
Understand the use cases and differences between VPC peering, AWS Managed VPN, and AWS Direct Connect.

---

## AWS Transit Gateway, AWS Outposts

**AWS Transit Gateway:**

- Connects VPCs and on-premises networks through a central hub.
- Simplifies network configuration.

**AWS Outposts:**

- Deploy AWS infrastructure on-premises.
- Extends a VPC into the on-premises environment.
- Supports several AWS services.

**Tip:**
AWS Transit Gateway centralizes network connections, while AWS Outposts extends AWS services on-premises.

---

# Exam Cram: Deployment and Automation

---

## Amazon CloudFront

**Explanation:**

- Content Delivery Network (CDN) caching content at edge locations worldwide.
- Accelerates content delivery for data, videos, applications, and APIs.
- Enhances security against DDoS attacks.
- Reduces latency for global users.

**Tip:**
CloudFront is ideal for optimizing content delivery globally.

---

## AWS Global Accelerator

**Explanation:**

- Routes connections to application endpoints in multiple regions.
- Improves application availability and performance for local or global users.
- Utilizes the AWS global network to optimize TCP and UDP traffic.

**Tip:**
AWS Global Accelerator enhances performance for diverse applications across regions.

---

## AWS Global Accelerator vs. CloudFront

**Comparison:**

- Both leverage the AWS global network and edge locations.
- CloudFront focuses on caching for content (cacheable and dynamic).
- Global Accelerator optimizes TCP and UDP traffic for various applications.
- Global Accelerator enables failover between AWS Regions.

**Tip:**
CloudFront for content caching, Global Accelerator for optimizing diverse application traffic.

---

## AWS CloudFormation

**Explanation:**

- Provision infrastructure consistently, reducing human errors.
- Saves time compared to manual resource configuration.
- Templates in YAML or JSON describe infrastructure.
- Creates a stack based on the template.
- Supports easy rollback and deletion of the entire stack.

**Tip:**
CloudFormation streamlines infrastructure provisioning and management.

---

## AWS Cloud Development Kit (CDK)

**Explanation:**

- Open-source framework for defining cloud application resources.
- Uses familiar programming languages (TypeScript, Python, Java, .NET).
- Preconfigures resources with proven defaults.
- Provisions resources using AWS CloudFormation.
- Enables modeling of application infrastructure with existing IDEs and tools.

**Tip:**
CDK simplifies cloud resource definition using familiar programming languages.

---

## AWS Elastic Beanstalk

**Explanation:**

- Managed service for web applications on EC2 instances and Docker containers.
- Deploys environments with Auto Scaling, Elastic Load Balancing, and databases.
- Platform as a Service (PaaS) solution.
- Provides control over underlying resources.
- Supports code deployment via ZIP file, WAR file, or Git repository.

**Tip:**
Elastic Beanstalk streamlines web application deployment and management.

---

## AWS X-Ray and AWS OpsWorks

**AWS X-Ray:**

- Analyzes and debugs production, distributed applications, especially those with microservices architecture.

**AWS OpsWorks:**

- Configuration management service providing managed instances of Chef and Puppet.
- Handles updates, patching, backup, configuration, and compliance management.

**Tip:**
X-Ray aids in analyzing microservices, OpsWorks offers managed instances for configuration management.

---

# Exam Cram: Databases and Analytics

---

## Amazon Relational Database Service (RDS)

**Explanation:**

- Utilizes EC2 instances; choose an instance family/type.
- Represents Structured Query Language (SQL) databases.
- Online Transaction Processing (OLTP) database type.
- Easy setup, high availability, fault tolerance, and scalability.
- Supports encryption using AWS Key Management Service (KMS).

**Tip:**
RDS is well-suited for online stores and banking systems, offering ease of management and encryption.

---

## Amazon Aurora

**Explanation:**

- Part of the RDS family, compatible with **MySQL** and **PostgreSQL**.
- Distributed, fault-tolerant, self-healing storage system.
- Auto-scales up to 128TB per database instance.
- Has automatic backup enabled.

**Tip:**
Amazon Aurora provides a robust and scalable relational database solution in the AWS environment.

---

## Amazon DynamoDB

**Explanation:**

- Fully managed NoSQL database service.
- Serves as a key/value store and document store.
- Serverless, supporting push-button scaling.

**Features:**

- Serverless, highly available, scalable, NoSQL.
- DynamoDB Accelerator (DAX) for in-memory caching.
- Backup and restore options.
- Global Tables for multi-region, multi-master solutions.

**Tip:**
DynamoDB is versatile, supporting flexible schema, horizontal scaling, and serverless architecture.

---

## Amazon RedShift

**Explanation:**

- SQL-based data warehouse for analytics.
- Relational database for Online Analytics Processing (OLAP) use cases.
- Uses Amazon EC2 instances; choose an instance family/type.
- Maintains three copies of data, continuous/incremental backups.

**Tip:**
Amazon RedShift is designed for analytical queries and data warehousing, with redundancy and continuous backups.

---

## Amazon EMR

**Explanation:**

- Managed cluster platform for big data frameworks (Hadoop, Spark).
- Used for analytics, business intelligence, and ETL functions.
- Extract, transform, and load (ETL) processes supported.

**Tip:**
Amazon EMR simplifies the processing of large datasets for analytics and business intelligence.

---

## Amazon ElastiCache

**Explanation:**

- Fully managed Redis and Memcached implementations.
- Key/value store for high-performance, low-latency in-memory databases.
- Can be used in front of databases like RDS and DynamoDB.

**Tip:**
ElastiCache enhances performance by providing in-memory caching for frequently accessed data.

---

## Amazon Athena and AWS Glue

**Amazon Athena:**

- Queries data in S3 using SQL.
- Supports various data formats.
- Utilizes a managed Data Catalog (AWS Glue).

**AWS Glue:**

- Fully managed ETL service.
- Prepares data for analytics.
- Runs ETL jobs on a managed Apache Spark environment.

**Tip:**
Athena simplifies querying data in S3 using SQL, while Glue prepares and processes data for analytics.

---

## Amazon Kinesis

**Kinesis Data Streams:**

- Producers send data stored in shards for up to 7 days.
- Consumers process and save data.

**Kinesis Data Firehose:**

- Automated, elastically scalable data delivery without shards.
- Directly saves data to services like S3, Splunk, RedShift, or Elasticsearch.

**Kinesis Data Analytics:**

- Provides real-time SQL processing for streaming data.

**Tip:**
Amazon Kinesis offers versatile options for real-time data processing and analytics.

---

## AWS Data Pipeline, QuickSight, and More

**AWS Data Pipeline:**

- Moves data between AWS compute and storage services.
- Saves results to services like S3, RDS, DynamoDB, and EMR.

**QuickSight:**

- Business intelligence service.
- Creates interactive BI dashboards for ML-powered insights.

**Others:**

- Amazon Neptune: Fully managed graph database service.
- Amazon DocumentDB: Fully managed document database supporting MongoDB workloads.
- Amazon QLDB: Fully managed ledger database.
- Amazon Managed Blockchain: Fully managed service for joining public and private networks.

**Tip:**
Explore AWS services like Data Pipeline, QuickSight, Neptune, DocumentDB, QLDB, and Managed Blockchain for comprehensive
analytics and database solutions.

---

# Exam Cram: Management and Governance

---

## AWS Organizations

**Explanation:**

- Consolidates multiple AWS accounts into a centrally managed organization.
- Two feature sets: Consolidated Billing and All Features.
- Includes root accounts and organizational units (OUs).
- Policies are applied to root accounts or OUs.
- Consolidated Billing includes Paying Account and Linked Accounts.

**Tip:**
AWS Organizations streamlines management by organizing and consolidating multiple AWS accounts under a central
structure.

---

## AWS Control Tower

**Explanation:**

- Simplifies the creation of multi-account environments.
- Establishes governance, compliance, and security guardrails.
- Integrates with various services, including AWS Organizations, SCPs, OUs, AWS Config, AWS CloudTrail, and more.

**Tip:**
AWS Control Tower automates the setup of foundational AWS services to ensure a secure and compliant multi-account
environment.

---

## AWS Systems Manager

**Components:**

- **Automation:** Uses documents to run automations.
- **Run Command:** Executes commands on EC2 instances.
- **Inventory:** Gathers inventory information.
- **Patch Manager:** Manages patching schedules and installation.
- **Session Manager:** Connects securely without SSH or RDP.
- **Parameter Store:** Stores secrets and configuration data securely.

**Tip:**
AWS Systems Manager provides a unified interface for managing AWS resources, offering automation, inventory tracking,
and secure connections.

---

## AWS Service Catalog

**Explanation:**

- Enables organizations to create and manage catalogs of approved IT services on AWS.
- Centrally manages commonly deployed IT services.
- IT services include virtual machine images, servers, software, databases, and multi-tier application architectures.

**Tip:**
AWS Service Catalog facilitates the efficient deployment of approved IT services, ensuring consistency and compliance.

---

## AWS Config

**Explanation:**

- Fully-managed service for compliance management.
- Assists with compliance auditing, security analysis, resource change tracking, and troubleshooting.

**Tip:**
AWS Config provides comprehensive visibility into resource configurations, aiding in compliance management.

---

## Trusted Advisor

**Explanation:**

- Online resource for optimizing AWS environments.
- Offers real-time guidance on cost optimization, performance, security, and fault tolerance.
- Advises on best practices for provisioning resources.

**Tip:**
Leverage Trusted Advisor for real-time recommendations on optimizing your AWS environment.

---

## AWS Personal Health Dashboard

**Explanation:**

- Provides alerts and remediation guidance during AWS events.
- Offers a personalized view of the performance and availability of AWS services.
- Proactively notifies about scheduled activities.

**Tip:**
AWS Personal Health Dashboard ensures you stay informed about the impact of AWS events on your resources.

---

## Service Health Dashboard

**Explanation:**

- Displays the current status of AWS services.
- Not personalized; provides general service status.

**Tip:**
Use the Service Health Dashboard to monitor the overall status of AWS services.

---

# Exam Cram: AWS Cloud Security and Identity

---

## AWS Directory Services

**AWS Managed Microsoft AD:**

- Full Microsoft AD managed by AWS.
- Suitable for enterprises requiring hosted Microsoft Active Directory.

**AD Connector:**

- Allows on-premises users to log into AWS services with existing AD credentials.
- Facilitates single sign-on for on-premises employees.

**Simple AD:**

- Low-scale, low-cost AD implementation based on Samba.
- Suitable for simple user directories or when LDAP compatibility is needed.

**Tip:**
Choose the AWS Directory Service that aligns with your organization's requirements for Active Directory.

---

## AWS Systems Manager Parameter Store

- Provides secure, hierarchical storage for configuration data and secrets.
- Stores data such as passwords, database strings, and license codes.
- Supports plaintext or ciphertext storage.
- References values using unique names.

**Tip:**
AWS Systems Manager Parameter Store is a secure way to manage and retrieve configuration data and secrets.

---

## AWS Secrets Manager

- Similar to Parameter Store with additional features.
- Allows native and automatic rotation of keys.
- Offers fine-grained permissions.
- Provides central auditing for secret rotation.

**Tip:**
AWS Secrets Manager is designed for secure and automated handling of sensitive information.

---

## AWS Certificate Manager (ACM)

- Creates, stores, and renews SSL/TLS X.509 certificates.
- Supports single domains, multiple domain names, and wildcards.
- Integrates with various AWS services.

**Tip:**
Use ACM to simplify the management of SSL/TLS certificates for your applications.

---

## AWS Key Management Service (KMS)

- Creates and manages encryption keys.
- Provides centralized control over encryption keys.
- Integrated with most AWS services for easy data encryption.

**Tip:**
AWS KMS is essential for securing and managing encryption keys across AWS services.

---

## AWS CloudHSM

- Cloud-based hardware security module (HSM).
- Allows generation and use of encryption keys on the AWS Cloud.
- Provides FIPS 140-2 Level 3 validated HSMs.
- Operates within your VPC.

**Tip:**
Use AWS CloudHSM for secure key management and cryptographic operations in your VPC.

---

## AWS CloudTrail

- Logs API activity for auditing purposes.
- Default retention of management events for 90 days.
- Trails can log events to S3 for indefinite retention.
- CloudWatch Events and CloudWatch Logs integration.

**Tip:**
Leverage AWS CloudTrail to maintain a comprehensive audit trail of API activity in your AWS environment.

---

## VPC Flow Logs

- Capture information about IP traffic in a VPC.
- Stored using Amazon CloudWatch Logs.
- Can be created at VPC, subnet, or network interface levels.

**Tip:**
VPC Flow Logs provide insights into IP traffic patterns for monitoring and troubleshooting.

---

## Elastic Load Balancing Access Logs

- Capture detailed information about requests to the load balancer.
- Useful for analyzing traffic patterns and troubleshooting.
- Optionally stored and retained in S3.

**Tip:**
Enable Elastic Load Balancing Access Logs to analyze and troubleshoot traffic patterns effectively.

---

## Amazon Detective

- Analyzes, investigates, and identifies potential security issues.
- Collects data from AWS resources using machine learning, statistical analysis, and graph theory.
- Utilizes data sources such as VPC Flow Logs, CloudTrail, and GuardDuty.

**Tip:**
Amazon Detective enhances security analysis and investigation using machine learning.

---

## AWS GuardDuty

- Intelligent threat detection service.
- Monitors for account compromise, instance compromise, reconnaissance, and bucket compromise.
- Continuous monitoring for events across various AWS services.

**Tip:**
AWS GuardDuty helps detect and respond to security threats in your AWS environment.

---

## Amazon Macie

- Fully managed data security and privacy service.
- Uses machine learning and pattern matching to discover and monitor sensitive data on Amazon S3.
- Enables security compliance and preventive security measures.

**Tip:**
Amazon Macie is designed for discovering and protecting sensitive data stored on Amazon S3.

---

## AWS WAF and AWS Shield

- **AWS WAF:**
    - Web application firewall.
    - Creates rules to block common web exploits.
    - Uses Web ACLs to define rules.

- **AWS Shield:**
    - Managed DDoS protection service.
    - Provides continuous monitoring and automatic inline mitigations.

**Tip:**
Combine AWS WAF and AWS Shield for robust protection against web exploits and DDoS attacks.

---

## AWS Artifact

- Provides on-demand access to AWS security and compliance reports.
- Includes reports such as SOC reports and PCI reports.

**Tip:**
Use AWS Artifact to access security and compliance reports for your AWS resources.

---

## AWS Security Hub

- Offers a comprehensive view of security alerts and posture across AWS accounts.
- Aggregates, organizes, and prioritizes security alerts from multiple AWS services.

**Tip:**
AWS Security Hub enhances security monitoring and incident response in your AWS environment.

---

## AWS Trust & Safety Team

- Contact for addressing misuse of AWS resources.
- Handles issues like spam, port scanning, DDoS attacks, intrusion attempts, objectionable content, and malware
  distribution.

**Tip:**
Engage with the AWS Trust & Safety team to report and address misuse of AWS resources.

---

## Penetration Testing

- Practice of testing one's application security for

vulnerabilities.

- AWS allows penetration testing without prior approval for eight AWS services.

**Tip:**
Leverage AWS's penetration testing permissions for enhancing the security of your AWS applications.

---

# Exam Cram: AWS Well-Architected Framework

---

## Operational Excellence Pillar

**Objective:**
Support development and run workloads effectively, gain insight into workload operations, and continuously improve
processes and procedures to deliver business value.

**Best Practices:**

- **Perform operations as code:** Manage and automate operations using code to increase efficiency.
- **Make frequent, small, reversible changes:** Avoid making large changes to reduce risk and impact.
- **Refine operations procedures frequently:** Continuously review and improve operational procedures.
- **Anticipate failure:** Design for failure by understanding potential failure points.
- **Learn from all operational failures:** Use incidents as learning opportunities to prevent future issues.

---

## Security Pillar

**Objective:**
Protect data, systems, and assets to leverage cloud technologies and improve security.

**Best Practices:**

- **Implement a strong identity foundation:** Establish and manage robust identity and access controls.
- **Enable traceability:** Monitor and audit actions to ensure accountability.
- **Apply security at all layers:** Employ security measures across all components of the architecture.
- **Automate security best practices:** Use automation to enforce and maintain security configurations.
- **Protect data in transit and at rest:** Implement encryption to secure data during transmission and storage.
- **Keep people away from data:** Minimize human access to sensitive data.
- **Prepare for security events:** Have plans and processes in place to respond to security incidents.

---

## Reliability Pillar

**Objective:**
Ensure a workload can perform its intended function correctly and consistently when expected.

**Best Practices:**

- **Automatically recover from failure:** Implement self-healing mechanisms to recover from failures.
- **Test recovery procedures:** Regularly test and validate recovery procedures.
- **Scale horizontally:** Increase aggregate workload availability by distributing load across multiple resources.
- **Stop guessing capacity:** Use auto-scaling and other dynamic scaling strategies.
- **Manage change in automation:** Implement automated processes for managing changes.

---

## Performance Efficiency Pillar

**Objective:**
Use computing resources efficiently to meet system requirements and maintain efficiency as demand changes.

**Best Practices:**

- **Democratize advanced technologies:** Provide access to advanced technologies to the entire organization.
- **Go global in minutes:** Use AWS services to deploy globally.
- **Use serverless architectures:** Leverage serverless computing to eliminate the need for server management.
- **Experiment more often:** Continuously experiment with new technologies and architectures.
- **Consider mechanical sympathy:** Understand the characteristics and constraints of the underlying hardware.

---

## Cost Optimization Pillar

**Objective:**
Run systems to deliver business value at the lowest price point.

**Best Practices:**

- **Implement Cloud Financial Management:** Apply financial management disciplines to the AWS environment.
- **Adopt a consumption model:** Pay only for what you consume.
- **Measure overall efficiency:** Monitor and optimize the overall cost efficiency of your workload.
- **Stop spending money on undifferentiated heavy lifting:** Use managed services to reduce operational overhead.
- **Analyze and attribute expenditure:** Regularly review and attribute costs to identify opportunities for
  optimization.

---

# Exam Cram: Accounts, Billing and Support

This Exam Cram provides key information related to accounts, billing, and support in AWS.

---

## Pay-as-you-go

- Easily adapt to changing business needs.
- Improved responsiveness to change.
- Adapt based on needs, not forecasts.
- Reduce risk over overpositioning or missing capacity.

## Save when you reserve

- Invest in reserved capacity (e.g., RDS and EC2).
- Save up to 75% compared to on-demand (pay-as-you-go).
- The more you pay upfront, the greater the discount.

## Pay less by using more

- Pay less using volume-based discounts.
- Tiered pricing means the more you use, the lower the unit pricing.

## Pricing Models

- **Reserved Instances:** 1 or 3-year commitment; up to 75% discount; steady-state, predictable workloads and reserved
  capacity.
- **Spot Instances:** Bid for unused capacity; up to 90% discount; can be terminated at any time; workloads with
  flexible start and end times.
- **Dedicated Instances:** Physical isolation at the host hardware level from instances belonging to other customers;
  pay per instance.
- **Dedicated Hosts:** Physical server dedicated for your use; socket/core visibility, host affinity; pay per host;
  workloads with server-bound software licenses.
- **Savings Plans:** Commitment to a consistent amount of usage (EC2 + Fargate + Lambda); Pay by $/hour; 1 or 3-year
  commitment.

## Amazon S3 Pricing

- Factors affecting pricing: Storage class, storage quantity, number of requests, lifecycle transitions requests, data
  transfer.

## Amazon Glacier Pricing

- Three options for access to archives: Expedited, Standard, Bulk.
- Data access time and retrieval costs vary based on the chosen option.

## Amazon EBS Pricing

- Volumes charged by the amount of GB provisioned per month.
- Snapshots based on the amount of space consumed by snapshots in S3.

## Amazon RDS Pricing

- Clock hours of server uptime.
- Database characteristics (engine, size, memory class).
- Database purchase type (On-Demand, Reserved).

## Amazon DynamoDB Pricing

- Charged for reading, writing, and storing data.
- On-demand capacity mode or provisioned capacity mode.

## AWS Lambda Pricing

- Charged based on the number of requests, duration of requests, and memory allocated to the function.

## AWS Organizations

- Consolidated billing benefits: One bill, easy tracking, combined usage, no extra fee.

## AWS Budgets

- Set custom budgets, configure alerts, integrated with other AWS services.

## AWS Cost Explorer

- Free tool to view charts of your costs.
- Discover patterns in spending on AWS resources over time.
- Identify cost problem areas.

## AWS Cost & Usage Report

- Publish AWS billing reports to an S3 bucket.
- Reports break down costs by hour, day, month, product, product resource, and tags.

## AWS Price List API

- Query the prices of AWS services.
- Utilizes the Price List Service API and AWS Price List API.

# Exam Cram: Migration, Machine Learning, and More

---

## AWS Migration Hub

- Provides a single location to track the progress of application migrations across multiple AWS and partner solutions.

## AWS Database Migration Service (DMS)

- Helps migrate databases to AWS quickly and securely.
- Source database remains fully operational during migration, minimizing downtime.

## AWS Server Migration Service (SMS)

- Migrates servers and virtual machines to Amazon EC2.
- Agentless service for faster migration of on-premises workloads to AWS.
- Automates, schedules, and tracks incremental replications of live server volumes.

## AWS DataSync

- Online data transfer service.
- Transfers data between on-premises and AWS storage services.

## Snowball Family

- Used for migrating large volumes of data to AWS.
- Snowball Edge Compute Optimized: Provides block and object storage, optional GPU, for edge computing use cases.
- Snowball Edge Storage Optimized: Provides block storage and S3-compatible object storage for local storage and
  large-scale data transfer.
- Snowcone: Small device for edge computing, storage, and data transfer; can transfer data offline or online with AWS
  DataSync agent.
- Uses secure storage devices for physical transportation (Snowball - 80TB, Snowball Edge - 100TB, Snowmobile - "exabyte
  scale" with up to 100PB).

## AWS Rekognition

- Adds image and video analysis to applications.
- Identifies objects, people, text, scenes, and activities in images and videos.

## Amazon Transcribe

- Adds speech-to-text capabilities to applications.
- Converts recorded speech to text for use in applications.

## Amazon Translate

- Neural machine translation service for fast, high-quality, and affordable language translation.
- Localizes content such as websites and applications for diverse users.

## Amazon SageMaker

- Assists data scientists and developers in preparing, building, training, and deploying high-quality machine learning (
  ML) models.

## Amazon Comprehend

- Natural-language processing (NLP) service.
- Uses machine learning to uncover information in unstructured data.

## Amazon Lex

- Conversational AI for chatbots.
- Builds conversational interfaces into any application using voice and text.

## Amazon Polly

- Turns text into lifelike speech.
- Creates applications that talk and builds speech-enabled products.

## Amazon Workspaces

- Managed Desktop-as-a-Service (DaaS) solution.
- Provision either Windows or Linux desktops.

## AWS AppStream 2.0

- Fully managed non-persistent application streaming service.
- Alternative to popular products such as Citrix XenApp.

## AWS WorkLink

- Provides secure, one-click access to internal websites and web apps using mobile phone browsers.
- Does not require VPN client or app.

## AWS WorkDocs

- Fully managed, secure content creation, storage, and collaboration service.
- Creates, edits, and shares content centrally stored on AWS.

## AWS IoT Core

- Connects IoT devices to the AWS cloud without the need to provision or manage servers.
