# What is a CloudFront distribution, and how is it created?
   "A CloudFront distribution is a way to deliver content globally by caching it at AWS edge locations. It helps reduce latency and improves website performance.

   To create a CloudFront distribution, I would:

     Log in to the AWS Console and go to the CloudFront service.
    Click Create Distribution and choose Web for standard content delivery.
    Set the origin, which could be an S3 bucket, an Elastic Load Balancer, or a custom server.
    Configure cache behaviors, set the viewer protocol policy (HTTP/HTTPS), and define other settings like TTL (Time to Live) and logging.
    If using a custom domain, I’d add it as an Alternate Domain Name and set up SSL with AWS Certificate Manager.
   After reviewing the settings, I would click Create Distribution, and CloudFront would deploy, providing a distribution domain (e.g., d1234.cloudfront.net).
    This setup helps in delivering content quickly to users around the world."

# What is Origin Access Control (OAC), and why is it used?
   
Origin Access Control (OAC) is a security feature in CloudFront that makes sure only CloudFront can access your content stored in an S3 bucket, not anyone on the internet directly.
   Why it’s used:
Secure Access: Stops public from accessing your S3 bucket directly.
Better Control: CloudFront delivers content while keeping your S3 bucket private.
   how it work :
When you enable OAC, CloudFront gets access to your S3 bucket through a special ID (OAI), acting as a trusted middleman. This lets CloudFront securely fetch content for users.

# How does CloudFront improve the performance of your website?
  CloudFront speeds up your website by storing content in servers around the world. It delivers the content from the nearest server, reducing load times and making your site faster.






