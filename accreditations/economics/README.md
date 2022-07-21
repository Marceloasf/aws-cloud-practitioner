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

## Cloud Economics: Two Primary focus areas

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

## Cost Savings Analysis

Help a customer compare costs and build a business case for transitioning to AWS. A cost savings analysis calculates the total cost of ownership, acquisition and operating costs for running an end to end traditional IT environment on-premises versus deploying to AWS.

Equal or improved performance does not mean the same volume of on premises resources. A typical on-premises data center requires fewer cores on AWS, because there’s no need to provision for peek, backup, clustering or future uses such as research. 
* The typical AWS deployment requires 20-40% less cores

Following are some ways that AWS reduces TCO.

Consumption-based model

Pay only for what you use, instead of paying for what you thing you might need in the future.

Overprovision vs. underprovision:

1. When the customers over provision, they order more servers than they need, ending up with unused resources.
2. When they under provision, they order too few servers, and fail to deliver on their service level agreements (SLAs).

In both cases the trade off is inefficiency and financial loss. AWS helps customers avoid inefficiencies and financial losses by enabling them to launch the infrastructure they need, when they need it.

AWS Pricing Models

Customers can optimize expenditure by matching the usage model to the requirements of workloads by maturity and behavior.

* On-Demand
* Reserved
* Spot

Maturity = Enough data? Does the customer have enough data to determine a usage baseline so they can use a reserved instance
Behavior = Data use to spiky? Is data usage too spiky for reserved instances. Will spot instances work better?

Typically customers start with on-demand instances to gauge their need and then switch to reserved instances (RIs) or spot instances once they know their demand base line. 
* Reserved instances can decrease cost by up to 75% versus on demand
* Spot Instances are AWS access capacity sold for a deep discount, reducing costs even further 

Price Reductions

Higher efficiency and lower price. Every time AWS reduce their prices, all AWS customers experience the savings immediately. Customers never need to call AWS, contact an account manager, renegotiate a contract or ask for the price reduction.

One exception to price reductions is reserved instances (RIs). RIs are already heavily discounted, with prices accounting for forecasted future discounts.

AWS Flywheel

Flywheel cycle:
* Reduced prices -> More customers -> More AWS usage -> More infrastructure -> Economies of scale -> Lower infrastructure -> Reduce prices …

Migration Challenges and Costs for Customers

* Migration-related costs
* Shifting to an operational expenditure (opEx) model
* Lack of cloud readiness
* Entrenched IT organization

Sunk infrastructure costs: Customer’s hardware is fully depreciated, and the company is not close to a hardware refresh.
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

Entrenched IT department can be a challenge on a migration. Where the IT of the organization feels threatened by perceived loss of control or potential staff reductions. Sometimes finding one or two key players on the company who understand the value of cloud adoption, can help move a migration forward.

Stakeholders

Cost savings engagement may require multiple discussions with different messages for different audiences:

* Application developer (DevOps): Focus mostly on technical specs and features that will simplify their lives, in most cases cost is not a major problem for them.
* IT support team: Changes they’ll have to make to support the new cloud environment, might also focus on the costs of the change.
* Procurement team: Focus on pricing and payment models, need help to understand and adapt to consuming IT as a service using the pay-as-you-go model.
* CFO/CIO/Investors: Focus on the big picture, bottom line, and growing the business and revenue.

Each audience will have unique perspectives on cost savings.

CapEx and OpEx defined

CapEx is defined as business expenses incurred in order to create long-term benefits in the future, such as purchasing fixed assets like a building or equipment. Some examples of IT items that fall under this category would be whole systems and servers, printers and scanners, or air conditioners and generators. You buy these items once and they benefit your business for many, many years. Maintenance of such items is also considered CapEx, as it extends their lifetime and usefulness.

OpEx is your operating costs, the expenses to run day-to-day business, like services and consumable items that get used up and are paid for according to use. This includes printer cartridges and paper, electricity, and even yearly services like website hosting or domain registrations. These things are necessary for your business’s success but are not considered major long-term investments like CapEx items (AWS changes this definition, since AWS Cloud can be seen to customers as a long term investment).

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
* Use realistic on-premises ratios (VM density, servers, racks)
* Explore on-premises CPU and MEM usage
* Apply cost benefits of automation (automatic scaling, APIs, AWS Trusted Advisor, Cost Optimization)

Does not work:
* Forget power/cooling (compute, storage, network)
* Forget administration costs (procurement, design, build, operations, network, security)
* Forget rent/real estate (building depreciation, taxes, shared services staff)
* Forget software and hardware maintenance costs
* Forget the cost of redundancy

Always address overhead costs.

Engagement Process

A typical engagement process takes from one to two months (aprox.) to complete.

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
    * Automated data discovery or flat file Ingest
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

## Staff Productivity

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
* Security benefits: Penetration testing, vulnerability scanning, and security audits are greatly improved

End of Staff Productivity
———————————————————————————————————————————————

## Operational Resilience

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

Helps the customer focus primarily on their business.

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

## Business Agility

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

## Cloud Financial Management

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

## Migration Portfolio Assessment (MPA)
### MPA is a web application that automates the portfolio analyses process.

Help customers collect and analyze data. They can use this data to validate their business cases and create migration plans. Customers can also use this data to estimate the level of effort and cost associated with migration. As well as estimate the annual run rates for compute and storage resources on AWS. 

The MPA tool can be used by:
* Consultants
* Sales teams
* Migration success managers (MSMs)
* Migration leads

MPA can help in a variety of ways:
* Can be used on discovery
* Evaluating total cost of ownership or cost savings
* Creating comparisons between on-premises and AWS
* Estimating migration project costs
* Right-sizing recommendations for a lift-and-shift migration
* Application grouping, prioritization and wave planning

MPA key features:
* Guided data import
* Amazon EC2 and Amazon EBS recommendations
* On-premises cost estimation and comparison
* Migration pattern recommendation
* Migration project cost estimation
* What-if analysis and comparison
* On-premises data visualization
* Application grouping, prioritization and migration planning

MPA data import:
* Allows to import CSV files that contain information about the application
    * Other common sources of MPA inputs:
        * Configuration Management Database (CMDB) extract
        * Automated discovery
        * Manually gathered data

Data ingestion process:
1. Identify the data you want to import
2. Map the required data fields
3. Map the supplemental data fields
4. Check for duplicate records
5. Import the data
6. Check and resolve data issues
7. Run the analysis

MPA target recommendation:
* Provision what you need
* Turn off equipment when you don’t need it 
* Get the lowest cost option automatically selected by MPA
* Delivers EC2 and EBS recommendations

MPA cost comparison:
* Shows cost comparisons between AWS and on-premisses based on data imports
* There are many scenarios to compare costs changing MPA’s variables 

MPA is available to all advanced and premier tier APN partners.

End of MPA
———————————————————————————————————————————————
 
