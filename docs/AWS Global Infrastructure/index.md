## AWS Global Infrastructure:

### Regions & Availability Zones:

Each Region is made up of multiple data centers. AWS calls a single data center or a group of data centers, an Availability Zone or AZ. Each Availability Zone is one or more discrete data centers with redundant power, networking, and connectivity. When you launch an Amazon EC2 instance, it launches a virtual machine on a physical hardware that is installed in an Availability Zone. This means each AWS Region consists of multiple isolated and physically separate Availability Zones within a geographic Region. As a best practice with AWS, we always recommend you run across at least two Availability Zones in a Region. This means redundantly deploying your infrastructure in two different AZs.

#### Some key points about Regions:

- Regions are geographically isolated areas, where you can access services needed to run your enterprise.

- Regions contain Availability Zones, that allow you to run across physically separated buildings, tens of miles of separation, while keeping your application logically unified. Availability Zones help you solve high availability and disaster recovery scenarios, without any additional effort on your part.

- AWS Edge locations run Amazon CloudFront to help get content closer to your customers, no matter where they are in the world.

### Selecting a Region

When determining the right Region for your services, data, and applications, consider the following four business factors:

1. **Compliance with data governance and legal requirements:**

   Depending on your company and location, you might need to run your data out of specific areas. For example, if your company requires all of its data to reside within the boundaries of the UK, you would choose the London Region.

   Not all companies have location-specific data regulations, so you might need to focus more on the other three factors.

2. **Proximity to your customers:**

   Selecting a Region that is close to your customers will help you to get content to them faster.

3. **Available services within a Region:**

   Sometimes, the closest Region might not have all the features that you want to offer to customers.

4. **Pricing:**

   Suppose that you are considering running applications in both the United States and Brazil. The way Brazil's tax structure is set up, it might cost 50% more to run the same workload out of the São Paulo Region compared to the Oregon Region.

### Availability Zones

An Availability Zone is a single data center or a group of data centers within a Region. Availability Zones are located tens of miles apart from each other. This is close enough to have low latency (the time between when content requested and received) between Availability Zones. However, if a disaster occurs in one part of the Region, they are distant enough to reduce the chance that multiple Availability Zones are affected.

### Edge Locations

An edge location is a site that Amazon CloudFront uses to store cached copies of your content closer to your customers for faster delivery.

Edge locations are separate from Regions, so you can push content from inside a Region to a collection of Edge locations around the world, in order to accelerate communication and content delivery. AWS Edge locations also run more than just CloudFront. They run a domain name service, or DNS, known as Amazon Route 53, helping direct customers to the correct web locations with reliably low latency.
