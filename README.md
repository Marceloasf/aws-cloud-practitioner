# AWS Partner: Accreditation (Technical)

The AWS Partner: Accreditation (Technical) training provides AWS Partner Network (APN) Partners with fundamental, technical knowledge of AWS cloud computing, global infrastructure, services, solutions, migration, and security. This course is designed to teach students the fundamental principles of AWS solution architecture design and to introduce the basic skills needed to engage customers in a pre-sales AWS technical opportunity. It is intended to empower learners to make recommendations and informed decisions about AWS cloud solutions based on customer business requirements. Upon successful completion of the accreditation test, you will earn accreditation as an AWS Technical Professional.

Course Summary:

* The AWS Cloud value proposition
* Core services and functionality
* Solving customer business challenges
* Architectural best practices
* Presenting solutions
* Proofs of concept
* Guiding customers toward modernization
* APN resources

Benefits of cloud computing:

Agility: Cloud provides more resources to organizations
Elasticity: Resources can be provisioned with the amount of resources that are actually needed
Cost Savings: Only pay for IT as it its consumed (pay-as-you-go pricing)
Deploy globally in minutes: Can deploy an application in multiple locations with a few clicks

AWS Regions:

Completely isolated from each other
Certain resources are tied to regions

AWS Availability Zones:

All AZs (availability zones) are connected to the same region, but they are separated in Datacenters within each AZ, for example: 
- AP-SOUTHEAST-1 (AZ within Singapore region) is divided in 3 datacenters:  
    - AP-SOUTHEAST-1a, AP-SOUTHEAST-1b and AP-SOUTHEAST-1c

Other AWS global infrastructure:

Local Zone - Literally local zones, like inside an industry, city, etc
Wavelength Zones - 5G zones 
Direct Connect Locations - Customer internet connects directly to AWS 
Edge Locations - CloudFlare - Called “EDGE”, but are located in specific centers providing lower latency (for example inside a capital city) - Locations designed to deliver content to end users
Regional Edge Caches - CloudFlare

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

- General Purpose - Balanced specs (CPU, RAM, Storage)
- Compute Optimized - More cpu bound
- Memory Optimized - More memory bound (RAM)
- Accelerated Computing - More cores for more processing power (used in IA, machine learning, float number calculations)
- Storage Optimized - More storage and I/O bound

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
- Specify the Amazon VPC (all the virtual network) and subnets (must select at least 2 subnets across different availability zones)

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

- Don’t scale MVPs to final products
- MVPs are production level solutions to validate an implementation
- Avoid Big Bang solutions, start with basic stuff and gather feedback
- A POC is more like a quick demo of the solution, whereas an MVP is production level

Migration Strategies

Determine the migration path:

- Rehost:
    - Choose manual or automate path:
        - If manual then you would: Manually install, config and deploy the app components
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

- Microservices: Provide process isolation, that makes it easy to break apart and run a application as independent components (called microservices)
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
- AWS Certified Solutions Architect then AWS Certified Developer

To become an AWS Partner, there are some steps:

1. Registered
2. Enrolled
3. Confirmed
4. Validated: This one is the most important of them all, because here is where the partner earns the bulk of the benefits
5. Differentiated

APN Partner Central:

Provides APN Partners with the tools and content they need to grow their businesses on AWS

 End of AWS Partner Network
——————————————————————————————————————————————————————————————————————————————————————————————————————————————

# AWS Partner: Cloud Economics (Accreditation) 

In this course, you will explore the concepts of business value, including cost savings, staff productivity, operational resilience, and business agility. In addition, you will learn about the Migration Portfolio Assessment, or MPA, tool. And finally, you will learn about key elements of cloud financial management. 

* Business value
    * Introduction to business value
    * Cost savings
    * Staff productivity 
    * Operational resilience
    * Business agility
* Cloud Financial Management
* Migration Portfolio Assessment (MPA) tool
    * Introduction to MPA tool
    * Conducting a Cost Savings analysis with MPA

Cloud Economics: Two Primary focus areas

Business Value (TCO)

* Discuss with customers before a sale to help them understand the value of AWS and how AWS will improve all aspects of their business’s performance and user experience
* Also known as Total Cost of Ownership

Cloud Financial Management

* Focus on helping customers on financially managing their cloud infrastructure


Introduction to Business Value

Value is delivered to the customer by:
* Proofs of concept (POC)
* Architectural Reviews
* Migration of workloads

Cloud Value Framework

Consists of 4 pillars:

1. Cost savings (TCO)
2. Staff productivity
3. Operational resilience
4. Business agility

Always emphasize all 4 pillars to your customers.

TCO: Referred as cost savings on AWS. Represents the cost benefits of moving to the cloud. (51% lower overall cost on running AWS about 5 years compared to on-premisses services)

Staff productivity: Efficiency gained from reducing or eliminating tasks no longer needed with the cloud. (62% greater staff efficiency with AWS)

Operational resilience: More uptime, less downtime and decreased risk. (Reduced by 32% by moving workloads from on-premisses to AWS Cloud)

Business agility: Customer can deliver more value to their customers.

* Cloud economics = Business value and cloud financial management
* Business value is more than just up from cost 

End of Introduction to Business Value
———————————————————————————————————————————————

Cost Savings Analysis

Help a customer compare costs and build a business case for transitioning to AWS. A cost savings analysis calculates the total cost of ownership, acquisition and operating costs for running an end to end traditional IT environment on-premises versus deploying to AWS.

Equal or improved performance does not mean the same volume of on premises resources. A typical on-premises data center requires fewer cores on AWS, because there’s no need to provision for peek, backup, clustering or future uses such as research. 
* The typical AWS deployment requires 20%-40% less cores

Following are some ways that AWS reduces TCO.

Consumption-based model

Pay only for what you use, instead of paying for what you thing you might need in the future.

Overprovision vs. underprovision:

When the customers over provision, they order more servers than they need, ending up with unused resources.

When they under provision, they order too few servers, and fail to deliver on their service level agreements (SLAs).

In both cases the trade off is inefficiency and financial loss.

AWS helps customers avoid inefficiencies and financial losses by enabling them to launch the infrastructure they need, when they need it.

AWS Pricing Models

Customers can optimize expenditure by matching the usage model to the requirements of workloads by maturity and behavior.

* On-Demand
* Reserved
* Spot
* Dedicated

Maturity = Enough data? Does the customer have enough data to determine a usage baseline so they can use a reserved instance

Behavior = Data use to spiky? Is data usage too spiky for reserved instances. Will spot instances work better?

Typically customers start with on demand instances to gauge their need and then switch to reserved instances or RIs once they know their demand base line. 
*  Reserved instances can decrease cost by up to 75% versus on demand
* Spot Instances are AWS access capacity sold for a deep discount, reducing costs even further 

Price Reductions

Higher efficiency and lower price.

Every time AWS reduce their prices, all AWS customers experience the savings immediately. Customers never need to call AWS, contact an account manager, renegotiate a contract or ask for the price reduction.

One exception to price reductions is reserved instances (RIs). RIs are already heavily discounted, with prices accounting for forecasted future discounts.

AWS Flywheel

Flywheel cycle:
* Reduced prices -> More customers -> More AWS usage -> More infrastructure -> Economies of scale -> Lower infrastructure -> Reduce prices …

Migration Challenges and Costs for Customers

* Migration-related costs
* Shifting to an operational expenditure (opEx) model
* Lack of cloud readiness
* Entrenched IT organization

Sunk infrastructure costs: Customer’s hardware is fully depreciated, and the company is not close to a hardware refresh

Cost (and effort) of migration and decommissioning: Customer’s existing footprint is moved to the cloud and the data center is shut down, which requires significant time and effort.

Migration Costs formula: Cost savings / Sunk costs + Migration costs = Return on investment (ROI)

Define the ROI with the customer.

Sunk Cost

To calculate it, ask the accounting department for non-depreciated assets for the hardware that is being evaluated. Evaluate the sunk costs for two factors: depreciation and recovery value.

Depreciation: Was the asset’s depreciation considered?
Recovery value: Can any value be recovered by selling the asset?

Cloud Readiness

The lack of cloud readiness is a challenge for customers:

* Human factor
    * The customers team lacks the skills and experience required to transition to the cloud
* Applications
    * The customers legacy applications or workloads are not ready for (or would not immediately benefit from) moving to the cloud

App Readiness Questions
* What are your application dependencies?
* What apps are communicating with other apps?
* What apps can be translated easily?

Entrenched IT department can be a challenge on a migration. Where the IT organization feels threatened by perceived loss of control or potential staff reductions. Sometimes finding one or two key players on the company who understand the value of cloud adoption, can help move a migration forward.

Stakeholders

Cost savings engagement may require multiple discussions with different messages for different audiences:

* Application developer (DevOps): Focus mostly on technical specs and features that will simplify their lives, in most cases cost is not a major problem for them.
* IT support team: Changes they’ll have to make to support the new cloud environment, might also focus on the costs of the change.
* Procurement team: Focus on pricing and payment models, need help to understand and adapt to consuming IT as a service using the pay-as-you-go model.
* CFO/CIO/Investors: Focus on the big picture, bottom line, and growing the business and revenue.

Each audience will have unique perspectives on cost savings.

CapEx and OpEx defined

CapEx is defined as business expenses incurred in order to create long-term benefits in the future, such as purchasing fixed assets like a building or equipment. Some examples of IT items that fall under this category would be whole systems and servers, printers and scanners, or air conditioners and generators. You buy these items once and they benefit your business for many, many years. Maintenance of such items is also considered CapEx, as it extends their lifetime and usefulness.

OpEx is your operating costs, the expenses to run day-to-day business, like services and consumable items that get used up and are paid for according to use. This includes printer cartridges and paper, electricity, and even yearly services like website hosting or domain registrations. These things are necessary for your business’s success but are not considered major long-term investments like CapEx items.

Customer Cost Savings Analysis Best Practices

What works:
* Make sure you have the right stakeholders in the room to discuss the cost analysis (finance, procurement, IT support, engineering).
* Work collaboratively with the customer, gaining support from leadership is crucial for successful cloud migration.
* Use realistic usage percentages (%).
* Assign cost/value to business-value factors, such as agility and risk.

Does not work:
* Focus purely on pricing and discounts, rather than cost analysis. A pricing discussion is not a costs saving discussion. Only bring discounts after the analysis is done, so you can show how AWS is even cheaper with the cost savings.
* Compare a duplicate of an on-premises environment—problematic apples-to-apples comparisons of machines.
* Allow all decisions and vision to be based on an unchecked cost analysis, and fail to capture the true costs of IT, data center, and on-premisses. Don’t have only one person running the cost analysis.
* Bring up the cost savings discussions late in the decision-making process. 
* Don’t conduct a cost savings analysis unless the customer asks for one. 

Cost Savings Analysis Best Practices

What works:
* 3 or 5 year depreciation
* 3 year RI
* Use volume RI discounts
* Use realistic on-premises rations (VM density, servers, racks)
* Explore on-premises CPU and met usage
* Apply cost benefits of automation (automatic scaling, APIs, AWS Trusted Advisor, Cost Optimization)
 Does not work:
* Forget power/cooling (compute, storage, network)
* Forget administration costs (procurement, design, build, operations, network, security)
* Forget rent/real estate (building depreciation, taxes, shared services staff)
* Forget software and hardware maintenance costs
* Forget the cost of redundancy

Always address overhead costs.

Engagement Process

A typical engagement process takes from one to two months to complete.

Kickoff (meeting): 
* Cost savings overview
* Timeline, scope and roles
* Identify customer important factors as they evaluate moving to AWS
    * For ex.: Are they moving to AWS for cost saving or are there any other reasons? 
* Stakeholders are included in this meeting and they all should have a role

Data collection (2-4 weeks):
* This can be the most time-consuming part of the process

Initial assessment:
* Review data
* Initial assessment
* ID open questions, assumptions

Q&A (~1 week):
* Answer customer’s questions

Full assessment: 
* Incorporate new data
* Repeat as needed

Iterate and finalize (~1 week):
* You and your customer can iterate as often as needed to finalize the process

Customer report out:
* Last but not least, the customer can communicate internally about the process

Resources for your customers

* AWS TCO Calculator
* AWS Economics Center
* Case Studies and Research

TSO Logic

* On-premises analysis and cloud planning
    * Automated agentões data discovery or flat file Ingest
    * Identifies on-premises compute, attached storage, memory and Microsoft licenses
    * Evaluates multiple future-state scenarios based on location, purchase type, utilization and other inputs
    * Right-sizes over provisioned resources to realize historically validated savings
    * Available to partners that meet certain qualifications

Migration Portfolio Assessment Tool

* Guided data ingestion
* Right-sized EC2 instance and storage recommendations
* Run rate cost comparison 
* Over 100 variables with repopulated industry defaults
* Migration pattern analysis and recommendation (7Rs)
* Migration estimating for resources, timelines, and costs
* Customizable dashboards to visualize data
* Secure access to APN Advanced and Premier Tiers

End of Cost Savings
———————————————————————————————————————————————

Staff Productivity

Typical functions:

* Server, Network, and Storage: involves managing hardware infrastructure
* Application: roles such as data base administrators, AppDev, QA, and support functions
* Facilities: facilities management for customers who have an on-premises data center
* Security: ensures infrastructure meets compliance, regulatory, and corporate standards

Almost all staff productivity is improved since on a cloud environment they don’t need to worry about physical problems on a server. The automation is another great factor that increases staff’s productivity. Focusing on other activities that will generate more value to their customers.

* Server benefits: Time spent installing, upgrading, and removing hardware is reduced by up to half
* Network benefits: Time spent on network planning and forecasting to provision hardware is greatly reduced
* Storage benefits: Time spent on supporting physical arrays is eliminated
* Application benefits: Time spent coding, testing, and supporting business apps is greatly reduced
* Facilities benefits: Time spent managing power and cooling systems are eliminated
* Security Benefits: Penetration testing, vulnerability scanning, and security audits are greatly improved


End of Staff Productivity
———————————————————————————————————————————————

Operational Resilience

Operational resilience equals availability and security. Availability envolves multiple layers.

Downtime

Downtime is the time the application is out of service and can impact a company in multiple ways. Downtime impacts are not cheap and it can cost from thousands to billions of dollars to a company. Here are some of the costs of downtime:

* Third-party fees
* Equipment replacement
* After-the-fact incidental costs
* Recovery activities and costs
* Detection costs associated with initial discovery and subsequent investigation
* Unproductive IT staff and end-user costs
* Lost revenue
* Business disruption costs

Downtime can occur because of security and lack of availability/stability on the server. Often occurs because the demand for services exceeds the infrastructure’s ability to meet the demand.

Cornerstones of Operational Resilience

* Operations
* Security
* Software
* Infrastructure

Operations: Causes of failure

Primary causes of operations failures:

* Human errors, such as lack of clearly defined procedures or user privilege 
* Configuration errors in hardware or operating system settings and startup scripts
* Procedural errors, like restoring the wrong backup or forgetting to restart a device
* Commonplace accidents in the data center, like tripping over power cords, dropping equipment, or disconnecting devices

How AWS Helps

* Leverages automation
* Manages services from end to end
* Provides system-wide visibility for usage, performance and operational metrics
* Enables security and governance configuration of AWS resources
* Monitors API access

Helps the customer focus primarly on their business.

Security: Causes for breaches

* Malware, such as worms, viruses and Trojan horses
* Network attacks, like open ports, SYN floods, and fragmented packets
* Unpatched applications or operating systems
* Security issues, such as password disclosures, social engineering, credentials not stored securely, non-strict password policies, and poor privilege and access management
* Poor or limited authentication

How AWS Helps

* AWS Shared responsibility model (AWS takes care of all the infrastructure and network of the cloud, while the customer takes care of what’s inside the cloud)
* Helps mitigate security risks with AWS automation and tools
* Provides built-in DDoS protection and security perimeter 
* Provides AWS Identity and Access Management (IAM) for centrally managing users and credentials
* Reduces or eliminates “rogue servers”
* Assists in building compliance-ready environments with over 30 compliance certifications and accreditations

Software: Causes for failure

* Resource exhaustion, like runaway processes, memory leaks, and file growth
* Computational or logic errors, such as faulty references, deallocated memory, corrupt pointers, sync errors, and race conditions
* Inadequate monitoring, such as the inability to identify issues
* Failed upgrades, such as inter-compatibility and integrations

How AWS Helps

* Offers blue/green deployments for quick rollbacks
* Automates continuous integration and continuous delivery workflow
* Runs smaller code deployments to reduce unit, integration and system bugs
* Provides current and secure resources with OS patching
* Creates and manages collections of related AWS resources

Infrastructure: Causes for failure

* Hardware failure of servers, storage, or networks
* Natural disaster, like hurricanes, floods and earthquakes
* Power outages, including failed power supplies and batteries
* Volumetric attacks, such as DDoS, Domain Name System (DNS) amplification, and UDP/ICMP floods

How AWS Helps

* Uses and improves AWS data centers on a large scale
* Enables customers to run applications and failover across multiple Availability Zones and Regions
* Provides highly available and durable systems
* Enables Availability Zones to redundantly connect to multiple tier-1 transit providers
* Uses two independent power sources for every instance, each with utility, UPS, and back-up generator

End of Operational Resilience
———————————————————————————————————————————————

Business Agility

It means bringing more value to customers. Letting our customers focus on building new projects, improving and expanding. Responding faster, experimenting more, and delivering results in the same or less amount of time.

AWS benchmarking insights (using AWS cloud):

* Accelerated time to market
* More features and fixes per release
* Increase in application revenue per user

Improved throughput (delivery) and quality (delivery quality)

Fail fast: Being able to easily shut down failed initiatives without the pain and wasted resources associated with an inflexible on-premises environment.

Key Performance Indicators (KPIs)

* New applications launched per year
* Adoption of new features
* Deployment frequency
* Employee retention

End of Business Agility
———————————————————————————————————————————————

Cloud Financial Management

Customers should pay for what they use and only for what they need to get their business done.

Four key areas:

* Measurement and Accountability: Establishing cost transparency, to ensure visibility into and accountability for spend. Enabling cost transparency and leveraging tools for measuring and monitoring costs and usage data.
* Cost Optimization: Identify waste, build cloud-friendly architectures that scale based on demand and improve cost efficiency.
* Planning and forecasting: Understand current and future costs and IT needs, driving accurate planning.
* Cloud financial operations: Identify and invest in people, processes, tools and automation.

Enabling cost transparency. Users can use custom cost allocation tags, so they can know where their investments are being made. Must-have tagging:

* Cost center
* Application or workload
* User
* Expiration date
* Automation

Measuring and monitoring tools:

* Cost and usage data
* Optimization recommendations
* Data-driven, cost-based decisions

Options:

1. DIY (do it yourself) - Build a custom dashboard
2. AWS Partner Network (APN) - AWS Cloud Management Tools (CMT)
3. AWS Tools - AWS Cost Explorer (free tool)

Cost optimization best practices

* Right-sizing instances
    * Select the lowest cost instance available that meets performance requirements
    * Look at CPU, RAM, storage, and network usage to identify potential instances that can be downsized
    * Use Amazon CloudWatch metrics and set up custom RAM metrics
    * AWS Cost Explorer identifies rightsizing opportunities
* Increasing elasticity
    * Turn off non-production instances
    * Look for dev/test, non-production instances that are running always-on and turn them off
    * AWS Lambda + CloudWatch = Automated Scheduling
    * Automatically scale production
    * Use automatic scaling to scale up and down based on demand and usage (for example, spikes)
* Choosing the right pricing model (instances and other services)
    * Reserved Instances (RIs): Up to 75% savings in some cases
* Optimizing storage
    * S3 Intelligent-tiering over standard - there is no extra cost and it saves money because hit understand your usage and switch the type of service used

Amazon EC2 Purchase Options

On-Demand Instances
* Pay for compute capacity by the second with no long-term commitments
    * Spiky workloads, to define needs
Reserved Instances
* Make a 1 or 3-year commitment and receive a significant discount off On-Demand prices
    * Committed & steady-state usage
Spot Instances
* Spare EC2 capacity at savings of up to 90% off On-Demand prices
    * Fault-tolerant, flexible, stateless workloads

They are all the same compute infrastructure, but the diference is the contract and the way that they work.

It’s recommended by AWS to balance your instances types. Use all three of them.

Reserved Instances

* Instances target for applications that must run all of the time, like a production app for example.
* There are other services that offer RIs besides EC2, for example Amazon ECS and Amazon RDS.

Regional RIs simplify optimization:
* Capacity reservation: Capacity reservation in a specific AZ (in a specified AZ).
* Availability Zone flexibility: The reserved instance discount applies to instance usage in any Availability Zone in a Region.
* Instance size flexibility: The reserved instance discount applies to instance usage regardless of size, within the instance family. Only supported on Linux/Unix Reserved Instances with default tenancy (in a specified Region). 

AWS Cost Explorer identifies RI savings opportunities

On-demand capacity reservations:
* Combine regional RIs with capacity reservations to benefit from billing discounts
    * Ensures access to EC2 capacity
    * Flexibility
    * Ability to cancel and cease charges

Capacity reservation pricing:
* A capacity reservation is charged the equivalent on-demand rate.
* Unused reservation on the customer’s EC2 bill. Only pay for the instance, not the reservation.

Capacity reservations: Restrictions
* Zonal RI billing discounts do not apply to capacity reservations
* Capacity reservations can’t be created in placement groups
* Capacity reservations can’t be used with dedicated hosts

Customers cannot modify reservations across families, sizes, operating systems and tenancy on common RIs.

Convertible Reserved Instance:
* Convertible RIs give customers the ability to modify reservations across families, sizes, operating systems and tenancy. 
    * The only aspect customers cannot modify is the region.
* Maximize flexibility and increase savings. 

Exchange a Convertible RI:
* Customers can exchange to the same value or higher of Convertible RIs
* For smaller instances, customers can split Convertible RIs first
* Converted RIs retain the expiration date of the original RIs
* Converted RIs must have the same term as the original RIs
* When exchanging a group of Convertible RIs:
    * Converted RIs have the latest expiration date of the whole group
    * In case of multiple terms, converted RIs will be 3-year RIs

Amazon EC2 Spot Instances

Good instance type for saving money and time. The customer can increase compute power with the same price and even having a cost reduction depending on the case, since spot instances are way cheaper.

Simple Spot Instances rules:
1. Spot infrastructure: Same as On-Demand and RIs: Same hardware, same capabilities, same instances, same geo footprint (Regions and AZs) but AWS can reclaim the instances with 2 minutes notice.
2. Spot pricing: Set it and forget it pricing—NO BIDDING, big savings (70-90% off).
3. Diversify: Use diverse instance fleets (instance types and sizes) to spin up 1 MM core (60,000+ instances) clusters.

Spare on-demand capacity: If AWS has a spike in requests in the on-demand space, AWS reclaims spot instances with a two minute notification.

* Minimal Interruptions: Over 95% of the instances were not interrupted in a 3 month period.

The work you are doing to make your applications fault-tolerant also prepares you for spot.

* Spot is optimized for stateless, fault-tolerant or flexible workloads
* Any application that can have part of all of the work paused and resumed or restored can use Spot

One way to handle interruptions: 
* Check for 2-minute interruption notification via instance metadata or Amazon CloudWatch events and automate by:
    * Checkpointing
    * Draining from Elastic Load Balancing (ELB)
    * Using stop-start and hibernate to restart faster
        * There are example scripts provided by AWS

* Stop/Start: Means customers would be able to persist an EBS volume if an instance is interrupted and when that instance becomes available again, it will reattach to that EBS volume and continue on with the work where the customer left off.
* Hibernate: Allows customers to flush in-state memory to disk.

EC2 Fleet with EC2 Auto Scaling

Automatically provision and scale instances across instance families and purchase models Auto scaling in a single Auto Scaling group.

Lowest Cost

Specify what percentage of your Auto Scaling group capacity should be fulfilled by On-Demand Instances, and Spot Instances to optimize cost.

Prioritized List

Use for On-Demand Instance types to scale capacity during an urgent, unpredictable event to optimize performance.

* Reduce cost
* Optimize performance
* Eliminate operational overhead

Plan and Forecast: AWS Pricing Calculator

AWS tools and services that estimate net new spend:
1. AWS Pricing Calculator: https://calculator.aws/#/
2. AWS service pricing pages: All services have pricing pages
3. AWS Price List API: Customers can setup notification when AWS change prices: https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/price-changes.html
4. AWS Cost Explorer
5. Migration Portfolio Assessment (MPA)

Cloud Financial Operations

Customer should create a Center of Excellence or COE in their companies. This team is responsible for:
* Align incentives
* Automate
* Report
* Control and governance
* Metrics and key performance indicators (KPIs)
* Bridge the gap between finance and IT (cloud)

The idea here is having a team that is specialized in cloud and that we can use them to align the financial and IT teams of the company. We can ask them more technical questions that can improve the company AWS Cloud usage.

Establish Clear Metrics and Targets

Customers should establish metrics and targets. Define success by establishing metrics and track progress.

Value-based optimization metrics: Unit cost = total cost / individual or unit cost

Other examples:
* Unit cost per customer or active subscriber
* Unit cost per revenue generated
* Unit cost per product or business unit
* Unit cost per internal user
* Unit cost per experiment
* Unit cost per full-time employee (FTE)

Using these metrics to understand why their bill is going up, even when optimization is improving.

Use and Build Tools

Customers must automate as much as they can. 

Building and automating their own tools:
* Identify always-on instances and recommend RI purchases
* Identify instances to downsize
* Automate idle instances and Amazon EBS volumes shut-down
* Automate storage aging from Amazon S3 to Amazon S3-IA, and then Amazon S3 Glacier
* Dashboard on status
* Report on savings

https://aws.amazon.com/solutions/implementations/instance-scheduler/

Buying and using some automation tools: 
* https://aws.amazon.com/products/management-tools/partner-solutions/?partner-solutions-cards.sort-by=item.additionalFields.partnerNameLower&partner-solutions-cards.sort-order=asc&awsf.partner-solutions-filter-partner-type=*all&awsf.Filter%20Name%3A%20partner-solutions-filter-partner-use-case=*all&awsf.partner-solutions-filter-partner-location=*all

End of Cloud Financial Management
———————————————————————————————————————————————

Migration Portfolio Assessment (MPA)


 

