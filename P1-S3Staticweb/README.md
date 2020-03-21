# Cloud Fundamentals Project

The cloud is perfect for hosting static websites that only include HTML, CSS, and JavaScript files that require no server-side processing. In this project, you will deploy a static website to AWS. First, you will create a S3 bucket and upload the website files to your bucket. Next, you will configure the bucket for website hosting and secure it using IAM policies. Next, you will speed up content delivery using AWS’ content distribution network service, CloudFront. Lastly, you will access your website in a browser using the unique CloudFront endpoint.

## Prerequisites:

- AWS Account
- Student-ready starter code: https://drive.google.com/open?id=15vQ7-utH7wBJzdAX3eDmO9ls35J5_sEQ

## Topics Covered:

- S3 bucket creation
- S3 bucket configuration
- Website distribution via CloudFront
- Access website via web browser



1. Create S3 Bucket
2. Upload Files to S3 Bucket
3. Secure Bucket with IAM Bucket Policy

```json
{
  "Version":"2012-10-17",
  "Statement":[
    {
      "Sid":"AddPerm",
      "Effect":"Allow",
      "Principal": "*",
      "Action":["s3:GetObject"],
      "Resource":["arn:aws:s3:::your-website/*"]
    }
  ]
}
```

4. Turn on Static Website Hosting

5. Use CloudFront to distribute website content by CDN.

   

[Rubric](https://review.udacity.com/#!/rubrics/2573/view)