# aws-s3-static-website-hosting
hosted a static website on aws wih bucket policies and public access configuration
this is the S3 policies that i use
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "PublicReadGetObject",
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::emmanuel-ec2-project-2026/*"
        }
    ]
}

USER BROWSER
- S3 static wedsite endpoint
- Bucket policy allows public read access
- index.html served

SETUP STEPS
1) created S3 bucket
2) uploaded index.html
3) enabled static website hosting
4) configured bucket policy
5) adjusted block public access settings
6) tested website endpoint

TROBOLESHOOTING SECTION
* PROBLEM
- received 403 forbidden error when opening S3 website endpoint.
* INVESTIGATION
- reviewed bucket policy and public access settings.
* CAUSE
- public access was blocked and bucket policy was incomplete.
* FIX
- Disabled block public Access appropriately and added correct bucket policy for public object access.

SKILLS USED
- AWS
- static website hosting
- bucket policies
- IAM concepts
- Troubleshooting
- HTTP access
