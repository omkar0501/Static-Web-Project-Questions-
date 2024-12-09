# If the website is slow to load in a specific region, how can CloudFront help?
CloudFront helps by delivering content from the nearest server, reducing delays. It also caches content locally and uses fast routes to ensure quick and reliable delivery

# How would you restrict access to your website to specific IPs or countries?
  "To restrict access to a website based on IP or country, I would use AWS CloudFront with AWS WAF.

For IP restrictions, I can create a rule in AWS WAF that allows or blocks specific IP addresses.
For country restrictions, I can use AWS WAF’s GeoMatch feature to allow or block access based on the user's country. Once the rules are set, I would associate the Web ACL (Access Control List) with the CloudFront distribution to enforce these restrictions."

# Explain how you set up and tested secure access between CloudFront and S3.
 "I set up secure access between CloudFront and S3 by:

Configuring Origin Access Control (OAC) to allow CloudFront to access the S3 bucket securely.
Updating the S3 bucket policy to block direct public access.
Testing by accessing the website through CloudFront to ensure S3 content is served securely and not directly from the bucket."

# If you had to add SSL (HTTPS) to your website, how would you do it with CloudFront?
Obtain an SSL Certificate: Use AWS Certificate Manager (ACM) to request or import an SSL certificate.
Configure CloudFront: In CloudFront, associate the SSL certificate with your distribution.
Force HTTPS: Set up a redirect in CloudFront to ensure all traffic is redirected from HTTP to HTTPS.

#




