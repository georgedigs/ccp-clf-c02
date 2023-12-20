## Networking and Content Delivery:

### Amazon API Gateway*

_Amazon API Gateway_ is a fully managed service that makes it easy for developers to publish, maintain, monitor, and secure APIs at any scale. With a few clicks in the AWS Management Console, you can create an API that acts as a "front door" for applications to access data, business logic, or functionality from your back-end services, such as applications running on Amazon Elastic Compute Cloud (Amazon EC2), Amazon Elastic Container Service (Amazon ECS) or AWS Elastic Beanstalk, code running on AWS Lambda, or any web application. Amazon API Gateway handles all of the tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls, including traffic management, authorization and access control, monitoring, and API version management. Amazon API Gateway has no minimum fees or startup costs. For HTTP APIs and REST APIs, you pay only for the API calls you receive and the amount of data transferred out. For WebSocket APIs, you pay only for messages sent and received and for the time a user/device is connected to the WebSocket API.

### Amazon CloudFront

_Amazon CloudFront_ is a service that helps deliver data, video, applications, and APIs to customers around the world with low latency and high transfer speeds. Amazon CloudFront uses what are called Edge locations, all around the world, to help accelerate communication with users, no matter where they are.

Amazon CloudFront is a content delivery network (CDN) that allows you to store (cache) your content at "edge locations" located around the world.

This allows customers to access content more quickly and provides security against DDoS attacks.

CloudFront can be used for data, videos, applications, and APIs.

#### CloudFront benefits:

1. Cache content at Edge Location for fast distribution to customers.
2. Built-in Distributed Denial of Service (DDoS) attack protection.
3. Integrates with many AWS services (S3, EC2, ELB, Route 53, Lambda).

#### Origins and Distributions:

1. An origin is the origin of the files that the CDN will distribute.
2. Origins can be either an S3 bucket, an EC2 instance, an Elastic Load Balancer, or Route 53 – can also be external (non-AWS).
3. To distribute content with CloudFront you need to create a distribution.

#### CloudFront uses Edge Locations and Regional Edge Caches:

1. An edge location is the location where content is cached (separate to AWS regions/AZs).
2. Requests are automatically routed to the nearest edge location.
3. Regional Edge Caches are located between origin web servers and global edge locations and have a larger cache.
4. Regional Edge caches aim to get content closer to users.

### AWS Direct Connect

_AWS Direct Connect_. Direct Connect allows you to establish a completely private, dedicated fiber connection from your data center to AWS. You work with a Direct Connect partner in your area to establish this connection, because like my magic doorway, AWS Direct Connect provides a physical line that connects your network to your AWS VPC. This can help you meet high regulatory and compliance needs, as well as sidestep any potential bandwidth issues.

[**AWS Direct Connect**](https://aws.amazon.com/directconnect/) is a service that lets you establish a dedicated private connection between your data center and a VPC.

### AWS Global Accelerator*

_AWS Global Accelerator_ is a networking service that helps you improve the availability, performance, and security of your public applications. Global Accelerator provides two global static public IPs that act as a fixed entry point to your application endpoints, such as Application Load Balancers, Network Load Balancers, Amazon Elastic Compute Cloud (EC2) instances, and elastic IPs.

### Amazon Route 53

_Amazon Route 53_ is AWS's domain name service, or DNS, and it's highly available and scalable. But wait, what is DNS, you say? Think of DNS as a translation service. But instead of translating between languages, it translates website names into IP, or Internet Protocol, addresses that computers can read.

Route 53 can direct traffic to different endpoints using several different routing policies, such as latency-based routing, geolocation DNS, geoproximity, and weighted round robin. If we take geolocation DNS, that means we direct traffic based on where the customer is located.

You can even use Route 53 to register domain names, so you can buy and manage your own domain names right on AWS.

Amazon Route 53 is a DNS web service. It gives developers and businesses a reliable way to route end users to internet applications hosted in AWS.

Amazon Route 53 connects user requests to infrastructure running in AWS (such as Amazon EC2 instances and load balancers). It can route users to infrastructure outside of AWS.

Another feature of Route 53 is the ability to manage the DNS records for domain names. You can register new domain names directly in Route 53. You can also transfer DNS records for existing domain names managed by other domain registrars. This enables you to manage all of your domain names within a single location.

#### Route 53 performs three main functions:

_Domain registration_ – Route 53 allows you to register domain names.

_Domain Name Service (DNS)_ – Route 53 translates name to IP addresses using a global network of authoritative DNS servers.

_Health checking – Route 53_ sends automated requests to your application to verify that it's reachable, available, and functional.

#### Policy What it Does

_Simple_ - Simple DNS response providing the IP address associated with a name.

_Failover_ - If primary is down (based on health checks), routes to secondary destination.

_Geolocation_ - Uses geographic location you're in (e.g. Europe) to route you to the closest region.

_Geoproximity_ - Routes you to the closest region within a geographic area.

_Latency_ - Directs you based on the lowest latency route to resources.

_Multivalue answer_ - Returns several IP addresses and functions as a basic load balancer.

_Weighted_ - Uses the relative weights assigned to resources to determine which to route to.

### Amazon VPC

_Amazon VPC_ enables you to provision an isolated section of the AWS Cloud. In this isolated section, you can launch resources in a virtual network that you define. Within a virtual private cloud (VPC), you can organize your resources into subnets. A **subnet** is a section of a VPC that can contain resources such as Amazon EC2 instances.

You place resources into different subnets. Subnets are chunks of IP addresses in your VPC that allow you to group resources together. Subnets, along with networking rules control whether resources are either publicly or privately available.

In a VPC, subnets can communicate with each other. For example, you might have an application that involves Amazon EC2 instances in a public subnet communicating with databases that are located in a private subnet.

_Internet gateway (igw)_ An internet gateway is a connection between a VPC and the internet. You can think of an internet gateway as being similar to a doorway that customers use to enter the coffee shop. Without an internet gateway, no one can access the resources within your VPC.

_Virtual private gateway_ To access private resources in a VPC, you can use a **virtual private gateway.** A virtual private gateway enables you to establish a virtual private network (VPN) connection between your VPC and a private network, such as an on-premises data center or internal corporate network. A virtual private gateway allows traffic into the VPC only if it is coming from an approved network.

### AWS VPN*

AWS VPN is comprised of two services: AWS Site-to-Site VPN and AWS Client VPN. AWS Site-to-Site VPN enables you to securely connect your on-premises network or branch office site to your Amazon Virtual Private Cloud (Amazon VPC). AWS Client VPN enables you to securely connect users to AWS or on-premises networks.

#### _AWS Client VPN_

_AWS Client VPN_ is a fully managed, elastic VPN service that automatically scales up or down based on user demand. Because it is a cloud VPN solution, you don't need to install and manage hardware or software-based solutions, or try to estimate how many remote users to support at one time.

#### AWS Site-to-Site VPN

_AWS Site-to-Site VPN_ creates a secure connection between your data center or branch office and your AWS cloud resources. For globally distributed applications, the accelerated Site-to-Site VPN option provides even greater performance by working with AWS Global Accelerator.
