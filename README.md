#CloudComputing

**Company**: CODTECH IT SOLUTIONS

**Name**: BETHARAJU GANESH

**Intern ID**: CT04DZ2046

**Domain**: CLOUD COMPUTING

**Duration**: 4 Weeks

**Mentor**: NEELA SANTHOSH

## Task 4: Cloud Security Implementation

**Objective:** To implement fundamental security controls on a cloud platform by configuring Identity and Access Management (IAM) policies and enabling data encryption to protect cloud resources.

### 1. IAM Policy for Least Privilege

To ensure secure access to AWS resources, I implemented the **Principle of Least Privilege**. This was achieved by creating a new IAM user with a custom policy that strictly limits their permissions to only what is necessary.

#### Steps Taken:
1.  **Navigated to IAM:** I went to the Identity and Access Management (IAM) service in the AWS Console.
2.  **Created a New User:** I initiated the "Create user" process, providing a unique user name (`read-only-user`) and setting up AWS Management Console access with a secure password.
3.  **Crafted a Custom Policy:** I used the visual policy editor to create a new JSON policy. This policy explicitly allows only two specific read actions (`s3:GetObject` and `s3:ListBucket`) and restricts them to a single, predefined S3 bucket ARN. This prevents the user from deleting, modifying, or even viewing any other resource in the account.
4.  **Attached the Policy:** The newly created policy was attached directly to the user, ensuring the permissions were immediately effective upon the user's creation.

**Configured IAM User Permissions:**
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/bb0aae1a-1cb3-42d4-930a-c477f7f18ce8" />

### 2. Secure Storage with Data Encryption

To protect sensitive data at rest, I configured default server-side encryption for the primary storage bucket.

#### Steps Taken:
1.  **Navigated to S3 Bucket:** I located the specific S3 bucket created in Task 1.
2.  **Edited Bucket Properties:** I went to the "Properties" tab of the bucket settings.
3.  **Enabled Default Encryption:** I located the "Default encryption" section, enabled it, and selected the standard **"Amazon S3-managed keys (SSE-S3)"** option. This setting automatically encrypts every new object that is uploaded to the bucket, providing a crucial layer of data security without any manual effort.

**S3 Bucket Encryption Status:**
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/bb5120f0-eb12-4163-826c-a905b64d6228" />

---
