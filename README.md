# AWS S3 Security Lab

## Overview
This lab simulates real-world S3 security misconfigurations and demonstrates how to enforce encryption and recover from access lockout scenarios.

## What I Implemented
- Created an S3 bucket in ap-southeast-2
- Enabled server-side encryption using AWS KMS (SSE-KMS)
- Configured a bucket policy to deny unencrypted uploads
- Tested upload failures without encryption and success with SSE-KMS
- Implemented IP-based access control and tested using a mobile hotspot
- Accidently locked myself out of the bucket and used AWS Cloudshell to regain access
- Identified and resolved an access lockout caused by an overly restrictive bucket policy

## Tools Used
- Amazon S3
- AWS KMS
- IAM Policies
- AWS CloudShell

## Key Security Concepts
- Explicit Deny overrides all permissions
- Bucket policies can enforce encryption at upload
- Misconfigured policies can cause complete access lockout
- CloudShell can be used to recover access safely

## Screenshots
### Upload Success
Successful upload using SSE-KMS enforced bucket policy.
![Upload Success](CA480DFA-C321-4255-BE14-B8BF7830E14D.PNG)
### CloudShell Recovery
Recovered access after misconfigured bucket policy using AWS CloudShell.
![CloudShell Recovery](IMG_595F6AB8-2DEF-4E1C-B712-3C6CC6A7BF14.JPEG)
