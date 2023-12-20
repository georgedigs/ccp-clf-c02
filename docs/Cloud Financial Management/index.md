## Cloud Financial Management:

### AWS Billing Conductor\*

AWS Billing Conductor is a custom billing service that can support the show back and chargeback workflows of AWS Solution Providers and Enterprise customers. Using AWS Billing Conductor, you can customize a second, alternative version of your monthly billing data.

### AWS Budgets

In AWS Budgets, you can create budgets to plan your service usage, service costs, and instance reservations. The information in AWS Budgets updates three times a day. This helps you to accurately determine how close your usage is to your budgeted amounts or to the AWS Free Tier limits. In AWS Budgets, you can also set custom alerts when your usage exceeds (or is forecasted to exceed) the budgeted amount.

#### Example: AWS Budgets:

Suppose that you have set a budget for Amazon EC2. You want to ensure that your company's usage of Amazon EC2 does not exceed $200 for the month.

In AWS Budgets, you could set a custom budget to notify you when your usage has reached half of this amount ($100). This setting would allow you to receive an alert and decide how you would like to proceed with your continued use of Amazon EC2.

### AWS Cost and Usage Report\*

AWS Cost and Usage Reports (AWS CUR) contains the most comprehensive set of cost and usage data available. You can use Cost and Usage Reports to publish your AWS billing reports to an Amazon Simple Storage Service (Amazon S3) bucket that you own. You can receive reports that break down your costs by the hour, day, or month, by product or product resource, or by tags that you define yourself. AWS updates the report in your bucket once a day in comma-separated value (CSV) format. You can view the reports using spreadsheet software such as Microsoft Excel or Apache OpenOffice Calc, or access them from an application using the Amazon S3 API.

AWS Cost and Usage Reports tracks your AWS usage and provides estimated charges associated with your account. Each report contains line items for each unique combination of AWS products, usage type, and operation that you use in your AWS account. You can customize the AWS Cost and Usage Reports to aggregate the information either by the hour, day, or month.

#### AWS Cost and Usage Reports can do the following:

- Deliver report files to your Amazon S3 bucket

- Update the report up to three times a day

- Create, retrieve, and delete your reports using the AWS CUR API Reference

### AWS Cost Explorer

AWS Cost Explorer is a tool that lets you visualize, understand, and manage your AWS costs and usage over time.

AWS Cost Explorer includes a default report of the costs and usage for your top five cost-accruing AWS services. You can apply custom filters and groups to analyze your data. For example, you can view resource usage at the hourly level. It will show you which services you are spending the most money on, and it gives you 12 months of historical data.

One important grouping to note is to group by tag. Many resources in AWS are taggable. Tags are essentially user-defined key-value pairs. So you can tag an EC2 instance with a specific project name or a database with the same project name, and then you can come into the AWS Cost Explorer, filter by tag, and see all of the expenses associated with that tag. Cost Explorer also allows you to create custom reports.

Cost Explorer gives you some powerful defaults for reports, but you can build your own custom ones as well. This will help you identify cost drivers and take action when necessary to curb spending. Cost optimization is a priority you should be paying close attention to, and you can use the Cost Explorer to help get you going in the right direction.

### AWS Marketplace

AWS Marketplace is a digital catalog that includes thousands of software listings from independent software vendors. You can use AWS Marketplace to find, test, and buy software that runs on AWS.

For each listing in AWS Marketplace, you can access detailed information on pricing options, available support, and reviews from other AWS customers.

You can also explore software solutions by industry and use case. For example, suppose your company is in the healthcare industry. In AWS Marketplace, you can review use cases that software helps you to address, such as implementing solutions to protect patient records or using machine learning models to analyze a patient's medical history and predict possible health risks.
