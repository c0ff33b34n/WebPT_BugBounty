S3 RECON TIPS:

# Method 1:

Use this google dorks for finding s3 bucket
site: s3.amazonaws.com <site.com>

# Method 2: Github Dorks

org:Target "bucket_name"

org:Target "aws_access_key"

org:Target "aws_secret_key"

org:Target "S3_BUCKET"

org:Target "S3_ACCESS_KEY_ID"

org:Target "S3_SECRET_ACCESS_KEY"

org:Target "S3_ENDPOINT"

org:Target "AWS_ACCESS_KEY_ID"

org:Target "list_aws_accounts"

# Method 3:

You can use many online tools which are available on GitHub to find S3 bucket of a website. I would like to list down a few of them:
1) Slurp
2) Bucket_finder
3) S3Scanner
4) Lazy S3
5) S3 Bucket Finder
Almost all tools are command-line tools, You have can clone them from GitHub.

# Method 4:

Use the Burp Suite and spider the target web application. Burp Spider can extract the Amazon bucket of the target web application.

# Method 5:

Right-click on any image of the target application and open image in new tab. If the image URL looks like this: http://xyz.s3.amazonaws.com/images/b1.gif
It means the target application is storing their data to the Amazon server and the bucket name is “xyz”. Anything before “.s3” in the URL is the bucket name of the target application.

# Method 6:

Sometimes you find Amazon bucket in Content-Security-Policy Response headers

# Method 7:

Online Websites: https://buckets.grayhatwarfare.com/
