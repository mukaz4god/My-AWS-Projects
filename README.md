# My-AWS-Projects

# AWS Account & Security Baseline – Day 1 Project

## Scenario
KFJ Solutions Ltd is a fintech startup migrating to AWS without an existing cloud security baseline.
The goal of this project is to secure the AWS account from day one using AWS best practices.

## Objectives
- Protect root account
- Enforce IAM best practices
- Enable cost governance
- Enable logging and visibility
- Document decisions for audits

## Security Controls Implemented
- Root MFA
- IAM Admin User (no root usage)
- AWS Budgets & Alerts
- CloudTrail (For Regions)
- IAM Access Analyzer

## Outcome
I demonstrated creat an AWS account with security baseline with AWS account security fundamentals which aligned with:
- AWS Well-Architected Framework (Security Pillar)
- CIS AWS Foundations Benchmark

## IAM Deep Dive (IAM Least Privilege & Access Control Failure) – Day 2 Project#

## Scenario
A company runs a backend service on EC2 that uploads logs to S3.
During a routine security review, the security team suspects that IAM permissions are overly permissive and could allow unintended access to sensitive S3 buckets.

## Objectives 
- Review IAM access
- Demonstrate the risk
- Apply least privilege
- Validate the fix

## Outcome
I built a real AWS environment where I demonstrated the security impact of over-permissive IAM roles on EC2, then remediated it using least-privilege policies and validated the fix with controlled testing.
