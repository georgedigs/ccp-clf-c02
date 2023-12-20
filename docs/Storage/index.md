## Storage:

### AWS Backup\*

_AWS Backup_ is a fully managed service that centralizes and automates data protection across AWS services and hybrid workloads. It provides core data protection features, ransomware recovery capabilities, and compliance insights and analytics for data protection policies and operations.

### Amazon Elastic Block Store (Amazon EBS)

_Amazon Elastic Block Store (Amazon EBS)_ is a service that provides block-level storage volumes that you can use with Amazon EC2 instances. If you stop or terminate an Amazon EC2 instance, all the data on the attached EBS volume remains available.

To create an EBS volume, you define the configuration (such as volume size and type) and provision it. After you create an EBS volume, it can attach to an Amazon EC2 instance.

Because EBS volumes are for data that needs to persist, it's important to back up the data. You can take incremental backups of EBS volumes by creating Amazon EBS snapshots.

#### _Amazon EBS snapshots_

An _EBS snapshot_ is an incremental backup. This means that the first backup taken of a volume copies all the data. For subsequent backups, only the blocks of data that have changed since the most recent snapshot are saved.

Incremental backups are different from full backups, in which all the data in a storage volume copies each time a backup occurs. The full backup includes data that has not changed since the most recent backup.

### Amazon Elastic File System (Amazon EFS)

_Amazon Elastic File System (Amazon EFS)_ is a scalable file system used with AWS Cloud services and on-premises resources. As you add and remove files, Amazon EFS grows and shrinks automatically. It can scale on demand to petabytes without disrupting applications.

### AWS Elastic Disaster Recovery\*

_AWS Elastic Disaster Recovery_ automatically converts your servers to boot and run natively on AWS when you launch instances for drills or recovery.

### Amazon FSx\*

_Amazon FSx_ for Windows File Server provides fully managed Microsoft Windows file servers, backed by a fully native Windows file system. FSx for Windows File Server has the features, performance, and compatibility to easily lift and shift enterprise applications to the AWS Cloud.

### Amazon S3

_Amazon Simple Storage Service (Amazon S3)_ is a service that provides object-level storage. Amazon S3 stores data as objects in buckets.

You can upload any type of file to Amazon S3, such as images, videos, text files, and so on. For example, you might use Amazon S3 to store backup files, media files for a website, or archived documents. Amazon S3 offers unlimited storage space. The maximum file size for an object in Amazon S3 is 5 TB.

When you upload a file to Amazon S3, you can set permissions to control visibility and access to it. You can also use the Amazon S3 versioning feature to track changes to your objects over time.

In _object storage_, each object consists of data, metadata, and a key.

The data might be an image, video, text document, or any other type of file. Metadata contains information about what the data is, how it is used, the object size, and so on. An object's key is its unique identifier.

In _file storage_, multiple clients (such as users, applications, servers, and so on) can access data that is stored in shared file folders. In this approach, a storage server uses block storage with a local file system to organize files. Clients access data through file paths.

Compared to block storage and object storage, file storage is ideal for use cases in which a large number of services and resources need to access the same data at the same time.

- Object sharing – the ability to make any object publicly available via a URL.
- Lifecycle management – set rules to transfer objects between storage classes at defined time intervals.
- Versioning – automatically keep multiple versions of an object (when enabled).
- Encryption can be enabled for bucket.
- Data is secured using ACLs and bucket policies.

#### S3 Charges:

- Storage.
- Requests.
- Storage management pricing.
- Data transfer pricing.
- Transfer acceleration.

_Typical use cases include:_

- _Backup and Storage_ – Provide data backup and storage services for others.
- _Application Hosting_ – Provide services that deploy, install, and manage web applications.
- _Media Hosting_ – Build a redundant, scalable, and highly available infrastructure that hosts video, photo, or music uploads and downloads.
- _Software Delivery_ – Host your software applications that customers can download.
- _Static Website_ – you can configure a static website to run from an S3 bucket.

_Amazon S3 storage classes_

With Amazon S3, you pay only for what you use. You can choose from a range of storage classes to select a fit for your business and cost needs. When selecting an Amazon S3 storage class, consider these two factors:

- How often you plan to retrieve your data
- How available you need your data to be

1. **S3 Standard**

   - Designed for frequently accessed data
   - Stores data in a minimum of three Availability Zones

   Amazon S3 Standard provides high availability for objects. This makes it a good choice for a wide range of use cases, such as websites, content distribution, and data analytics. Amazon S3 Standard has a higher cost than other storage classes intended for infrequently accessed data and archival storage.

2. **S3 Standard-Infrequent Access (S3 Standard-IA)**

   - Ideal for infrequently accessed data
   - Similar to Amazon S3 Standard but has a lower storage price and higher retrieval price

   Amazon S3 Standard-IA is ideal for data infrequently accessed but requires high availability when needed. Both Amazon S3 Standard and Amazon S3 Standard-IA store data in a minimum of three Availability Zones. Amazon S3 Standard-IA provides the same level of availability as Amazon S3 Standard but with a lower storage price and a higher retrieval price.

3. **S3 One Zone-Infrequent Access (S3 One Zone-IA)**

   - Stores data in a single Availability Zone
   - Has a lower storage price than Amazon S3 Standard-IA

   Compared to S3 Standard and S3 Standard-IA, which store data in a minimum of three Availability Zones, S3 One Zone-IA stores data in a single Availability Zone. This makes it a good storage class to consider if the following conditions apply:
   
   - You want to save costs on storage.
   - You can easily reproduce your data in the event of an Availability Zone failure.

4. **S3 Intelligent-Tiering**

   - Ideal for data with unknown or changing access patterns
   - Requires a small monthly monitoring and automation fee per object

   In the S3 Intelligent-Tiering storage class, Amazon S3 monitors objects' access patterns. If you haven't accessed an object for 30 consecutive days, Amazon S3 automatically moves it to the infrequent access tier, S3 Standard-IA. If you access an object in the infrequent access tier, Amazon S3 automatically moves it to the frequent access tier, S3 Standard.

5. **S3 Glacier Instant Retrieval**

   - Works well for archived data that requires immediate access
   - Can retrieve objects within a few milliseconds

   When you decide between the options for archival storage, consider how quickly you must retrieve the archived objects. You can retrieve objects stored in the S3 Glacier Instant Retrieval storage class within milliseconds, with the same performance as S3 Standard.

6. **S3 Glacier Flexible Retrieval**

   - Low-cost storage designed for data archiving
   - Able to retrieve objects within a few minutes to hours

   S3 Glacier Flexible Retrieval is a low-cost storage class that is ideal for data archiving. For example, you might use this storage class to store archived customer records or older photos and video files. You can retrieve your data from S3 Glacier Flexible Retrieval from 1 minute to 12 hours.

7. **S3 Glacier Deep Archive**

   - Lowest-cost object storage class ideal for archiving
   - Able to retrieve objects within 12 hours

   S3 Deep Archive supports long-term retention and digital preservation for data that might be accessed once or twice in a year. This storage class is the lowest-cost storage in the AWS Cloud, with data retrieval from 12 to 48 hours. All objects from this storage class are replicated and stored across at least three geographically dispersed Availability Zones.

8. **S3 Outposts**

   - Creates S3 buckets on Amazon S3 Outposts
   - Makes it easier to retrieve, store, and access data on AWS Outposts

   Amazon S3 Outposts delivers object storage to your on-premises AWS Outposts environment. Amazon S3 Outposts is designed to store data durably and redundantly across multiple devices and servers on your Outposts. It works well for workloads with local data residency requirements that must satisfy demanding performance needs by keeping data close to on-premises applications.

### AWS Storage Gateway\*

_AWS Storage Gateway_ is a hybrid cloud storage service that gives you on-premises access to virtually unlimited cloud storage. Storage Gateway provides a standard set of storage protocols such as iSCSI, SMB, and NFS, which allow you to use AWS storage without rewriting your existing applications.
