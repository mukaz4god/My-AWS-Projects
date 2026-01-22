1️⃣ Create a Separate AWS Account (Free Tier)
Steps

Go to: https://aws.amazon.com/

Click Create an AWS Account

Use:

A new email (not personal work email)

Strong password (password manager recommended)

Select Personal Account (unless you have a registered company)

Enter payment details (required for Free Tier)

Complete phone verification

✅ Outcome:
A clean, isolated AWS environment for security learning and projects.

2️⃣ Secure the Root Account (CRITICAL)
Why?

Root has unlimited power. It should never be used for daily work.

Steps

Log in as Root user

Go to IAM → Security Credentials

Enable MFA on root

Choose Virtual MFA

Use Google Authenticator / Authy

Store:

Root email

MFA recovery codes

Password securely

🚫 Rule: Root account is now locked away.

✅ Outcome:
Root account protected against compromise.

3️⃣ Create an IAM Admin User (No Root Usage)
Steps

Go to IAM → Users → Create User

Username: admin-user

Select:

AWS Management Console access

Attach policy:

AdministratorAccess

Create user

Log out from root

Log in as admin-user

Enable MFA for this user as well

✅ Outcome:
All future AWS actions happen via IAM, not root.

4️⃣ Set AWS Budgets & Billing Alerts (VERY IMPORTANT)
Why?

Misconfigured resources can cost £££ overnight.

Steps

Go to Billing → Budgets

Create budget:

Type: Cost Budget

Monthly limit: $5 (Free Tier safety)

Add alerts:

50% threshold → email

80% threshold → email

100% threshold → email

Verify billing alerts are enabled in Billing Preferences

✅ Outcome:
You can prove cost governance knowledge.

5️⃣ Enable AWS CloudTrail (All Regions)
Why?

CloudTrail is your security black box:

Who did what?

When?

From where?

Steps

Go to CloudTrail

Create trail

Settings:

Apply to All Regions

Enable Management Events

Read + Write

Create new S3 bucket for logs

Enable log file validation

✅ Outcome:
Full audit trail for investigations & compliance.

6️⃣ Enable IAM Access Analyzer
Why?

Detects:

Publicly exposed resources

Over-permissive IAM policies

Steps

Go to IAM → Access Analyzer

Create analyzer

Scope: Account

✅ Outcome:
Proactive detection of risky access configurations.
