# If the website is slow to load in a specific region, how can CloudFront help?
CloudFront helps by delivering content from the nearest server, reducing delays. It also caches content locally and uses fast routes to ensure quick and reliable delivery

# How would you restrict access to your website to specific IPs or countries?
  "To restrict access to a website based on IP or country, I would use AWS CloudFront with AWS WAF.

For IP restrictions, I can create a rule in AWS WAF that allows or blocks specific IP addresses.
For country restrictions, I can use AWS WAF’s GeoMatch feature to allow or block access based on the user's country. Once the rules are set, I would associate the Web ACL (Access Control List) with the CloudFront distribution to enforce these restrictions."
