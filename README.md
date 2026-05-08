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
