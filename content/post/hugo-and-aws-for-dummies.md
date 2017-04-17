+++
title       = "Hugo and AWS for Dummies"
description = "Steps necessary for deploying a Hugo static website to AWS"
date        = "2017-04-17"
draft       = true
+++

I guess I must be a dummy.  In my quest to move this website from Media Temple to AWS, I searched the Internet for relevant examples and tutorials.  While there was excellent information to be found, most of the articles were either outdated, overly complex, or a combination of the two.

Following is my personal workflow for setting up a Hugo website, deploying it to AWS, and configuring it all using a custom domain.

## Step 1: Configuring Hugo

 using S3, CloudFront, and Route53.


## Step 2: Configuring AWS

Set up a Bucket Policy.  I used the example policy from Amazon:

``` JSON
{
"Version": "2012-10-17",
"Statement":
    [{
    "Sid": "PublicReadGetObject",
    "Effect": "Allow",
    "Principal": "*",
    "Action": ["s3:GetObject"],
    "Resource": ["arn:aws:s3:::example-bucket/*"]
    }]
}
```

Replace "example-bucket" with your bucket name, which should be the same as your domain name, which in my case is elemdage.com.

## Step 3: Configuring Nameservers
