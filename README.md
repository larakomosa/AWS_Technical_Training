# AWS_Technical_Training

#### Goal: To be able to articulate the value of key AWS service and features, including:
- Cloud computing overviews
- AWS core technologies
- Breadth and Depth of AWS Services and Offerings
	
#### What is Cloud: 
- The cloud provides access to the same or similar resources through internet, as hosted by a cloud services platform.  The term itself comes from a time when internet resources or connectivity was often represented by a cloud in diagrams that illustrated connectivity and data flow.

#### What is Cloud Computing: 
- Cloud computing is on-demand delivery of compute power, database, storage, applications and other IT resources via the Internet with pay as you go pricing.
	
#### Advantages to Cloud Computing:
- Trade capital expense for variable expense
- Benefit from massive economies of scale
- Stop guessing capacity
- Increase speed and agility
- Stop spending money running and maintaining data centers
- Go Global in minutes 
	
#### AWS Intro
- Broad portfolio of global cloud-based products including compute, storage, databases, analytics, networking, mobile developer tools, management tools, ITO, security and enterprise applications that is on demand, available as you go pricing.
- This allows business to access the building blocks they need to respond quickly to changing business requirements.
- Cloud offered on-demand delivery of IT, with pay as you go pricing, instead of costly up from investments.  On top of that, AWS offers a huge range of features and services to help customers solve business challenges and achieve their goals.
	
#### Infrastructure
- Each region is designed to be completely isolated from other regions.  
- Within each region is a separate geographic area know as AZ (availability zones)- Each AZ is isolated from each other AZ's within a region
- High-Speed, low latency connection between AZs within a region.
- POP consist of Edge locations and Regional Edge Cache servers.  The locations used by Amazon CloudFront to securely deliver data, videos, application and APIs to customers globally.
	
# AWS Core Technologies
- Compute
- Storage
- Database
- Security
- Management
- Networking

## Compute Services
- Develop, deploy, run and scale workloads in the AWS Cloud
- Amazon EC2 - Resize Compute Capacity
- Amazon ECS Auto Scaling - Increase or Decrease instances
- Elastic Load Balancing- Distribute incoming traffic
- AWS Lambda - Run code in response to events
- Amazon Elastic Containers Services - Run applications on a managed Cluster
	
#### Benefits of EC2
- Elasticity
- Control
- Flexibility
- Integrated
- Reliable
- Secure
- Inexpensive 
- Easy 
	
#### EC2 Choices: Instance Types:
- Each Category has different families with fundamental differences within the category.  Within each famimly are different generations which are slight variations. 
- General Purpose: Provide balance between memory and networking resources
- Compute Optimized: Ideal for compute bound applications that benefit from high performance processors.
- Memory Optimized: Deliver fast performances for workloads that process large data sets in memory.
- Accelerated Computing: Use hardware accelerators to perform functions such as floating point number calculations, graphics processing or data pattern matching.
- Storage Optimized: Designed for workloads that require high, sequential read and write access to large data sets on local storage.

#### Scaling on AWS
- Launch new instances in advance of peak periods
- Use monitoring to programmatically scale out 
- Automatically scale in
- Pay for the resources needed, when needed.

#### Amazon EC2 Auto Scaling
- Monitor the health of running instances
- Replace impaired instances automatically
- Balance capacity across availability zones
- Dynamic and predictive scaling.

#### Elastic Load Bouncing
- Increases availability and fault tolerance	
- Configure health checks
- Offload encryption and decryption
- Types:
	- Application Load Balancer (app layer)
	- Network Load Balancer (network layer)
	- Class Load Balancer (classic instances)

#### Summary
- Building Blocks on AWS
- Come in huge variety of hardware capabilities to meet the demands of any workload.
- AMIS can be applied to customize the software installation when launched.
- Can configure autoscaling and load balancing so application is always running the proper amount of instances
	
## Storage:
- A reliable, scalable and secure place for Data

### Services
- Amazon Elastic Block Store - Persistent level storage
- Amazon S3 - Durable, scalable object storage
- Amazon S3 Glacier - Data archiving and back up 
- AWS Storage Gateway- Seamless and secure Integration
- Amazon Elastic File System - File storage for Amazon EC2 instance

#### Amazon Elastic Block Storage: (Network-attached block storage)
- Persist independently from instance
- Used like a phyisical hard drive
- Automatically replicated
- Attached to any instance in the same AZ
- One EBS volumne to one EC2 instance
- One instance to many EBS volumes
- EBS volumes can retain data after EC2 instance termination
- Allow Point-in-Time Snapshots to S3 GB increments

#### Amazon S3
- Highly scalable object storage
- Common s3 Use Cases:
	- Backup and storage 
	- Application hosting
	- Media hosting
	- Software Delivery
- Storage Classes
	- Standard 
	- Standard - Infrequent Access (lower rate and per gigabyte retreival)
	- One Zone IA - Stores data in AZ.  Cost 20% less and do not need availability.  Good for back up copies of data
	- Amazon Glazer - Low Cost Data Archiving
	- S3 Intelligent Tiering (moves between 2 tiers)


## Databases -purpose built for specific application use cases 
- Replace daily management tasks with value-added processes
- AWS database services handle time-consuming database management tasks, such as backups, patch management, and replication, allowing customers to pursue higher-value application development.
- Offload time-consuming management tasks
- Amazon RDS - choice of 6 popular databases (PostgreSQL, mySQL)
- Amazon DynamoDB is a no SQL database with single digit millisecond performance
- Amazon ElasticCache is a caching service that makes it easy to deploy, operate and scale in-memory cache in cloud.

### EC2 vs AWS Databases Services
#### AWS
- Easy to Setup, manage, maintain
- Reduce undifferentiated heavy listing
- Push Button High Availability
- Automatic backup/recovery
- Scale up or down based upon pattern

#### EC2
- More control/flexibility
- Operating system access
- Need features of specific application

## Networking
- Isolate cloud infrastructure and scale request-handling capacity
	
### Options
- Amazon VPC 
	- Build a virtual network in the cloud
- Security Groups
	- Control Access to instances
- Network Access Control List (NACL)
	- Contol access to subnets
- Amazon Route 53
	- Route end users to internet applications 

#### Amazon Virtual Private Cloud
- Networking layer for Amazon EC2
- A virtual network dedicated to a customer's AWS account
- Subnet
	- A range of IP addresses in VPC

#### Securing a VPC
- Network Access Control Lists
- Control traffic at the subnet level
- Security Groups
	- Control traffic at the instance level
- Flow Logs
- Host-based firewalls 
	- Operating system firewalls
	
#### Summary
- Build a VPC (Virtual Network in Clould
- Configure Public and Private Subnets
- Secure network using ACLs
- Create Another layer of security at the instance level using security groups.

## Security	
- Offer security, identity, and compliance services

### Options
- AWS Identity and Access Management, or IAM,	
- AWS Shared Responsibility Model
- AWS Cloud compliance.

#### Amazon IAM
- Securely manage access to AWS services an resources 
	- Fine-grained access control to AWS resources
	- Multi-factor Authentication
	- The ability to analyze access
	- Integration with Corporate directories

#### Cloud Security
- Inherit benefits from AWS data cnter and network architechure
- Similar to on premise data centers, without maintaining facilites and hardware
- Can be easily automated
- Inherit all the best practices of AWS
	
#### AWS Shared Responsibility Model
- AWS is responsibility of the security of the cloud
- AWS is also responsible for the security configurations of it's products that are considered to be managed services, such as Amazon RDS
- Customers are responsible for Security in the cloud

#### AWS Cloud Compliance
- Sharing Information
	- Obtaining industry certifications and independent third-party attestations
	- Publishing information about the AWS security and control practices in whitepapers and website content
	- Providing certificates, reports, and other documents directly to AWS customers under NDA
	- Assurance Programs
		○ Certifications and attestations
		○ Laws, regulations and privacy
		○ Alignments and frameworks

#### Summary
- AWS Shared Responsibility Model
	- AWS handles the infrastructure piece and their manage services, while customers are responsible for securing the data and resources they build in the cloud
	- AWS gives customers the tools they need to meet that end, but its up to them to implement them.
	
##  AWS Management Interfaces
- AWS Management Console
	- Graphical interface to facilitates cloud management
- Command Line Interfaces (AWS CLI)
	- Access to services via discrete command
- Software Development Kits
	- Access services in your code 
	
## AWS Services to Solutions
- Adapt AWS Solutions to Meet Customer Challenges
- Adapt AWS architechural and cost optimazation best practices

#### Content
- Describing the customer challenge
- Outlining the initial AWS Solution
- Diving Deeper
	- Migration approaches
	- Architectural best practices
	- Well architected framework
	- Use Cases

#### AWS Solutions
- Machine Learning
- Analytics and Data Lakes
- Internet of Things
- Serverless Computing
- Containers
- Enterprise Applications
- Storage
- Windows Workloads 

#### Addressing Customer Challenges
Ex: AnyCompany Apparel
- Acquiring ExampleCorp
- eCommerce Site is slow
- Created by Contractor
- Not enough resources
- Not PCI compliant
- Relies upon contractor
- Prefer less hands on

#### Migration Strategies
- Rehost
- Replatform
- Refactor
- Retire
- Retain
- Repurchase

#### Rehost
- Recreating the on-premises network, only hosted on AWS
- Automating with tools such as AWS VM Import/Export
- Easier to optimize and re-architect applications after the migration

#### Replatform:  life, tinker, and shift
- Retaining the core architecture
- Making targeted AWS cloud optimizations
- Examples
	- Migrating databases to Amazon RDS
	- Migrating applications to Amazon Elastic Beanstalk

#### Refactoring
- Re-imagining how the application is architected and developed 
- Using could-native features

#### Retire
- Shutting off non-useful applications
- Reducing spend, management, and security

#### Retain/Revisit
- Keeping certain applications on-premises

#### Repurchase
- Moving workflows to software as a service (SaaS)

## Best Practices 
- Design for failure and nothing fails
- Avoid single points of failure
- Multiple instances
- Multiple availability Zones
- Separate single server into multiple tiered application
	- For Amazon RDS, use Multi-AZ feature
- Build Security in every layer
	- Encrpyt Data at rest and in transit
	- Enforce principle of least privilege in IAM
	- Implement both Security Groups and Network Access Control Lists
	- Consider advanced security features and services 
- Leverage Different Storage Options
	- Move static web assets to Amazon S3
	- Use Amazon CloudFront to serve globally
	- Store session state in DynamoDB
	- Use Elasticache between hosts and databases
- Implement Elasticity
	- Implemnt Auto Scaling polices
	- Architect resiliency to reboot and relaunch
	- Leverage managed serves like Amazon s3 and Amazon DynamoDB
- Think Parallel
	- Scale horizontally, not vertically
	- Decouple compute from session/state
	- Use Elastic Load Balancing
	- Right-Size your infrastructure
- Loose Coupling sets you free
	- Instead of a single ordered workflow, use multiple queues
	- Use Amazon Simple Queue Service and Simple Notification Service (SQS and SNS)
	- Leverage existing services 
- Don’t fear constraints
	- Rethink traditional constraints
	- Need more RAM
	- Better IOPS for databases
	- Response to failure?

## Well-Architected Framework
- A framework for ensuring infrastructures are:
	- Secure
	- High-Performing
	- Resilient
	- Efficient
- Practices developed through revieing customers architectures on AWWS
- Systematic approach for evaluating and implementing architectures
- Well-Architected took in the console

#### Five Pillars of Architecture
- Operational excellence
- Security
- Reliability
- Performance Efficiency
- Cost Optimization
	
#### Cost Optimization (pay for what you need)
- Right-sizing instances
- Increase elasticity
- Choosing the right pricing model
- Optimizing Storage


## AWS Solutions
- Definition of an AWS Solution - Vetted, technical reference implementations designed to help customers solve common problems and build faster - http://aws.amazon/solutions
- AWS Solution Space provides customers who need help deploying an AWS solution by highlighting AWS competency partner solutions- http://aws.amazon.com/solutionspace.



