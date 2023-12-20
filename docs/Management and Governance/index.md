
## Management and Governance:

### AWS Auto Scaling\*

_AWS Auto Scaling_ monitors your applications and automatically adjusts capacity to maintain steady, predictable performance at the lowest possible cost. Using AWS Auto Scaling, it's easy to setup application scaling for multiple resources across multiple services in minutes.

### AWS CloudFormation

_AWS CloudFormation_ is an infrastructure as code tool that allows you to define a wide variety of AWS resources in a declarative way using JSON or YAML text-based documents called CloudFormation templates. A declarative format like this allows you to define what you want to build without specifying the details of exactly how to build it. CloudFormation lets you define what you want and the CloudFormation engine will worry about the details on calling APIs to get everything built out.

CloudFormation supports many different AWS resources from storage, databases, analytics, machine learning, and more. Once you define your resources in a CloudFormation template, CloudFormation will parse the template and begin provisioning all the resources you defined in parallel. CloudFormation manages all the calls to the backend AWS APIs for you. You can run the same CloudFormation template in multiple accounts or multiple regions, and it will create identical environments across them. There is less room for human error as it is a totally automated process.

### AWS CloudTrail

_AWS CloudTrail_ records API calls for your account. The recorded information includes the identity of the API caller, the time of the API call, the source IP address of the API caller, and more. You can think of CloudTrail as a "trail" of breadcrumbs (or a log of actions) that someone has left behind them.

Recall that you can use API calls to provision, manage, and configure your AWS resources. With CloudTrail, you can view a complete history of user activity and API calls for your applications and resources.

Events are typically updated in CloudTrail within 15 minutes after an API call. You can filter events by specifying the time and date that an API call occurred, the user who requested the action, the type of resource that was involved in the API call, and more.

AWS CloudTrail, the comprehensive API auditing tool. The engine is simple, every request made to AWS, it doesn't matter if it's to launch an EC2 instance, or add a row to a DynamoDB table, or change a user's permissions. Every request gets logged in the CloudTrail engine. The engine records exactly who made the request, which operator, when did they send the API call? Where were they? What was their IP address? And what was the response? Did something change? And what is the new state? Was the request denied?

From an auditing perspective, well, this is fabulous. So imagine that you're dealing with an auditor who is checking to make sure that nobody from the outside can access your database. That's a good thing. Well, okay, you build a security group that locks out external traffic. But remember that a root-level administrator still has permissions to change those settings, right?

Well, so how do you prove to the auditor that the security group settings never changed? The answer is CloudTrail. And then CloudTrail can save those logs indefinitely in secure S3 buckets. In addition, with tamper-proof methods like Vault Lock, you then can show absolute provenance of all of these critical security audit logs.

#### CloudTrail Insights

Within CloudTrail, you can also enable CloudTrail Insights(opens in a new tab). This optional feature allows CloudTrail to automatically detect unusual API activities in your AWS account.

For example, CloudTrail Insights might detect that a higher number of Amazon EC2 instances than usual have recently launched in your account. You can then review the full event details to determine which actions you need to take next.

### Amazon CloudWatch

_Amazon CloudWatch_ is a web service that enables you to monitor and manage various metrics and configure alarm actions based on data from those metrics.

CloudWatch uses metrics to represent the data points for your resources. AWS services send metrics to CloudWatch. CloudWatch then uses these metrics to create graphs automatically that show how performance has changed over time.

CloudWatch allows you to monitor your AWS infrastructure and the applications you run on AWS in real time. It works by tracking and monitoring metrics. Think of metrics as variables that are tied to your resources

#### _CloudWatch alarms_

With CloudWatch, you can create alarms(opens in a new tab) that automatically perform actions if the value of your metric has gone above or below a predefined threshold.

For example, suppose that your company's developers use Amazon EC2 instances for application development or testing purposes. If the developers occasionally forget to stop the instances, the instances will continue to run and incur charges.

In this scenario, you could create a CloudWatch alarm that automatically stops an Amazon EC2 instance when the CPU utilization percentage has remained below a certain threshold for a specified period. When configuring the alarm, you can specify to receive a notification whenever this alarm is triggered.

CloudWatch alarms are integrated with SNS. So we can then send an SMS to the manager to say, clean the machine. You can create all sorts of custom alarms for metrics from all different types of AWS resources.

The _CloudWatch dashboard_ feature enables you to access all the metrics for your resources from a single location. For example, you can use a CloudWatch dashboard to monitor the CPU utilization of an Amazon EC2 instance, the total number of requests made to an Amazon S3 bucket, and more. You can even customize separate dashboards for different business purposes, applications, or resources.

#### _CloudWatch benefits_

1. You can have access to all your _metrics from a central location_. This enables you to collect metrics and logs from all your AWS resources applications, and services that run on AWS and on-premises servers, helping you break down silos so that you can easily gain system-wide visibility.
2. You can also get _visibility across your applications_, infrastructure, and services, which means you gain insights across your distributed stack so you can correlate and visualize metrics and logs to quickly pinpoint and resolve issues. This in turn means you can reduce mean time to resolution, or MTTR, and improve total cost of ownership, or TCO.
3. This means _freeing up important resources_ like developers to focus on adding business value. you can drive insights to optimize applications and operational resources. By, for example, aggregating usage across an entire fleet of EC2 instances to derive operational and utilization insights.

### AWS Compute Optimizer\*

_AWS Compute Optimizer_ is a service that analyzes the configuration and utilization metrics of your AWS resources. It reports whether your resources are optimal, and generates optimization recommendations to reduce the cost and improve the performance of your workloads. Compute Optimizer also provides graphs showing recent utilization metric history data, as well as projected utilization for recommendations, which you can use to evaluate which recommendation provides the best price-performance trade-off. The analysis and visualization of your usage patterns can help you decide when to move or resize your running resources, and still meet your performance and capacity requirements.

### AWS Config\*

_AWS Config_ is a fully managed service that provides you with resource inventory, configuration history, and configuration change notifications to use security and governance. With AWS Config, you can discover existing AWS resources, record configurations for third-party resources, export a complete inventory of your resources with all configuration details, and determine how a resource was configured at any point in time. These capabilities use compliance auditing, security analysis, resource change tracking, and troubleshooting.

### AWS Control Tower\*

_AWS Control Tower_ offers a straightforward way to set up and govern an AWS multi-account environment, following prescriptive best practices. AWS Control Tower orchestrates the capabilities of several other AWS services, including AWS Organizations, AWS Service Catalog, and AWS IAM Identity Center (successor to AWS Single Sign-On), to build a landing zone in less than an hour. Resources are set up and managed on your behalf.

AWS Control Tower orchestration extends the capabilities of AWS Organizations. To help keep your organizations and accounts from drift, which is divergence from best practices, AWS Control Tower applies controls (sometimes called guardrails). For example, you can use controls to help ensure that security logs and necessary cross-account access permissions are created, and not altered.

### AWS Health Dashboard\*

_AWS Health Dashboard_ is the single place to learn about the availability and operations of AWS services. You can view the overall status of AWS services, and you can sign in to view personalized communications about your particular AWS account or organization. Your account view provides deeper visibility into resource issues, upcoming changes, and important notifications.

### AWS Launch Wizard\*

_AWS Launch Wizard_ is a console-based service to quickly and easily size, configure, and deploy third-party applications on AWS without the need to identify and provision individual AWS resources.

### AWS License Manager\*

_License Manager_ provides you with the flexibility and control to manage license usage to match your organizational structure and processes. License Manager can be set in different configurations to address specific business needs.

### AWS Management Console

_The AWS Management Console_ is browser-based interface. Through the console, you can manage your AWS resources visually and in a way that is easy to digest. This is great for getting started and building your knowledge of the services. It's also useful for building out test environments or viewing AWS bills, viewing monitoring, and working with other non-technical resources. You can quickly access recently used services and search for other services by name, keyword, or acronym. The console includes wizards and automated workflows that can simplify the process of completing tasks.
 You can also use the AWS Console mobile application to perform tasks such as monitoring resources, viewing alarms, and accessing billing information. Multiple identities can stay logged into the AWS Console mobile app at the same time.

### AWS Organizations

Suppose that your company has multiple AWS accounts. You can use  **AWS Organizations****  **to consolidate and manage multiple AWS accounts within a central location.

When you create an organization, AWS Organizations automatically creates a  **root** , which is the parent container for all the accounts in your organization.

In AWS Organizations, you can centrally control permissions for the accounts in your organization by using **service control policies (SCPs)**.

#### service control policies (SCPs)

SCPs enable you to place restrictions on the AWS services, resources, and individual API actions that users and roles in each account can access.

#### Organizational units (OU)

In AWS Organizations, you can group accounts into organizational units (OUs) to make it easier to manage accounts with similar business or security requirements. When you apply a policy to an OU, all the accounts in the OU automatically inherit the permissions specified in the policy.

By organizing separate accounts into OUs, you can more easily isolate workloads or applications that have specific security requirements. For instance, if your company has accounts that can access only the AWS services that meet certain regulatory requirements, you can put these accounts into one OU. Then, you can attach a policy to the OU that blocks access to all other AWS services that do not meet the regulatory requirements.

_Consolidated Billing_. At the end of every month, instead of having to pay an AWS bill for every single account, you can roll those bills up into one bill owned by the owner of the organization. This makes it easier to keep track of your bills. You don't get 100 bills, if you have 100 AWS accounts.

You can still view your AWS bill in an itemized fashion. So you know which accounts spent what, but it all goes into one central location for ease of viewing. There are other benefits of using this feature too. One of them is that the usage for AWS resources is rolled up to the organization level. AWS does offer bulk pricing. Each individual account may only have a small amount of usage, but you can get the bulk discount pricing because of the aggregate across all accounts in the organization. In addition, if you have a savings plan in place, or if you are using reserved instances for EC2, it can be shared across AWS accounts in the organization. The best part about this is that the feature is free and easy to use. So it simplifies the billing process, lets you share savings across accounts and doesn't cost you any extra money.

### AWS Resource Groups and Tag Editor\*

_Resource Groups_ to organize your AWS resources. AWS Resource Groups is the service that lets you manage and automate tasks on large numbers of resources at one time.

_Tags_ are key and value pairs that act as metadata for organizing your AWS resources. With most AWS resources, you have the option of adding tags when you create the resource. Examples of resources include an Amazon Elastic Compute Cloud (Amazon EC2) instance, an Amazon Simple Storage Service (Amazon S3) bucket, or a secret in AWS Secrets Manager.

### AWS Service Catalog\*

_AWS Service Catalog_ lets you centrally manage your cloud resources to achieve governance at scale of your infrastructure as code (IaC) templates, written in CloudFormation or Terraform configurations. With AWS Service Catalog, you can meet your compliance requirements while making sure your customers can quickly deploy the cloud resources they need.

### AWS Systems Manager\*

_AWS Systems Manager_ allows you to safely automate common and repetitive IT operations and management tasks. With Systems Manager Automation, you use predefined playbooks, or you can build, run, and share wiki-style automated playbooks to enable AWS resource management across multiple accounts and AWS Regions.

### AWS Trusted Advisor

_AWS Trusted Advisor_ is a web service that inspects your AWS environment and provides real-time recommendations in accordance with AWS best practices.

Trusted Advisor compares its findings to AWS best practices in five categories: cost optimization, performance, security, fault tolerance, and service limits. For the checks in each category, Trusted Advisor offers a list of recommended actions and additional resources to learn more about AWS best practices.

The guidance provided by AWS Trusted Advisor can benefit your company at all stages of deployment. For example, you can use AWS Trusted Advisor to assist you while you are creating new workflows and developing new applications. You can also use it while you are making ongoing improvements to existing applications and resources.

#### _AWS Trusted Advisor dashboard_

When you access the Trusted Advisor dashboard on the AWS Management Console, you can review completed checks for cost optimization, performance, security, fault tolerance, and service limits.

For each category:

- The green check indicates the number of items for which it detected no problems.
- The orange triangle represents the number of recommended investigations.
- The red circle represents the number of recommended actions.

#### _Trusted Advisor 5 Pillars:_

1.
#### _Cost Optimization_

Trusted Advisor can help you save cost with actionable recommendations by analyzing usage, configuration and spend. Examples include identifying idle RDS DB instances, underutilized EBS volumes, unassociated Elastic IP addresses, and excessive timeouts in Lambda functions.

1.
#### _Performance_

Trusted Advisor can help improve the performance of your services with actionable recommendations by analyzing usage and configuration. Examples include analyzing EBS throughput and latency, compute usage of EC2 instances, and configurations on CloudFront.

1.
#### _Security_

Trusted Advisor can help improve the security of your AWS environment by suggesting foundational security best practices curated by security experts. Examples include identifying RDS security group access risk, exposed access keys, and unnecessary S3 bucket permissions.

1.
#### _Fault Tolerance_

Trusted Advisor can help improve the reliability of your services. Examples include examining Auto scaling EC2 groups, deleted health checks on Route 53, disabled Availability Zones, and disabled RDS backups.

1.
#### _Service Limits (quotas)_

Service quotas are the maximum number of resources that you can create in an AWS account. AWS implements quotas to provide highly available and reliable service to all customers, and protects you from unintentional spend. Trusted Advisor will notify you once you reach more than 80% of a service quota. You can then follow recommendations to delete resources or request a quota increase.

### AWS Well-Architected Tool

The AWS Well-Architected Tool lets you review your workloads against current AWS best practices and obtain advice on how to architect your workloads for the cloud. This tool uses the AWS Well-Architected Framework.

It kind of looks like a traffic light system, with green being go, keep up the good work. Orange being, you should probably look into this because there's room for improvement. And red being, okay, you should look at this because something is at risk. These are areas where the tool has detected potential issues, and it presents you with a plan on how to architect using established best practices. It should be noted that you can always override these settings if the questions don't apply to your scenario. It's very customizable.

### AWS OpsWorks

AWS OpsWorks is a configuration management service that provides managed instances of Chef and Puppet. Chef and Puppet are automation platforms that allow you to use code to automate the configurations of your servers. OpsWorks lets you use Chef and Puppet to automate how servers are configured, deployed, and managed across your Amazon EC2 instances or on-premises compute environments.