AWS Partner: Accreditation (Technical)

The AWS Partner: Accreditation (Technical) training provides AWS Partner Network (APN) Partners with fundamental, technical knowledge of AWS cloud computing, global infrastructure, services, solutions, migration, and security. This course is designed to teach students the fundamental principles of AWS solution architecture design and to introduce the basic skills needed to engage customers in a pre-sales AWS technical opportunity. It is intended to empower learners to make recommendations and informed decisions about AWS cloud solutions based on customer business requirements. Upon successful completion of the accreditation test, you will earn accreditation as an AWS Technical Professional.

Benefits of cloud computing:

Agility: Cloud provides more resources to organizations
Elasticity: Resources can be provisioned with the amount of resources that are actually needed
Cost Savings: Only pay for IT as it its consumed (pay-as-you-go pricing)
Deploy globally in minutes: Can deploy an application in multiple locations with a few clicks

AWS Regions:

Completely isolated from each other
Certain resources are tied to regions

AWS Availability Zones:

All AZs (availability zones) are connected to the same region, but they are separated within the AZ, for example: 
- AP-SOUTHEAST-1 (singapore region) is divided in 3 datacenters:  
    - AP-SOUTHEAST-1a, AP-SOUTHEAST-1b and AP-SOUTHEAST-1c

Other AWS global infrastructure:

Local Zone
Wavelength Zones
Direct Connect Locations
Edge Locations
Regional Edge Caches

——————————————————————————————————————————————————————————————————————————————————————————————————————————————

Introduction to AWS Core Technologies

AWS Core Technologies - Compute:

- Amazon EC2 (Amazon Elastic Compute Cloud): Is a web service that provides secure resizable compute capacity
- Amazon EC2 Auto Scaling: Increase or decrease number of instances
- Elastic Load Balancing: Distribute incoming traffic
- Amazon Elastic Container Service: Run applications on a managed cluster (managed cluster of EC2 instances or an AWS fargate)
- Amazon Elastic Kubernetes Service: Run Kubernetes applications on AWS and on-premises
- AWS Lamba: Run code in response to events (server-less computing)

Benefits of Amazon EC2:

Elasticity
Control
Flexibility
Integrated
Reliable
Secure
Cost-effective
Easy

Amazon EC2 choices:

Instance Types:

- General Purpose
- Compute Optimized
- Memory Optimized
- Accelerated Computing
- Storage Optimized 

Each category has different families and each family has different generations (MAC, T, M, A)

Amazon Machine Images (AMI):

Customers need to choose an AMI to run the instance (s) - Linux, Windows…

Why Scaling Matters:

Scaling is flexible with cloud:

- Launch new instances in advance of peak periods
- Use monitoring to programmatically scale out
- Automatically scale in when needed
- Pay for the resources needed, only when needed

Amazon EC2 Auto Scaling group:

- Automatically adjusts resource capacity
- Define where Amazon EC2 Auto Scaling deploys resources
- Specify the Amazon VPC and subnets (must select at least 2 subnets across different availability zones)

An auto scaling group can have their instances automatically picked.

Amazon Elastic Load Balancing (ELB):

Automatically distribute traffic across multiple EC2 instances

- Increases availability and fault tolerance
- Configure health checks
- Offload encryption and decryption
- Types of ELB:
    - Application Load balancer (operates on the app layer, best to web apps)
    - Network Load Balancer (operates on the network layer)
    - Gateway Load Balancer

AWS Core Technologies - Storage:

- Amazon Elastic Block Store (EBS): Persistent block-level storage, it’s like a hard-drive for the instances
- Amazon S3: Durable, scalable object storage (images for ex)
- Amazon S3 Glacier: Data archiving and backup (retain data for weeks, months, years and even decades)
- AWS Storage Gateway: Integrate cloud storage with on-site workloads 
- Amazon Elastic File System (EFS): File storage for Amazon EC2 instances (is elastic because it grows and shrinks automatically)
- Amazon FSx: File storage for widely-used file systems

Amazon Elastic Block Store (EBS):

Network-attached block storage for use with Amazon EC2 instances:
- Persist independently from instance
- Used like a physical hard drive
- Automatically replicated
- Attached to any instance in the same AZ
- One instance to many EBS volumes
- EBS Volumes can retain data after EC2 instance termination
- Allow point-in-time snapshots to S3 GiB increments

They replicate all EBS volumes upon creation.

Amazon Simple Storage Service (Amazon S3):

Object storage service that stores objects inside buckets, where customers can read, write and delete objects that are inside the buckets. Infinite scalability, greater analysis and faster data retrievel. Hight scalability, durability and availability.

Common S3 use cases:

- Data lakes (used to store a lot of data for IA, machine learning and a bunch of data analytics)
- Backup and storage
- Application hosting
- Media hosting
- Software delivery

Storage classes on Amazon S3:

- Amazon S3 Standard (frequently access - higher cost)
- Amazon S3 Standard-Infrequent Access
- Amazon S3 One Zone-Infrequent Access
- S3 Glacier Storage Classes (archived data - lower cost)

AWS Core Technologies - Databases: 

We can install and configure a database in an EC2 instance, but we can use AWS database services to manage databases.

- Amazon RDS (Relational databases): Customers can set-up, operate and scale a relational database in the cloud, that provides cost-efficient and resizable capacity (Cost-efficient and resizable capacity). It contains many other features, including automated backups, database snapshots and automatic host replacement
- Amazon DynamoDB (NoSQL): Fast and predictable performance 
- Amazon ElasticCache: Fast, managed information retrieval (cloud caching system)

Advantages of hosting a database using AWS Databases Services:

- Easy to set up, manage and maintain
- Reduce undifferentiated heavy lifting
- Push-button high availability
- Automatic backup/recovery
- Scale up or down based upon pattern

Advantages of hosting a database on a Amazon EC2 instance (manual):

- More control/flexibility
- Operating system access
- Need features of specific application (configs and etc)

AWS Core Technologies - Networking:

- Amazon VPC: Build a virtual network in the cloud
- Security Groups: Control access to instances
- Network Access Control Lists (NACL): Control access to subnets
- Amazon Route 53: Route end users to internet applications (DNS service)

Amazon Virtual Private Cloud (VPC):

- Networking layer for AWS resources
- A virtual network dedicated to a customer’s AWS account 

Subnet:
- Is a range of IP addresses in a VPC

Securing a VPC:

- Network Access Control Lists: Control traffic at the subnet level
- Security groups: Control traffic at the instance level
- Flow logs: Capture network flow information
- Host-based firewalls: Operating system firewalls

AWS networking: 

- VPC = virtual network in the cloud
- Then create public and private subnets
- Can secure the network with Network ACLs (NACL)
- Configure other layers of security using Security groups

AWS Core Technologies - Security:

One of the most important concepts to understand. AWS is designed to help build secure, high-performing, resilient, and efficient infrastructure for applications.

Cloud Security on AWS:
    - Inherit benefits from AWS data center and network architecture
    - Similar to on-premises data centers, without maintaining facilities and hardware
    - Can be easily automated
    - Inherit all the best practices of AWS
    - AWS cloud is often safer than most environments

AWS offers security, identity and compliance services. Multiple categories contains multiple services:

- Data Protection:
    - Amazon Macie
    - AWS CloudHSM
    - AWS Secrets Manager
    - AWS KMS
    - AWS Certificate Manager
- Incident Response:
    - Amazon Detective
    - CloudEndure Disaster Recovery
- Detection:
    - Amazon GuardDuty
    - Amazon Inspector
    - AWS CloudTrail
    - AWS Security Hub
    - AWS Config
    - AWS IoT Device Defender
- Identity & Access Management:
    - AWS IAM
    - AWS Single Sign-on
    - AWS Organizations
    - AWS Resource Access Manager
    - AWS Directory Service
    - Amazon Cognito
- Infrastructure Protection:
    - AWS Network Firewall
    - AWS Shield
    - AWS WAF
    - AWS Firewall Manager
- Compliance:
    - AWS Artifact
    - AWS Audit Manager

AWS shared responsibility model:

- AWS is responsible for the security OF the Cloud
- Customers and APN partners are responsible for security IN the Cloud

Amazon Identity and Access Management (IAM):

Securely manage access to AWS services and resources.

- Fine-grained access control to AWS resources
- Multi-factor authentication
- The ability to analyze access
- Integration with corporate directories

AWS Cloud compliance (guidance):

Environments are continuously audited with certifications from accreditation bodies across geographies and verticals.
 
AWS Management Interfaces:

AWS contains 3 main interfaces:

AWS Management Console: Graphical web interface to facilitate cloud management
Command Line Interface (AWS CLI): Access to services via commands
Software Development Kits (SDKs): Access to services in your code (apis for ex)

AWS service breadth and depth:

Foundation Services:

Compute
Networking
Storage
(Less but important, Databases and Security)

Products and Services:

Databases
- Relational
- NoSQL
- Caching
Analytics
- Cluster computing
- Real time
- Data warehouse
- Data workflows
App Services
- Queuing
- Orchestration
- App streaming
- Transcoding
- Email
- Search
Deployment and Management
- Containers
- DevOps tools
- Resource templates
- Usage tracking
- Monitoring and logs
Mobile Services
- Identity
- Sync
- Mobile analytics
- Notifications

Infrastructure: 

Region
Availability Zone
Edge Locations

 End of Introduction to AWS Core Technologies
——————————————————————————————————————————————————————————————————————————————————————————————————————————————

Introduction to solution design

AWS Solutions

- Machine Learning
- Analytics & Data Lakes
- Internet of Things (IOT)
- Serverless Computing
- Containers
- Enterprise Applications
- Storage
- Windows Workloads

Migration Strategies

The Seven R’s

- Rehost
- Replatform
- Relocate
- Refactor
- Retire
- Retain
- Repurchase

Migrating Workloads to the AWS Cloud:

Rehost: lift and shift

- Recreating the on-premises network, only on AWS Cloud
- Automating with tools such as AWS Application Migration Service
- Easier to optimize and re-architect applications after migration

Relocate: hypervisor-level lift and shift

- Migration specific to VMware Cloud on AWS
- Example: Migrate hypervisor host Oracle database to VMware Cloud on AWS

Replatform: lift, tinker and shift

- Retaining the core architecture
- Making targeted AWS cloud optimizations
- Examples:
    - Migrating databases to Amazon RDS
    - Migrating applications to Amazon Elastic Beanstalk
    - Migrating file saving to S3 Bucket

Refactor: modernize

- Re-imagining how the application is architected and developed
- Using cloud-native features

Other strategies:

Retire: 

- Shutting off non-useful applications
- Reducing spend, management and security

Retain/Revisit:

- Keeping certain application on-premise

Repurchase:

- Moving workflows to software as a service (SaaS)

Cloud Architecture Best Practices

- Design for failure and nothing fails:
    - Avoid single points of failure
    - Design using multiple instances
    - Design using multiple Availability Zones
    - Separate single server into multiple tiered application
    - For Amazon RDS, use the Multi-AZ feature

- Build Security in every layer:
    - Encrypt Data at rest and in transit
    - Enforce principle of least privilege in IAM
    - Implement both Security Groups and Network Access Control Lists (NACL)
    - Consider advanced security features and services

- Leverage different storage options:
    - Move static web assets to Amazon S3
    - Use Amazon CloudFront to serve globally
    - Store session state in DynamoDB
    - Use ElastiCache between hosts and databases

- Implement elasticity:
    - Implement Auto Scaling policies
    - Architect resiliency to reboot and relaunch
    - Leverage managed services like Amazon S3 and Amazon DynamoDB

- Think parallel: 
    - Scale horizontally, not vertically
    - Decouple compute from session/state
    - Use Elastic Load Balancing
    - Right-size your infrastructure

- Loose coupling sets you free:
    - Instead of a single, ordered workflows, use multiple queues
    - Use Amazon Simple Queue Service and Simple Notification Service (SQS and SNS)
    - Leverage existing services

- Don’t fear constraints:
    - Rethink traditional constraints
    - Need more RAM? Consider distributing load across a number of commodity instances
    - Better IOPS (input/output operations per second) for databases? Consider scaling horizontally by spreading the load around. Consider creating a read replica for your database and modifying your application to separate database reads from writes.
    - Response to failure (hardware failure or config corruption for example)? Favor a rip-and-replace approach. Simply decommission the entire component and spin up a fully functional replacement.

The AWS Well-Architected Framework

A framework for ensuring infrastructures are:

    - Secure
    - High-performing
    - Resilient
    - Efficient
    - Sustainable

- Practices Developed through reviewing customers’ architectures on AWS
- Systematic approach for evaluating and implementing architectures
- There is a Well-Architected Tool in the console

The six pillars:

- Operational Excellence
- Security
- Reliability
- Performance Efficiency 
- Cost Optimization
- Sustainability

AWS Cloud Adoption Framework (AWS CAF)

The AWS Professional Services team created the AWS CAF. It enables smooth migration to AWS.

It is divided by capabilities:

- Business Capabilities: 
    - Business:
        - Ensure IT aligns with business
        - Creates a strong business case for cloud adoption
        - Ensure business align with IT
        - Common roles include:
            - Business managers
            - Finance managers
            - Budget owners
            - Strategy stakeholders
    - People:
        - Support change management strategy
        - Evaluate organizational structures and roles
        - Evaluate new skill and process requirements
        - Identify gaps
        - Prioritize training
        - Common roles:
            - Human resources (HR)
            - Staffing
            - People managers
    - Governance:
        - Focus on skills and processes
        - Ensure the business values are maximized and risks are minimized
        - Update the staff skills and processes
        - Measure cloud investments to evaluate business outcomes
        - Common roles:
            - Chief information officer (CIO)
            - Program managers
            - Enterprise architects
            - Business analysts 
            - Portfolio managers

- Technical Capabilities:
    - Platform:
        - Implement new solutions in the cloud
        - Migrate on-premises workloads to the cloud
        - Understand and communicate the structure of IT systems and their relationships
        - Describe the architecture of the target state environment in detail
        - Common roles:
            - Chief technology officer (CTO)
            - IT managers
            - Solutions architects
    - Security:
        - Meet security objectives for visibility, audibility, control and agility
        - Structure the selection and implementation of security controls
        - Common roles:
            - Chief information security officer (CISO)
            - IT security managers
            - IT security analysts
    - Operations:
        - Enable, run, use, operate, and recover IT workloads
        - Define how business is conducted
        - Align with and support the business operations
        - Define current operating procedures
        - Common roles:
            - IT operations managers
            - IT support managers

Action Plan:

- Uncover gaps in skills and processes
- Use inputs as basis for creating AWS CAF Action Plan
- Guide an organization’s change management
- Keep on track toward achieving their desired outcomes

Case studies:

You can see some exemples of real Case Studies on aws.amazon.com/solutions/case-studies

AWS Solution:

Vetted, technical reference implementations designed to help customers solve common problems and build faster

AWS Solution Space:

Provides customers who need help deploying an AWS Solution by highlighting AWS Competency Partner Solutions

Solution Space Categories:

- Solution Brief: Technical overview of APN Partner solution
- Consulting Offer: Proof of concept of APN Partner solution
- Quick Start: APN Partner solution deployment guide

See some quick start solutions on aws.amazon.com/quickstart


 End of Introduction to Solution Design
——————————————————————————————————————————————————————————————————————————————————————————————————————————————

Presenting AWS Solutions to Customers

Customer-facing discussions fall into three distinct categories, based upon typical milestones in the sales cycle.

1. Discovery is the information-gathering meeting to help you understand your customer’s challenges.
2. After all the necessary information is collected that identifies the customer’s goals and pain points, you will meet with the customer again to present your findings and propose one or more AWS solutions. This may actually end up being several meetings, depending on whether tweaks to the solution are needed.
3. After the customer agrees to a potential solution, you will ask them if they would like to move forward with a proof of concept (POC), where they evaluate the solution in their own environment. 

Preparing for Discovery

- Research customer’s business
- Determine market segment
- Identify industry trends
- Identify customer’s competitors
- Research recent news
- Research customer relationship to AWS

Use your knowledge to encourage a detailed conversation, asking targeted questions and open-ended questions (avoid yes/no questions).

Five whys is a good practice, dive deeper, uncover the real desired outcomes.

Whiteboarding is another good practice, keeping track of the conversation, illustrating workflows and ideation.

Objection handling best practices

- Data-driven approach
- Use case studies
- Dive deep
- Have backbone (have confidence on your responses or assure that you will find an answer to their questions)
- Keep the momentum going

Handling objections = Connect (understand customer objection) -> Condense (understand exactly what is bothering) -> Continue (respond the question with some of the best practices above and continue the presentation)

Common objection responses

- Security:
    - Security at AWS is our top priority
    - Higher security posture than in legacy environments
    - All customers inherit all the benefits of our experience
    - Validated against the strictest of third-party assurance frameworks

- Cost or cost savings:
    - Reduce total cost of ownership (TCO)
    - Achieve continuously optimized and predictable spend
    - No longer over provision infrastructure for peak demand
    - GE Oil and Gas decreased TCO by 52%

- Scalability and Response
    - Build Cloud Foundation Team
    - Create guardrails around security, availability, reliability and compliance
    - AWS Control Tower gives maximum control–without sacrificing speed and agility

What NOT to do when meeting a customer:

- Avoid using words like definitely, never or guaranteed.
- Avoid using acronyms or technical jargon (unless you heard them using them as well).
- Don’t focus on technology, focus should be customer centered.
- Do not focus on the short/mid-term.
- Avoid reading the slides, maintaining eye contact with the customer and not the screen.

Proof-of-Concept (POC)

POC Fundamentals:

- Practical example of solution
- Evaluation mechanism
- Educational tool

Building a POC:

- Start building only after the customer agrees to move forward with a POC
- Determine what success looks like (make sure there are clear goals and scope defined for the POC)
- Include any modifications that show up during the presentations
- Consult as necessary (consult someone that has more business or technical expertise when needed)
- Collect the following information before starting:
    - Networking and security
    - Application code
    - Databases
    - Data

Resources for Proofs of Concept

- Skills: 
    - Building on AWS
    - Migrating data
    - Validation and testing

- Resources:
    - Cost of running POC

AWS contains partner training that can help you design and create a POC.

AWS Quick Starts:

- Rapidly deploy architectures based upon best practices
- Launch, configure and run AWS services required to deploy a specific workload on AWS
- Reduce manual procedures into few steps
- Check back frequently for updates

Partner Opportunity Acceleration (POA) Program:

Helps APN partners to present your expertise and earn customer trust.

- Accelerate sales cycles and customer adoption
- Co-invest with you
- AWS promotional credits
- Cash reimbursements
- Expectations and requirements


 End of Presenting AWS Solutions to Customers
——————————————————————————————————————————————————————————————————————————————————————————————————————————————

Look Ahead (Migration & Beyond)

Three phase migration process

Assessment:

- Identify your customer’s readiness for operating in the cloud
- Identify potential business outcome

Readiness and Planning:

- Address gaps in your customer’s readiness that were uncovered in your assessment phase
- Analyze their environment, create a map of interdependencies
- Determine migration strategies, such as repost or replatform
- At this stage , you set up a secure and well-architected multi-account AWS environment (called an AWS Landing Zone)

Migration and Modernization:

- In the migration phase, the focus shifts from the portfolio level to the individual application level
- Each application is designed, migrated and validated
- Automatic or manual migration from different source environments, such as physical, virtual or cloud-based to AWS
- You likely require a one-time migration of a large volume of data to AWS 

Minimum Viable Product (MVP)

A functional product or solution with just enough features to satisfy requirements.

- Don’t scale MVPs
- MVPs are production level solutions to validate an implementation
- Avoid Big Bang solutions, start with basic stuff and gather feedback
- A POC is more like a quick demo of the solution, whereas an MVP is production level

Migration Strategies

Determine the migration path:

- Rehost:
    - Choose manual or automate path
        - If manual then you would: Manually install, config and deploy of the app components
        - If automate, you just gotta use the migration tools

- Replatform or lift, shift and tinker:
    - Determine new platform for the application, then modify underlying infrastructure to prepare for migration to the cloud, then use the migration tools

- Refactor:
    - Require many more steps by nature
        - The application needs to be redesigned for the target architecture and infrastructure
        - Develop the code for the target architecture
        - Then a full Application Lifecycle Management (ALM) or a Software Development Lifecycle (SDLC) must be complete
        - Followed by the integration of the target application


Once the strategy is chosen and applied, the applications would:

- Validation: Applications validated on AWS
- Transition: Then production would be transitioned
- Production: Finally, full production achieved on AWS

Going to Production:

Best Practices:

- Involve AWS account team (Solutions Architect or Technical Account Manager)
- Customer-specific regulatory requirements
- AWS Support level (depends on the customer selection)

It’s good to run a periodic Well Architected Review (using the AWS Well-Architected Tool, it can be performed by APN Partners or the customers themselves), it provides:

- Architectural guidance
- Continuous review
- Identify and implement improvements

Modernize to drive growth - Other Ways to Modernize Customer’s Solutions

- Retire expensive legacy solutions
- Reduce TCO, improve cost optimization
- Gain agility through automation
- Free up resources to drive innovation

Containers:

- Package code, configurations, dependencies, and runtime engines into a single object
- Share an operating system installed on the server
- Run as resource-isolated processes, ensuring quick, reliable and consistent deployments regardless of environment
- AWS offers resources and orchestration services that make it easy for you to build and run containerized applications in production 

Use cases:

- Microservices: Provide process isolation, that makes it easy to break apart and run application as independent component (called microservices)
- Batch processing: Package batch processing and ETL jobs into containers to start jobs quickly and scale them dynamically in response to demand
- Machine learning: Quickly scale machine learning models for training and inference and run them close to data sources on any platform
- Hybrid applications: Let customers standardize how code is deployed, making it easy to build workflows applications that run between on-premisses and cloud environment
- Application migration to the cloud: Easy to package entire applications and move them to the cloud without needing to make any code changes
- Platform as a service: Used to build platforms that remove the need for developers to mangasse infra and standardize how applications are deployed and managed

Serverless:

Serverless applications don’t require provisioning, maintaining and administering servers for backend components, such as compute, database, storage, stream processing, message queuing, and more.

- AWS provides a set of fully managed services for serverless applications:
    - AWS Lambda
    - Lambda@Edge
    - AWS Fargate
    - Amazon Simple Storage Service
    - Amazon Elastic File System
    - Amazon DynamoDB
    - Amazon Aurora Serverless
    - Amazon API Gateway
    - Amazon SNS
    - Amazon SQS
    - AWS AppSync
    - Amazon EventBridge
    - AWS Step Functions
    - Amazon Kinesis
    - Amazon Athena
    - Developer Tooling: Various tools and services…

Analytics and Data Lakes:

Data lakes can be used to make it easier to read data and obtain insights. AWS provides the most comprehensive set of services to move, set and analyze your data. 

Data lakes and analytics solutions on AWS:

- Interactive Analytics: Amazon Athena
- Big Data Processing: Amazon EMR
- Data Warehousing: Amazon Redshift
- Real-time Analytics: Amazon Kinesis
- Operational Analytics: Amazon OpenSearch Service
- Dashboards and Visualizations: Amazon QuickSight
- Cataloging and Securing: AWS Lake Formation

 End of Look Ahead (Migration & Beyond)
——————————————————————————————————————————————————————————————————————————————————————————————————————————————

AWS Partner Network (APN)

Some APN benefits:
- Leverage AWS innovation
- Access tools and resources
- Expand addressable market

AWS Technical Professional Learning Path:

Cloud Fundamentals (Recommended Progression):

- AWS Partner: Accreditation
- AWS Partner: Cloud Economics Accreditation
- AWS Partner: Cloud Practitioner Essentials
- AWS Certified Cloud Practitioner 
- AWS Partners Well-Architected Best Practices (Technical)
- AWS Certified Solutions Architect - Associate Learning Path
- AWS Professional Services: Cloud adoption Framework
- AWS Certified Solutions Architect or AWS Certified Developer

APN Partner Central:

Provides APN Partners with the tools and content they need to grow their businesses on AWS

 End of AWS Partner Network
——————————————————————————————————————————————————————————————————————————————————————————————————————————————

Course Summary:

* The AWS Cloud value proposition
* Core services and functionality
* Solving customer business challenges
* Architectural best practices
* Presenting solutions
* Proofs of concept
* Guiding customers toward modernization
* APN resources



