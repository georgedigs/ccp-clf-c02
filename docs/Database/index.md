
## Database:

### Amazon Aurora

_Amazon Aurora_is an enterprise-class relational database. It is compatible with MySQL and PostgreSQL relational databases. It is up to five times faster than standard MySQL databases and up to three times faster than standard PostgreSQL databases.

Amazon Aurora helps to reduce your database costs by reducing unnecessary input/output (I/O) operations, while ensuring that your database resources remain reliable and available.

Consider Amazon Aurora if your workloads require high availability. It replicates six copies of your data across three Availability Zones and continuously backs up your data to Amazon S3.

The other benefits are things like your data is replicated across facilities, so you have six copies at any given time. You can also deploy up to 15 read replicas, so you can offload your reads and scale performance. Additionally, there's continuous backups to S3, so you always have a backup ready to restore. You also get point in time recovery, so you can recover data from a specific period.

### Amazon DynamoDB

_Amazon DynamoDB_ is a key-value database service. It delivers single-digit millisecond performance at any scale.

**DynamoDB is serverless** , which means that you do not have to provision, patch, or manage servers. You also do not have to install, maintain, or operate software.

As the size of your database shrinks or grows, **DynamoDB automatically scales** to adjust for changes in capacity while maintaining consistent performance. This makes it a suitable choice for use cases that require high performance while scaling.

DynamoDB is a non-relational, NoSQL database. It is purpose built. Meaning it has specific use cases, and it isn't the best fit for every workload out there. It has millisecond response time. It's fully managed, and it's highly scalable.

_Amazon DynamoDB Accelerator (DAX)_ is an in-memory cache for DynamoDB. It helps improve response times from single-digit milliseconds to microseconds.

### Amazon MemoryDB for Redis\*

MemoryDB for Redis is a durable, in-memory database service that delivers ultra-fast performance. It is purpose-built for modern applications with microservices architectures.

MemoryDB is compatible with Redis, a popular open source data store, enabling you to quickly build applications using the same flexible and friendly Redis data structures, APIs, and commands that they already use today. With MemoryDB, all of your data is stored in memory, which enables you to achieve microsecond read and single-digit millisecond write latency and high throughput. MemoryDB also stores data durably across multiple Availability Zones (AZs) using a Multi-AZ transactional log to enable fast failover, database recovery, and node restarts.

### Amazon Neptune

_Amazon Neptune_ is a graph database service. You can use Amazon Neptune to build and run applications that work with highly connected datasets, such as recommendation engines, fraud detection, and knowledge graphs.

### Amazon RDS

_Amazon Relational Database Service (Amazon RDS)_ is a service that enables you to run relational databases in the AWS Cloud.

Amazon RDS is a managed service that automates tasks such as hardware provisioning, database setup, patching, and backups. With these capabilities, you can spend less time completing administrative tasks and more time using data to innovate your applications. You can integrate Amazon RDS with other services to fulfill your business and operational needs, such as using AWS Lambda to query your database from a serverless application.

Amazon RDS provides a number of different security options. Many Amazon RDS database engines offer encryption at rest (protecting data while it is stored) and encryption in transit (protecting data while it is being sent and received).

#### _Amazon RDS database engines_

Amazon RDS is available on six database engines, which optimize for memory, performance, or input/output (I/O). Supported database engines include:

1. Amazon Aurora
2. PostgreSQL
3. MySQL
4. MariaDB
5. Oracle Database
6. Microsoft SQL Server