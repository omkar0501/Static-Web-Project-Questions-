# How do you configure a bucket for static website hosting?
  "To set up S3 for static website hosting, I first create a bucket and upload all the static files like index.html and style.css. Then, I enable static website hosting in the bucket’s properties and set the index.html as the starting file.
Next, I configure permissions to allow public access by adding a bucket policy that grants read access to the objects. Finally, I use the website endpoint provided by S3 to access the hosted site. This makes the static website live and accessible to users."

 # What is a bucket policy, and how did you use it in your project?
 A bucket policy is a JSON document that defines access permissions for an S3 bucket and its objects. It controls who can access the bucket and what actions they can perform (e.g., read, write).
   ## How I Used It in My Project:
   In my project, I used a bucket policy to make the bucket publicly accessible for static website hosting. The policy allowed anyone to read objects (e.g., HTML, CSS files) so the website could load in a browser.

# Can you explain what "Block Public Access" in S3 means?
  "Block Public Access" in S3 stops anyone from accessing your files without permission. It keeps your data private by blocking settings that would make your files public, unless you choose to allow it.

# How would you troubleshoot a 403 Forbidden error when accessing a static website?
  "If I encounter a 403 Forbidden error on a static website hosted on S3, I would take the following steps:

   Check Bucket Permissions: Ensure the S3 bucket allows public access to files, and verify the bucket policy allows s3:GetObject for everyone.
   Verify Block Public Access Settings: Confirm that the 'Block Public Access' setting is correctly configured, especially if public access is needed.
   Check Object Permissions: Ensure the specific file or object you're trying to access has the right permissions set to allow public access.
   Inspect CORS Settings: If the website uses resources from different domains, check that the CORS configuration on the bucket is correct.
   CloudFront Configuration: If using CloudFront, ensure the Origin Access Identity (OAC) is set up properly and CloudFront has access to the S3 bucket.
   Confirm Static Website Hosting Settings: Verify that Static Website Hosting is enabled on the bucket and that the correct index and error pages are set.
      By checking these configurations, I can identify the root cause of the error and fix it."








