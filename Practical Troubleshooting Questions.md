# What steps would you take if your S3-hosted static website is not loading via CloudFront?
    If an S3-hosted static website isn't loading via CloudFront, I would:

       Check CloudFront Distribution: Ensure the distribution is deployed and active.
       Verify Origin Settings: Confirm the S3 bucket is set as the origin and is accessible by CloudFront (via OAC or OAI).
       Review DNS Settings: Check if the domain points to the correct CloudFront URL.
       Check S3 Bucket Permissions: Ensure the bucket policy allows CloudFront access.
       CloudFront Cache: Invalidate the cache to remove outdated content.
      Check Error Pages: Verify that CloudFront and S3 have proper error page configurations.

# How do you resolve a mismatch between S3 bucket policies and CloudFront permissions?
     Enable OAC: Allow only CloudFront to access the S3 bucket.
     Fix Bucket Policy: Update the policy to give CloudFront permission to access the bucket.
     Check CloudFront Settings: Make sure CloudFront is set up correctly with the S3 bucket.
    Test Access: Confirm that CloudFront can load files from the bucket without issues.

# What is the significance of the "index document" and "error document" in static website hosting?
    Index Document: The main page (e.g., index.html) that opens when someone visits your site.
    Error Document: A page (e.g., error.html) that shows if a page is missing or there’s an error.


# How would you update your website content in S3, and ensure CloudFront serves the latest version?
   Upload New Content: Replace or upload updated files to the S3 bucket.
   Invalidate CloudFront Cache: In CloudFront, create an invalidation request for the updated files or /* to refresh all content.
   Test: Check the website to confirm the new content is being served.

# If the website loads on your laptop but not on mobile, how would you approach debugging?
   Check Network Connection: Ensure the mobile has internet access.
   Clear Cache: Clear the browser cache on the mobile to avoid loading old data.
   Test on Another Browser: Try opening the site in a different browser on mobile.
   Responsive Design: Verify the site is mobile-friendly and adjusts properly for smaller screens.
   CORS and Permissions: Ensure there are no CORS issues or access restrictions affecting mobile requests.
   Logs and Errors: Check browser developer tools on mobile for error messages.

  
  
