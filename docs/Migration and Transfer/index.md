
## Migration and Transfer:

### AWS Application Discovery Service\*

_AWS Application Discovery Service_ collects and presents data to enable enterprise customers to understand the configuration, usage, and behavior of servers in their IT environments. Server data is retained in the Application Discovery Service where it can be tagged and grouped into applications to help organize AWS migration planning. Collected data can be exported for analysis in Excel or other cloud migration analysis tools.

### AWS Application Migration Service\*

_AWS Application Migration Service_ minimizes time-intensive, error-prone manual processes by automating the conversion of your source servers to run natively on AWS. It also simplifies application modernization with built-in and custom optimization options.

### AWS Database Migration Service (AWS DMS)

_AWS Database Migration Service (AWS DMS)_ enables you to migrate relational databases, nonrelational databases, and other types of data stores.

With AWS DMS, you move data between a source database and a target database. The source and target databases can be of the same type or different types. During the migration, your source database remains operational, reducing downtime for any applications that rely on the database.

For example, suppose that you have a MySQL database that is stored on premises in an Amazon EC2 instance or in Amazon RDS. Consider the MySQL database to be your source database. Using AWS DMS, you could migrate your data to a target database, such as an Amazon Aurora database.

_Use Cases_

1. _Development and test migration_ Enabling developers to test applications against production data without affecting production users
2. _Database consolidation_is when you have several databases and want to consolidate them into one central database.
3. _Continuous Replication_is when you use DMS to perform continuous data replication. This could be for disaster recovery or because of geographic separation.

### AWS Migration Hub\*

_AWS Migration Hub_ provides access to the tools you need to collect and inventory your existing IT assets based on actual usage, analyze application components and infrastructure dependencies, and group resources into applications. You can generate migration strategy and Amazon Elastic Compute Cloud (EC2) instance recommendations for business case and migration planning, track the progress of application migrations to AWS, and modernize applications already running on AWS.

### AWS Schema Conversion Tool (AWS SCT)\*

_AWS Schema Conversion Tool (AWS SCT)_ to convert your existing database schema from one database engine to another. You can convert relational OLTP schema, or data warehouse schema.

### AWS Snow Family

It should be noted that all Snow Family devices are designed to be secure and tamper-resistant while on-site or in transit. This means the hardware and software is cryptographically signed, and all data stored is automatically encrypted using 256-bit encryption keys, owned and managed by you, the customer. You can even use AWS Key Management Service to generate and manage keys.

_AWS Snowcone_ and it's a device that holds up to eight terabytes of data and contains edge computing. Edge computing options are Amazon EC2 instances and AWS IoT Greengrass. To obtain one, you place an order via AWS Management Console we ship it to you, you plug it in and copy your data, and finally, ship it back to us. We'll then copy the data to your AWS account, usually an Amazon S3 bucket that you own and your data is available to use. Customers usually use these devices to ship terabytes of information such as analytics data, video libraries, image collections, backups, and even tape replacement data.

AWS Snowcone is a small, rugged, and secure edge computing and data transfer device. It features 2 CPUs, 4 GB of memory, and up to 14 TB of usable storage.

_Snowball Edge_. It comes in two versions: a Snowball Edge Compute Optimized option and a Snowball Edge Storage Optimized option. Even better is that they fit into existing server racks and can be clustered for greater computing needs. Ones you plug them into your infrastructure, you can even run AWS Lambda functions, Amazon EC2-compatible AMI's, or even AWS IoT Greengrass to perform simple processing of data right then and there. Customers usually ship these to remote locations, where it's trickier to have a lot of computing power lying around. The use cases include capturing of streams from IoT devices, image compression, video transcoding, and even industrial signaling.

#### AWS Snowball offers two types of devices:

_Snowball Edge Storage Optimized_ devices are well suited for large-scale data migrations and recurring transfer workflows, in addition to local computing with higher capacity needs.

- Storage: 80 TB of hard disk drive (HDD) capacity for block volumes and Amazon S3 compatible object storage, and 1 TB of SATA solid state drive (SSD) for block volumes.
- Compute: 40 vCPUs, and 80 GiB of memory to support Amazon EC2 sbe1 instances (equivalent to C5).

_Snowball Edge Compute Optimized_ provides powerful computing resources for use cases such as machine learning, full motion video analysis, analytics, and local computing stacks.

- Storage: 80-TB usable HDD capacity for Amazon S3 compatible object storage or Amazon EBS compatible block volumes and 28 TB of usable NVMe SSD capacity for Amazon EBS compatible block volumes.
- Compute: 104 vCPUs, 416 GiB of memory, and an optional NVIDIA Tesla V100 GPU. Devices run Amazon EC2 sbe-c and sbe-g instances, which are equivalent to C5, M5a, G3, and P3 instances.

_AWS Snowmobile_, and as the name suggests, it's housed in a 45-foot rugged shipping container and pulled along by a freaking truck, I mean this thing is huge. It houses 100 petabytes and is ideal for the largest migrations and even data center shutdowns. We drive the truck to your designated location, plug it in, and it then appears as a network attached storage device with, like I said, capacity of up to 100 petabytes. It is tamper resistant, waterproof, temperature controlled, it even has fire suppression and GPS tracking. I mean, can you believe that it also has 24/7 video surveillance with a dedicated security team and escort security vehicle during transit? That's some serious business.

AWS Snowmobile is an exabyte-scale data transfer service used to move large amounts of data to AWS.

- You can transfer up to 100 petabytes of data per Snowmobile, a 45-foot long ruggedized shipping container, pulled by a semi trailer truck.

### AWS Transfer Family\*

#### _AWS Transfer Family_ Managed File Transfer (MFT)

The AWS Transfer Family offers fully managed support for the transfer of files over SFTP, AS2, FTPS, and FTP directly into and out of Amazon S3 or Amazon EFS. You can seamlessly migrate, automate, and monitor your file transfer workflows by maintaining existing client-side configurations for authentication, access, and firewalls — so nothing changes for your customers, partners, and internal teams, or their applications.

_SFTP stands for Secure Shell (SSH) File Transfer Protocol_, a network protocol used for secure transfer of data over the internet. The protocol supports the full security and authentication functionality of SSH, and is widely used to exchange data between business partners in a variety of industries including financial services, healthcare, media and entertainment, retail, advertising, and more.

_FTP stands for File Transfer Protocol_, a network protocol used for the transfer of data. FTP uses a separate channel for control and data transfers. The control channel is open until terminated or inactivity timeout, the data channel is active for the duration of the transfer. FTP uses cleartext and does not support encryption of traffic.

_FTPS stands for File Transfer Protocol over SSL_, and is an extension to FTP. Like FTP, FTPS uses a separate channel for control and data transfers. The control channel is open until terminated or inactivity timeout, while the data channel is active for the duration of the transfer. FTPS uses Transport Layer Security (TLS) to encrypt traffic, and allows encryption of both the control and data channel connections either concurrently or independently.