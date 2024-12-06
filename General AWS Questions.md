# What is Amazon S3, and what are its key features?
S3 stands for Simple Storage Service. that you can use store any amount of data, at any time, from anywhere in the world. with pay only for what you use and payment model is pay as you go.
  ## key features : 
  Scalability: Stores unlimited data.
  Durability: 99.999999999% data durability.
  Security: Supports encryption and access control.
  Storage Classes: Options like Standard, Glacier for cost optimization
  Versioning: Keeps multiple versions of files.
  Lifecycle Policies: Automates data transfer to cheaper storage.

# What is Amazon CloudFront, and why is it used?
Amazon CloudFront is a content delivery network (CDN) service by AWS. It delivers content (like websites, videos, or Photos) to users with low latency and high transfer speed 
  ## Why is it used?
  Faster Delivery: CloudFront sends content from the nearest server to the user, making it load quickly.
  Improves Performance: Makes websites and apps work faster.
  Global Reach: Shares content with users all over the world.
  Security: Protects data with HTTPS, AWS Shield, and WAF.
  Scalability: Handles high traffic efficiently.
  Cost-effective: Reduces data transfer costs.

# What are the key differences between S3 and CloudFront?
"Amazon S3 and CloudFront serve different purposes. S3 is mainly used to store data like files, images, or videos, while CloudFront is a content delivery network that delivers these files faster by caching them at edge locations around the world.

S3 is centralized in specific AWS regions, but CloudFront distributes content globally, reducing latency. S3 is focused on storage, and you pay for storing and accessing data, while CloudFront focuses on fast delivery, and you pay for data transfer and caching. Together, they work well for storing and quickly delivering content to users."

# What is an AWS region, and why is it important in your project?
 AWS region is a geographic area where AWS has data centers. Each region has a collections of multiple Availability Zones for high availability and fault tolerance.
   ## Importance in a Project:
   Low Latency: Choosing a region close to your users improves performance.
   Data Residency: Ensures compliance with data storage laws (e.g., GDPR)
   High Availability: Regions with multiple zones ensure better reliability.
   Cost: Some regions have lower pricing.
   Service Availability: Not all AWS services are available in every region.
  
