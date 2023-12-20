## Summaries

### What is Cloud Computing

The on-demand delivery of IT resources over the internet with pay-as-you-go pricing.

This means that you can make requests for IT resources like compute, networking, storage, analytics, or other types of resources, and then they're made available for you on demand. You don't pay for the resource upfront. Instead, you just provision and pay at the end of the month.

### Cloud Computing Models

There are 3 common types of cloud computing model:

1. Infrastructure as a service (IaaS).
2. Platform as a service (PaaS).
3. Software as a service (SaaS).

#### Infrastructure as a Service (IaaS)

Infrastructure as a Service (IaaS) contains the basic building blocks for cloud IT and typically provide access to networking features, computers (virtual or on dedicated hardware), and data storage space.

IaaS provides you with the highest level of flexibility and management control over your IT resources and is very similar to the existing IT resources that many IT departments and developers are familiar with today.

#### Platform as a Service (PaaS)

Platform as a Service (PaaS) removes the need for your organization to manage the underlying infrastructure (usually hardware and operating systems) and allows you to focus on the deployment and management of your applications.

This helps you be more efficient as you don't need to worry about resource procurement, capacity planning, software maintenance, patching, or any of the other undifferentiated heavy lifting involved in running your application.

#### Software as a Service (SaaS)

Software as a Service (SaaS) provides you with a completed product that is run and managed by the service provider. In most cases, people referring to Software as a Service are referring to end-user applications.

With a SaaS offering you do not have to think about how the service is maintained or how the underlying infrastructure is managed; you only need to think about how you will use that piece of software.

A common example of a SaaS application is web-based email which you can use to send and receive email without having to manage feature additions to the email product or maintain the servers and operating systems that the email program is running on.

SaaS provides high availability, fault tolerance, scalability and elasticity.

### Advantages of Cloud Computing

Operating in the AWS Cloud offers many benefits over computing in on-premises or hybrid environments.

#### Six Advantages of Cloud Computing

- Trade upfront expense for variable expense.
- Benefit from massive economies of scale.
- Stop guessing capacity.
- Increase speed and agility.
- Stop spending money running and maintaining data centers.
- Go global in minutes.

1. #### Trade Upfront Expense for Variable Expense

   Upfront expenses include data centers, physical servers, and other resources that you would need to invest in before using computing resources.

   Instead of investing heavily in data centers and servers before you know how you're going to use them, you can pay only when you consume computing resources.

2. #### Benefit from Massive Economies of Scale

   By using cloud computing, you can achieve a lower variable cost than you can get on your own. Because usage from hundreds of thousands of customers aggregates in the cloud, providers such as AWS can achieve higher economies of scale. Economies of scale translate into lower pay-as-you-go prices.

3. #### Stop Guessing Capacity

   With cloud computing, you don't have to predict how much infrastructure capacity you will need before deploying an application.

   For example, you can launch Amazon Elastic Compute Cloud (Amazon EC2) instances when needed and pay only for the compute time you use. Instead of paying for resources that are unused or dealing with limited capacity, you can access only the capacity that you need, and scale in or out in response to demand.

4. #### Increase Speed and Agility

   The flexibility of cloud computing makes it easier for you to develop and deploy applications. This flexibility also provides your development teams with more time to experiment and innovate.

5. #### Stop Spending Money Running and Maintaining Data Centers

   Cloud computing in data centers often requires you to spend more money and time managing infrastructure and servers. A benefit of cloud computing is the ability to focus less on these tasks and more on your applications and customers.

6. #### Go Global in Minutes

   The AWS Cloud global footprint enables you to quickly deploy applications to customers around the world, while providing them with low latency.

### Types of Cloud Deployment

#### Three Common Types of Cloud Deployment

1. _Public Cloud_ – e.g. AWS, Microsoft Azure, Google Cloud Platform (GCP).
2. _Hybrid Cloud_ – a mixture of public and private clouds.
3. _Private Cloud (on-premises)_ – a cloud managed in your own data center, e.g. Hyper-V, OpenStack, VMware.

#### Public Cloud

A cloud-based application is fully deployed in the cloud and all parts of the application run in the cloud. Applications in the cloud have either been created in the cloud or have been migrated from an existing infrastructure to take advantage of the benefits of cloud computing.

Cloud-based applications can be built on low-level infrastructure pieces or can use higher level services that provide abstraction from the management, architecting, and scaling requirements of core infrastructure.

#### Hybrid

A hybrid deployment is a way to connect infrastructure and applications between cloud-based resources and existing resources that are not located in the cloud.

The most common method of hybrid deployment is between the cloud and existing on-premises infrastructure to extend, and grow, an organization's infrastructure into the cloud while connecting cloud resources to the internal system.

#### On-Premises

The deployment of resources on-premises, using virtualization and resource management tools, is sometimes called the "private cloud."

On-premises deployment doesn't provide many of the benefits of cloud computing but is sometimes sought for its ability to provide dedicated resources.

In most cases this deployment model is the same as legacy IT infrastructure while using application management and virtualization technologies to try and increase resource utilization.

### Compute in the Cloud

EC2, you can dynamically spin up and spin down virtual servers called EC2 instances. When you launch an EC2 instance, you choose the instance family. The instance family determines the hardware the instance runs on.

And you can have instances that are built for your specific purpose. The categories are general purpose, compute optimized, memory optimized, accelerated computing, and storage optimized.

You can scale your EC2 instances either vertically by resizing the instance, or horizontally by launching new instances and adding them to the pool. You can set up automated horizontal scaling, using Amazon EC2 Auto Scaling.

Once you've scaled your EC2 instances out horizontally, you need something to distribute the incoming traffic across those instances. This is where the Elastic Load Balancer comes into play.

EC2 instances have different pricing models. There is On-Demand, which is the most flexible and has no contract, spot pricing, which allows you to utilize unused capacity at a discounted rate, Savings Plans or Reserved Instances, which allow you to enter into a contract with AWS to get a discounted rate when you commit to a certain level of usage, and Savings Plans which apply to AWS Lambda, and AWS Fargate, as well as EC2 instances.

We also covered messaging services. There is Amazon Simple Queue Service or SQS. This service allows you to decouple system components. Messages remain in the queue until they are either consumed or deleted. Amazon Simple Notification Service or SNS, is used for sending messages like emails, text messages, push notifications, or even HTTP requests. Once a message is published, it is sent to all of these subscribers.

You also learned that AWS has different types of compute services beyond just virtual servers like EC2. There are container services like Amazon Elastic Container Service, or ECS. And there's Amazon Elastic Kubernetes Service, or EKS. Both of which are container orchestration tools. You can use these tools with EC2 instances, but if you don't want to manage that, you don't need to.

You can use AWS Fargate, which allows you to run your containers on top of a serverless compute platform. Then there is AWS Lambda, which allows you to just upload your code, and configure it to run based on triggers. And you only get charged for when the code is actually running. No containers, no virtual machines. Just code and configuration.

### AWS Global Infrastructure

Logical clusters of data centers make up Availability Zones, Availability Zones in turn make up Regions, and those are spread globally. You then choose what Regions and Availability Zones you want to operate out of and as a best practice, you should always deploy infrastructure across at least two Availability Zones. And some AWS services like Elastic Load Balancing, Amazon SQS, and Amazon SNS already do this for you.

Edge locations and how you can deploy content there to speed up delivery to your customers. We even touched upon edge devices like AWS Outposts which allow you to run AWS infrastructure right in your own data center.

how to provision AWS resources through various options, such as the AWS Management Console, the SDK, CLI, AWS Elastic Beanstalk, and AWS CloudFormation, where you learned how you can set up your infrastructure as code.

### Networking:

#### Network Hardening

AWS has a wide range of tools that cover every layer of security: network hardening, application security, user identity, authentication and authorization, distributed denial-of-service or DDoS prevention, data integrity, encryption.

The public subnets have access to the internet gateway; the private subnets do not.

But subnets can also control traffic permissions. Packets are messages from the internet, and every packet that crosses the subnet boundaries gets checked against something called a network access control list or network ACL. This check is to see if the packet has permissions to either leave or enter the subnet based on who it was sent from and how it's trying to communicate.

_network ACLs_

A network ACL is a virtual firewall that controls inbound and outbound traffic at the subnet level. Network ACLs perform **stateless** packet filtering. They remember nothing and check packets that cross the subnet border each way: inbound and outbound. When a packet response for that request comes back to the subnet, the network ACL does not remember your previous request. The network ACL checks the packet response against its list of rules to determine whether to allow or deny. After a packet has entered a subnet, it must have its permissions evaluated for resources within the subnet, such as Amazon EC2 instances.

You can think of **network ACLs** as passport control officers. If you're on the approved list, you get through. If you're not on the list, or if you're explicitly on the do-not-enter list, then you get blocked. Network ACLs check traffic going into and leaving a subnet, just like passport control. The list gets checked on your way into a country and on the way out. And just because you were let in doesn't necessarily mean they're gonna let you out. Approved traffic can be sent on its way, and potentially harmful traffic, like attempts to gain control of a system through administrative requests, they get blocked before they ever touch the target. You can't hack what you can't touch.

Now, this sounds like great security, but it doesn't answer all of the network control issues. Because a network ACL only gets to evaluate a packet if it crosses a subnet boundary, in or out. It doesn't evaluate if a packet can reach a specific EC2 instance or not. Sometimes, you'll have multiple EC2 instances in the same subnet, but they might have different rules around who can send them messages, what port those messages are allowed to be sent to. So, you need instance level network security as well.

By default, your account's default network ACL allows all inbound and outbound traffic, but you can modify it by adding your own rules. For custom network ACLs, all inbound and outbound traffic is denied until you add rules to specify which traffic should be allowed. Additionally, all network ACLs have an explicit deny rule. This rule ensures that if a packet doesn't match any of the other rules on the list, the packet is denied.

_security groups_

A security group is a virtual firewall that controls inbound and outbound traffic for an Amazon EC2 instance. By default, a security group denies all inbound traffic and allows all outbound traffic. You can add custom rules to configure which traffic should be allowed; any other traffic would then be denied. Security groups perform **stateful** packet filtering. They remember previous decisions made for incoming packets. When a packet response for that request returns to the instance, the security group remembers your previous request. The security group allows the response to proceed, regardless of inbound security group rules.

To solve instance level access questions, we introduce **security groups**. Every EC2 instance, when it's launched, automatically comes with a security group. And by default, the security group does not allow any traffic into the instance at all. All ports are blocked; all IP addresses sending packets are blocked. That's very secure, but perhaps not very useful. If you want an instance to actually accept traffic from the outside, like say, a message from a front end instance or a message from the Internet. So obviously, you can modify the security group to accept a specific type of traffic. In the case of a website, you want web-based traffic or HTTPS to be accepted but not other types of traffic, say an operating system or administration requests.

#### Security Group and a Network ACL Key Differences:

The key difference between a security group and a network ACL is the security group is stateful, meaning, as we talked about, it has some kind of a memory when it comes to who to allow in or out, and the network ACL is stateless, which remembers nothing and checks every single packet that crosses its border regardless of any circumstances. With both network ACLs and security groups, you can configure custom rules for the traffic in your VPC. As you continue to learn more about AWS security and networking, make sure to understand the differences between network ACLs and security groups.

#### Subnets

A subnet is a section of a VPC in which you can group resources based on security or operational needs. Subnets can be public or private.

_Public subnets_ contain resources that need to be accessible by the public, such as an online store's website.

_Private subnets_ contain resources that should be accessible only through your private network, such as a database that contains customers' personal information and order histories. In a VPC, subnets can communicate with each other. For example, you might have an application that involves Amazon EC2 instances in a public subnet communicating with databases that are located in a private subnet.

#### Domain Name System (DNS)

Suppose that AnyCompany has a website hosted in the AWS Cloud. Customers enter the web address into their browser, and they are able to access the website. This happens because of _Domain Name System (DNS_**) resolution. DNS resolution involves a customer DNS resolver communicating with a company DNS server.

You can think of DNS as being the phone book of the internet. DNS resolution is the process of translating a domain name to an IP address.

1. When you enter the domain name into your browser, this request is sent to a customer DNS resolver.
2. The customer DNS resolver asks the company DNS server for the IP address that corresponds to AnyCompany's website.
3. The company DNS server responds by providing the IP address for AnyCompany's website, 192.0.2.0.

### Storage and Databases:

### Storage

The first one we learned about is Elastic Block Store volumes, and you attach those to EC2 instances so you have local storage that is not ephemeral.

You learned about how S3 and how you can store objects in AWS with the click of a button or call of an API.

#### Amazon S3 and Amazon EBS Key Differences:

#### S3

In the regional object storage corner, weighing in at unlimited storage, with individual objects at 5,000 gigabytes in size, they specialize in write once/read many, they are 99 .999 999 999% durable, they are Amazon Simple Storage Service!

#### EBS

In the block storage corner, weighing in at sizes up to 16 tebibytes each, with a unique ability to survive the termination of their Amazon EC2 instances, they are solid state, they are spinning platters, they are Amazon Elastic Block Storage!

#### Use Cases

Let's say you're running a photo analysis website where users upload a photo of themselves, and your application finds the animals that look just like them. You have potentially millions of animal pictures that all need to be indexed and possibly viewed by thousands of people at once. This is the perfect use case for S3. S3 is already web enabled. Every object already has a URL that you can control access rights to who can see or manage the image. It's regionally distributed, which means that it has 11 nines of durability, so no need to worry about backup strategies. S3 is your backup strategy. Plus the cost savings is substantial overrunning the same storage load on EBS. With the additional advantage of being serverless, no Amazon EC2 instances are needed. **Sounds like S3 is the judge's winner here for this round.**

You have an 80-gigabyte video file that you're making edit corrections on. To know the best storage class here, we need to understand the difference between object storage and block storage. Object storage treats any file as a complete, discreet object. Now this is great for documents, and images, and video files that get uploaded and consumed as entire objects, but every time there's a change to the object, you must re-upload the entire file. There are no delta updates. Block storage breaks those files down to small component parts or blocks. This means, for that 80-gigabyte file, when you make an edit to one scene in the film and save that change, the engine only updates the blocks where those bits live. If you're making a bunch of micro edits, using EBS, elastic block storage, is the perfect use case. If you were using S3, every time you saved the changes, the system would have to upload all 80 gigabytes, the whole thing, every time. **EBS clearly wins round two.**

This means, if you are using complete objects or only occasional changes, S3 is victorious. If you are doing complex read, write, change functions, then, absolutely, EBS is your knockout winner. Your winner depends on your individual workload. Each service is the right service for specific needs. Once you understand what you need, you will know which service is your champion!

#### Amazon EBS and Amazon EFS Key Differences:

Amazon EBS volumes attach to EC2 instances and are an Availability Zone-level resource. In order to attach EC2 to EBS, you need to be in the same AZ. You can save files on it. You can also run a database on top of it. Or store applications on it. It's a hard drive. If you provision a two terabyte EBS volume and fill it up, it doesn't automatically scale to give you more storage. So that's EBS.

#### EBS Vs EFS

Amazon EFS can have multiple instances reading and writing from it at the same time.

But it isn't just a blank hard drive that you can write to. It is a true file system for Linux. It is also a regional resource. Meaning any EC2 instance in the Region can write to the EFS file system. As you write more data to EFS, it automatically scales. No need to provision any more volumes.

#### Amazon EBS

An Amazon EBS volume stores data in a  **single**  Availability Zone.

To attach an Amazon EC2 instance to an EBS volume, both the Amazon EC2 instance and the EBS volume must reside within the same Availability Zone.

#### Amazon EFS

Amazon EFS is a regional service. It stores data in and across  **multiple**  Availability Zones.

The duplicate storage enables you to access data concurrently from all the Availability Zones in the Region where a file system is located. Additionally, on-premises servers can access Amazon EFS using AWS Direct Connect.

### Databases

The various relational database options available on AWS. Or for the workloads that just need a key-value pair, we have the non-relational offering called DynamoDB.

Next up was EFS for file storage use cases.

We then have Amazon Redshift for all our data warehouse needs.

And to aid in migration of existing databases, we have DMS or Database Migration Service

#### Relational databases

In a _relational database_, data is stored in a way that relates it to other pieces of data.

An example of a relational database might be the coffee shop's inventory management system. Each record in the database would include data for a single item, such as product name, size, price, and so on.

Relational databases use structured query language (SQL) to store and query data. This approach allows data to be stored in an easily understandable, consistent, and scalable way. For example, the coffee shop owners can write a SQL query to identify all the customers whose most frequently purchased drink is a medium latte.

_Lift-and-Shift_ and migrate your database to run on Amazon EC2. This means you have control over the same variables you do, in your on-premises environment, such as OS, memory, CPU, storage capacity, and so forth. It's a quick entry to the cloud, and you can migrate them using standard practices or using something like Database Migration Service.

#### Relational databases Vs Nonrelational databases

#### Nonrelational databases

In a _nonrelational database_, you create tables. A table is a place where you can store and query data.

Nonrelational databases are sometimes referred to as "NoSQL databases" because they use structures other than rows and columns to organize data. One type of structural approach for nonrelational databases is key-value pairs. With key-value pairs, data is organized into items (keys), and items have attributes (values). You can think of attributes as being different features of your data.

In a key-value database, you can add or remove attributes from items in the table at any time. Additionally, not every item in the table has to have the same attributes.

#### Amazon RDS and Amazon DynamoDB Key Differences:

#### Amazon RDS

In the relational corner, engineered to remove undifferentiated heavy lifting from your database administrators with automatic high availability and recovery provided. You control the data, you control the schema, you control the network. You are running Amazon RDS.

#### Amazon RDS Vs Amazon DynamoDB

#### Amazon DynamoDB

The NoSQL corner, using a key value pair that requires no advanced schema, able to operate as a global database at the touch of a button. It has massive throughput. It has petabyte scale potential. It has granular API access. It is Amazon DynamoDB.

#### Use Cases

**Round One** Relational databases have been around since the moment businesses started using computers. Being able to build complex analysis of data spread across multiple tables, is the strength of any relational system. In this round, you have a sales supply chain management system that you have to analyze for weak spots. Using RDS is the clear winner here because it's built for business analytics, because you need complex relational joins. Round one easily goes to RDS.

**Round two**, the use case, pretty much anything else. Now that sounds weird, but despite what your standalone legacy database vendor would have you believe, most of what people use expensive relational databases for, has nothing to do with complex relationships. In fact, a lot of what people put into these databases ends up just being look-up tables.

Imagine you have an employee contact list: names, phone numbers, emails, employee IDs. Well, this is all single table territory. I could use a relational database for this, but the things that make relational databases great, all of that complex functionality, creates overhead and lag and expense if you're not actually using it. This is where non-relational databases, Dynamo DB, delivers the knockout punch. By eliminating all the overhead, DynamoDB allows you to build powerful, incredibly fast databases where you don't need complex joint functionality. DynamoDB comes out the undisputed champion.

### Security

### Shared Responsibility Model:

- AWS is responsible for the security **of** the cloud.
- The Customer is responsible for the security **in** the cloud.

#### AWS: Security **of** the cloud

AWS is responsible for security of the cloud.

AWS operates, manages, and controls the components at all layers of infrastructure. This includes areas such as the host operating system, the virtualization layer, and even the physical security of the data centers from which services operate.

AWS is responsible for protecting the global infrastructure that runs all of the services offered in the AWS Cloud. This infrastructure includes AWS Regions, Availability Zones, and edge locations.

AWS manages the security of the cloud, specifically the physical infrastructure that hosts your resources, which include:

- Physical security of data centers
- Hardware and software infrastructure
- Network infrastructure
- Virtualization infrastructure

Although you cannot visit AWS data centers to see this protection firsthand, AWS provides several reports from third-party auditors. These auditors have verified its compliance with a variety of computer security standards and regulations.

#### Customers: Security **in** the cloud

Customers are responsible for the security of everything that they create and put in the AWS Cloud.

When using AWS services, you, the customer, maintain complete control over your content. You are responsible for managing security requirements for your content, including which content you choose to store on AWS, which AWS services you use, and who has access to that content. You also control how access rights are granted, managed, and revoked.

The security steps that you take will depend on factors such as the services that you use, the complexity of your systems, and your company's specific operational and security needs. Steps include selecting, configuring, and patching the operating systems that will run on Amazon EC2 instances, configuring security groups, and managing user accounts.

#### Amazon Web Services (AWS) Security **of** the cloud

- **Hardware**: Regions, Availability Zones, Edge Locations
- **Software**: Compute, storage, database, networking

#### Customers: Security **in** the cloud

- Client-side data encryption, server-side data encryption, and networking traffic protection
- Operating systems, and network and firewall configuration
- Platform, applications, Identity and Access Management (IAM)
- Customer data

_Encryption_ in AWS, you are the owner of your data, and you are responsible for security. That means you need to pay attention to encryption, in transit and at rest.

### Compliance

AWS has already built out data center infrastructure and networking following industry best practices for security, and as an AWS customer, you inherit all the best practices of AWS policies, architecture, and operational processes.

AWS complies with a long list of assurance programs that you can find online. This means that segments of your compliance have already been completed, and you can focus on meeting compliance within your own architectures that you build on top of AWS. The next thing to know in regards to compliance and AWS, is that the Region you choose to operate out of, might help you meet compliance regulations. If you can only legally store data in the country that the data is from, you can choose a Region that makes sense for you and AWS will not automatically replicate data across Regions.

You also should be very aware of the fact that you own your data in AWS. As shown in the AWS shared responsibility model, you have complete control over the data that you store in AWS. You can employ multiple different encryption mechanisms to keep your data safe, and that varies from service to service. So, if you need specific standards for data storage, you can devise a way to either reach those requirements by building it yourself on top of AWS or using the features that already exist in many services. For a lot of services, enabling data protection is a configuration setting on the resource.

AWS also offers multiple whitepapers and documents that you can download and use for compliance reports. Since you aren't running the data center yourself, you can essentially request that AWS provides you with documentation proving that they are following best practices for security and compliance.

#### AWS Compliance Center

Check out the AWS Compliance Center in order to find compliance information all in one place. It will show you compliance enabling services as well as documentation like the AWS Risk and Security Whitepaper, which you should read to ensure that you understand security and compliance with AWS.

we follow a shared responsibility. The underlying platform is secure and AWS can provide documentation on what types of compliance requirements they meet, through services like AWS Artifact and whitepapers. But, beyond that, what you build on AWS is up to you. You control the architecture of your applications and the solutions you build, and they need to be built with compliance, security, and the shared responsibility model in mind.

_AWS compliance uses third-party auditors_ to prove its adherence to a wide variety of compliance programs. You can use the AWS Compliance Center to find more information on compliance and AWS Artifact to gain access to compliance documents. The compliance requirements you have will vary from application to application and between areas of operation.

#### Denial-of-Service Attacks

A _denial-of-service (DoS) attack_ is a deliberate attempt to make a website or application unavailable to users.

In a _distributed denial-of-service (DDoS)_ attack, multiple sources are used to start an attack that aims to make a website or application unavailable. This can come from a group of attackers, or even a single attacker. The single attacker can use multiple infected computers (also known as "bots") to send excessive traffic to a website or application.

To help minimize the effect of DoS and DDoS attacks on your applications, you can use AWS Shield.

_Distributed denial-of-service attacks_, or DDoS attacks, and how to combat them with AWS using tools like ELB, security groups, AWS Shield, and AWS WAF.

### IAM

With _IAM_, you have users, groups, roles, and policies. Users log in with a username and password and by default they have no permissions. Groups are groupings of users and roles are identities that you can assume to gain access to temporary credentials and permissions for a configurable amount of time. In order to give permissions to an identity, you need to create policies that either explicitly allow or deny a specific action in AWS. _With IAM also comes identity federation_. If you have an existing corporate identity store, you can federate those users to AWS, using role based access, which allows your users to use one login for both your corporate systems as well as AWS. One final point to remember about IAM is that you should make sure that you turn on _multi-factor Authentication_ for users, but especially for your root user which has all the permissions by default and cannot be restricted.

_AWS Organizations_. With AWS, it's likely you'll have multiple accounts. Accounts are commonly used to isolate workloads, environments, teams, or applications. AWS Organizations helps you manage multiple accounts in a hierarchical fashion.

Use the _least privilege principle_ when scoping permissions for users and roles in IAM, encrypt your data at every layer, both in transit and at rest. And make sure you use AWS services to protect your environment.

### Monitoring and Analytics

#### Example: AWS CloudTrail event

Suppose that the coffee shop owner is browsing through the AWS Identity and Access Management (IAM) section of the AWS Management Console. They discover that a new IAM user named Mary was created, but they do not know who, when, or which method created the user.

To answer these questions, the owner navigates to AWS CloudTrail.

In the CloudTrail Event History section, the owner applies a filter to display only the events for the "CreateUser" API action in IAM. The owner locates the event for the API call that created an IAM user for Mary. This event record provides complete details about what occurred:

On January 1, 2020 at 9:00 AM, IAM user John created a new IAM user (Mary) through the AWS Management Console.

_CloudWatch_ can provide near real-time understanding of how your system is behaving, including being alerted to conditions that require your attention. CloudWatch also gives you the ability to look at those metrics over time as you tune your system for maximum performance.

_CloudTrail_ can help you know exactly who did what, when, and from where. It answers all of your AWS auditing questions, except why they did it.

_Trusted Advisor_ that compiles a quick dashboard of over 40 common concerns around cost, performance, security, and resilience in an actionable dashboard. AWS Trusted Advisor is a web service that inspects your AWS environment and provides real-time recommendations in accordance with AWS best practices. The inspection includes security checks, such as Amazon S3 buckets with open access permissions.

### Pricing and Support

### Pricing

#### AWS Free Tier

_The AWS Free Tier_ enables you to begin using certain services without having to worry about incurring costs for the specified period.

Three types of offers are available:

- Always Free
- 12 Months Free
- Trials

_Always Free_ These offers do not expire and are available to all AWS customers. For example, AWS Lambda allows 1 million free requests and up to 3.2 million seconds of compute time per month. Amazon DynamoDB allows 25 GB of free storage per month.

_12 Months Free_ These offers are free for 12 months following your initial sign-up date to AWS. Examples include specific amounts of Amazon S3 Standard Storage, thresholds for monthly hours of Amazon EC2 compute time, and amounts of Amazon CloudFront data transfer out.

_Trials_ Short-term free trial offers start from the date you activate a particular service. The length of each trial might vary by number of days or the amount of usage in the service. For example, Amazon Inspector offers a 90-day free trial. Amazon Lightsail (a service that enables you to run virtual private servers) offers 750 free hours of usage over a 30-day period.

#### _Pay for what you use_

For each service, you pay for exactly the amount of resources that you actually use, without requiring long-term contracts or complex licensing.

#### _Pay less when you reserve._

Some services offer reservation options that provide a significant discount compared to On-Demand Instance pricing.

For example, suppose that your company is using Amazon EC2 instances for a workload that needs to run continuously. You might choose to run this workload on Amazon EC2 Instance Savings Plans, because the plan allows you to save up to 72% over the equivalent On-Demand Instance capacity.

#### Pay less with volume-based discounts when you use more.

Some services offer tiered pricing, so the per-unit cost is incrementally lower with increased usage. For example, the more Amazon S3 storage space you use, the less you pay for it per GB.

#### AWS Pricing Calculator

_The AWS Pricing Calculator_ lets you explore AWS services and create an estimate for the cost of your use cases on AWS. You can organize your AWS estimates by groups that you define. A group can reflect how your company is organized, such as providing estimates by cost center. When you have created an estimate, you can save it and generate a link to share it with others.

Suppose that your company is interested in using Amazon EC2. However, you are not yet sure which AWS Region or instance type would be the most cost-efficient for your use case. In the AWS Pricing Calculator, you can enter details, such as the kind of operating system you need, memory requirements, and input/output (I/O) requirements. By using the AWS Pricing Calculator, you can review an estimated comparison of different EC2 instance types across AWS Regions.

#### Pricing Examples:

For _Pricing AWS Lambda_, you are charged based on the number of requests for your functions and the time that it takes for them to run. AWS Lambda allows 1 million free requests and up to 3.2 million seconds of compute time per month. You can save on AWS Lambda costs by signing up for a Compute Savings Plan. A Compute Savings Plan offers lower compute costs in exchange for committing to a consistent amount of usage over a 1-year or 3-year term. This is an example of paying less when you reserve.

With _Pricing Amazon EC2_, you pay for only the compute time that you use while your instances are running. For some workloads, you can significantly reduce Amazon EC2 costs by using Spot Instances. For example, suppose that you are running a batch processing job that is able to withstand interruptions. Using a Spot Instance would provide you with up to 90% cost savings while still meeting the availability requirements of your workload. You can find additional cost savings for Amazon EC2 by considering Savings Plans and Reserved Instances.

For _Amazon S3 pricing_, consider the following cost components:

**Storage** - You pay for only the storage that you use. You are charged the rate to store objects in your Amazon S3 buckets based on your objects' sizes, storage classes, and how long you have stored each object during the month.

**Requests and data retrievals** - You pay for requests made to your Amazon S3 objects and buckets. For example, suppose that you are storing photo files in Amazon S3 buckets and hosting them on a website. Every time a visitor requests the website that includes these photo files, this counts towards requests you must pay for.

**Data transfer** - There is no cost to transfer data between different Amazon S3 buckets or from Amazon S3 to other services within the same AWS Region. However, you pay for data that you transfer into and out of Amazon S3, with a few exceptions. There is no cost for data transferred into Amazon S3 from the internet or out to Amazon CloudFront. There is also no cost for data transferred out to an Amazon EC2 instance in the same AWS Region as the Amazon S3 bucket.

**Management and replication** - You pay for the storage management features that you have enabled on your account's Amazon S3 buckets. These features include Amazon S3 inventory, analytics, and object tagging.

_AWS Billing & Cost Management dashboard_ to pay your AWS bill, monitor your usage, and analyze and control your costs.

- Compare your current month-to-date balance with the previous month, and get a forecast of the next month based on current usage.
- View month-to-date spend by service.
- View Free Tier usage by service.
- Access Cost Explorer and create budgets.
- Purchase and manage Savings Plans.
- Publish AWS Cost and Usage Reports

### Support Plans

#### AWS Support

AWS offers four different Support plans(opens in a new tab) to help you troubleshoot issues, lower costs, and efficiently use AWS services.

You can choose from the following Support plans to meet your company's needs:

- Basic
- Developer
- Business
- Enterprise On-Ramp
- Enterprise

#### Basic Support

Basic Support is free for all AWS customers. It includes access to whitepapers, documentation, and support communities. With Basic Support, you can also contact AWS for billing questions and service limit increases.

With Basic Support, you have access to a limited selection of AWS Trusted Advisor checks. Additionally, you can use the AWS Personal Health Dashboard, a tool that provides alerts and remediation guidance when AWS is experiencing events that may affect you.

If your company needs support beyond the Basic level, you could consider purchasing Developer, Business, Enterprise On-Ramp, and Enterprise Support.

#### Developer Support

Customers in the Developer Support plan have access to features such as:

- Best practice guidance
- Client-side diagnostic tools
- Building-block architecture support, which consists of guidance for how to use AWS offerings, features, and services together

For example, suppose that your company is exploring AWS services. You've heard about a few different AWS services. However, you're unsure of how to potentially use them together to build applications that can address your company's needs. In this scenario, the building-block architecture support that is included with the Developer Support plan could help you to identify opportunities for combining specific services and features.

#### Business Support

Customers with a Business Support plan have access to additional features, including:

- Use-case guidance to identify AWS offerings, features, and services that can best support your specific needs
- All AWS Trusted Advisor checks
- Limited support for third-party software, such as common operating systems and application stack components

Suppose that your company has the Business Support plan and wants to install a common third-party operating system onto your Amazon EC2 instances. You could contact AWS Support for assistance with installing, configuring, and troubleshooting the operating system. For advanced topics such as optimizing performance, using custom scripts, or resolving security issues, you may need to contact the third-party software provider directly.

#### Enterprise On-Ramp Support

In November 2021, AWS opened enrollment into AWS Enterprise On-Ramp Support plan. In addition to all the features included in the Basic, Developer, and Business Support plans, customers with an Enterprise On-Ramp Support plan have access to:

- A pool of Technical Account Managers to provide proactive guidance and coordinate access to programs and AWS experts
- A Cost Optimization workshop (one per year)
- A Concierge support team for billing and account assistance
- Tools to monitor costs and performance through Trusted Advisor and Health API/Dashboard

Enterprise On-Ramp Support plan also provides access to a specific set of proactive support services, which are provided by a pool of Technical Account Managers.

- Consultative review and architecture guidance (one per year)
- Infrastructure Event Management support (one per year)
- Support automation workflows
- 30 minutes or less response time for business-critical issues

#### Enterprise Support

In addition to all features included in the Basic, Developer, Business, and Enterprise On-Ramp support plans, customers with Enterprise Support have access to:

- A designated Technical Account Manager to provide proactive guidance and coordinate access to programs and AWS experts
- A Concierge support team for billing and account assistance
- Operations Reviews and tools to monitor health
- Training and Game Days to drive innovation
- Tools to monitor costs and performance through Trusted Advisor and Health API/Dashboard

The Enterprise plan also provides full access to proactive services, which are provided by a designated Technical Account Manager:

- Consultative review and architecture guidance
- Infrastructure Event Management support
- Cost Optimization Workshop and tools
- Support automation workflows
- 15 minutes or less response time for business-critical issues

#### Developer, Business, Enterprise On-Ramp, and Enterprise Support

The Developer, Business, Enterprise On-Ramp, and Enterprise Support plans include all the benefits of Basic Support, in addition to the ability to open an unrestricted number of technical support cases. These Support plans have pay-by-the-month pricing and require no long-term contracts.

The information in this course highlights only a selection of details for each Support plan. A complete overview of what is included in each Support plan, including pricing for each plan, is available on the AWS Support site.

In general, for pricing, the Developer plan has the lowest cost, the Business and Enterprise On-Ramp plans are in the middle, and the Enterprise plan has the highest cost.

#### Technical Account Manager (TAM)

The Enterprise On-Ramp and Enterprise Support plans include access to a Technical Account Manager (TAM).

The TAM is your primary point of contact at AWS. If your company subscribes to Enterprise Support or Enterprise On-Ramp, your TAM educates, empowers, and evolves your cloud journey across the full range of AWS services. TAMs provide expert engineering guidance, help you design solutions that efficiently integrate AWS services, assist with cost-effective and resilient architectures, and provide direct access to AWS programs and a broad community of experts.

For example, suppose that you are interested in developing an application that uses several AWS services together. Your TAM could provide insights into how to best use the services together. They achieve this, while aligning with the specific needs that your company is hoping to address through the new application.

### Migration and Innovation

#### AWS Cloud Adoption Framework

The **Cloud Adoption Framework** exists to provide advice to your company to enable a quick and smooth migration to AWS.

The different Perspectives are Business, People, and Governance Perspectives, which focus on the business capabilities, and then you have the Platform, Security and Operations Perspectives which focus on the technical capabilities.

Each Perspective is used to uncover gaps in your skills and processes, which are then recorded as inputs. These inputs are then used as the basis for creating what is called an **AWS Cloud Adoption Framework Action Plan** that you then use to guide your organization's change management as you journey to the cloud. Having an action plan that makes sense for your organization can help keep you on track. Migrating to the cloud can be complicated, but again, you're not alone in this, there are tons of resources to help you get started, and the Cloud Adoption Framework is a great place to look.

#### Business Perspective

The **Business Perspective** ensures that IT aligns with business needs and that IT investments link to key business results. Use the Business Perspective to create a strong business case for cloud adoption and prioritize cloud adoption initiatives. Ensure that your business strategies and goals align with your IT strategies and goals.

Common roles in the Business Perspective include:

- Business managers
- Finance managers
- Budget owners
- Strategy stakeholders

#### People Perspective

The **People Perspective** supports development of an organization-wide change management strategy for successful cloud adoption. Use the People Perspective to evaluate organizational structures and roles, new skill and process requirements, and identify gaps. This helps prioritize training, staffing, and organizational changes.

Common roles in the People Perspective include:

- Human resources
- Staffing
- People managers

#### Governance Perspective

The **Governance Perspective** focuses on the skills and processes to align IT strategy with business strategy. This ensures that you maximize the business value and minimize risks. Use the Governance Perspective to understand how to update the staff skills and processes necessary to ensure business governance in the cloud. Manage and measure cloud investments to evaluate business outcomes.

Common roles in the Governance Perspective include:

- Chief Information Officer (CIO)
- Program managers
- Enterprise architects
- Business analysts
- Portfolio managers

#### Platform Perspective

The **Platform Perspective** includes principles and patterns for implementing new solutions on the cloud, and migrating on-premises workloads to the cloud. Use a variety of architectural models to understand and communicate the structure of IT systems and their relationships. Describe the architecture of the target state environment in detail.

Common roles in the Platform Perspective include:

- Chief Technology Officer (CTO)
- IT managers
- Solutions architects

#### Security Perspective

The **Security Perspective** ensures that the organization meets security objectives for visibility, auditability, control, and agility. Use the AWS CAF to structure the selection and implementation of security controls that meet the organization's needs.

Common roles in the Security Perspective include:

- Chief Information Security Officer (CISO)
- IT security managers
- IT security analysts

#### Operations Perspective

The **Operations Perspective** helps you to enable, run, use, operate, and recover IT workloads to the level agreed upon with your business stakeholders. Define how day-to-day, quarter-to-quarter, and year-to-year business is conducted. Align with and support the operations of the business. The AWS CAF helps these stakeholders define current operating procedures and identify the process changes and training needed to implement successful cloud adoption.

Common roles in the Operations Perspective include:

- IT operations managers
- IT support managers

### Migration Strategies

#### 7 strategies for migration

When migrating applications to the cloud, 7 of the most common migration strategies(opens in a new tab) that you can implement are:

- Rehosting
- Replatforming
- Refactoring/re-architecting
- Repurchasing
- Relocate
- Retaining
- Retiring

**Rehosting:** This is otherwise known as **lift and shift**. And this is an easy thing for businesses to do because you're not making any changes. At least not at first. Just pick up the applications and move them pretty much as is onto AWS. You may not get all the possible benefits. But some companies found that even without any optimization, they could save up to 30% of their total costs just by rehosting. Also, we find it's easier to optimize applications later once they already live in the cloud. Because your organization has better skills to do so. The hard part, the migration, is already complete.

**Replatforming:** Or **lift, tinker, and shift**. It's still basically a lift and shift, but instead of a pure one-to-one, you might make a few cloud optimizations. But you're not touching any core code in the process. No new dev efforts are involved here. For example, you could take your existing MySQL database and replatform it onto RDS MySQL, without any code changes at all. Or even consider upgrading to Amazon Aurora. This gives significant benefit to your DBA team as well as improved performance without any code changes.

**Retire:** Some parts of your enterprise IT portfolio are just no longer needed. We found as much as 10% to 20% of companies' application portfolios include applications that are no longer being used or already have replacements live and functional. Using the AWS migration plan as the opportunity to actually **end-of-life** these applications can save significant cost and effort for your team. Sometimes you just have to turn off the lights.

**Retain:** Some applications are about to be deprecated but maybe not just yet. They still need to run but don't turn them off for another three months or eight months. These apps could be migrated to AWS, but why? You should only migrate what makes sense for your business. And then as time goes on, these applications can be deprecated where they live, and ultimately retired.

**Repurchase:** This is common for companies looking to abandon legacy software vendors and get a fresh start as part of migration. For example, ending a contract with an old CRM vendor and moving to a brand new one. Or perhaps finally ending your licensing with an out-of-date database vendor in favor of cloud-native database offerings. Now, this sounds great, but remember, you'll now be dealing with a new software package and some are easy to implement, some take time. The total upfront expense of the step, therefore, goes up, but the potential benefits could be substantial.

**Refactoring (also known as re-architecting):** Now, you're writing new code. This is driven by a strong business need to add features or performance that might not be possible on-prem, but now are within your reach. Dramatic changes to your architecture can be very beneficial to your enterprise but this will come at the highest initial cost in terms of planning and human effort.

### The Cloud Journey

### The AWS Well-Architected Framework

The **AWS Well-Architected Framework** helps you understand how to design and operate reliable, secure, efficient, and cost-effective systems in the AWS Cloud. It provides a way for you to consistently measure your architecture against best practices and design principles and identify areas for improvement.

#### The Well-Architected Framework is based on six pillars:

- Operational excellence
- Security
- Reliability
- Performance efficiency
- Cost optimization
- Sustainability

**Operational excellence Pillar** is the ability to run and monitor systems to deliver business value and to continually improve supporting processes and procedures.

Design principles for operational excellence in the cloud include performing operations as code, annotating documentation, anticipating failure, and frequently making small, reversible changes.

The **Security pillar** is the ability to protect information, systems, and assets while delivering business value through risk assessments and mitigation strategies.

When considering the security of your architecture, apply these best practices:

- Automate security best practices when possible.
- Apply security at all layers.
- Protect data in transit and at rest.

**Reliability Pillar** is the ability of a system to do the following:

- Recover from infrastructure or service disruptions
- Dynamically acquire computing resources to meet demand
- Mitigate disruptions such as misconfigurations or transient network issues

Reliability includes testing recovery procedures, scaling horizontally to increase aggregate system availability, and automatically recovering from failure.

**Performance efficiency Pillar** is the ability to use computing resources efficiently to meet system requirements and to maintain that efficiency as demand changes and technologies evolve.

Evaluating the performance efficiency of your architecture includes experimenting more often, using serverless architectures, and designing systems to be able to go global in minutes.

**Cost optimization Pillar** is the ability to run systems to deliver business value at the lowest price point.

Cost optimization includes adopting a consumption model, analyzing and attributing expenditure, and using managed services to reduce the cost of ownership.

**Sustainability Pillar** is the ability to continually improve sustainability impacts by reducing energy consumption and increasing efficiency across all components of a workload by maximizing the benefits from the provisioned resources and minimizing the total resources required.

To facilitate good design for sustainability:

- Understand your impact
- Establish sustainability goals
- Maximize utilization
- Anticipate and adopt new, more efficient hardware and software offerings
- Use managed services
- Reduce the downstream impact of your cloud workloads
