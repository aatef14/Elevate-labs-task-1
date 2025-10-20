# 🧠 ELEVATE LABS - TASK #1

---

## 🔷 Name
**Mohammed Aatef**

## 📧 Email
[moatif1416@gmail.com](mailto:moatif1416@gmail.com)

---

## 🧰 Objective
To create an **S3 bucket** in AWS and understand how **object storage** works.

---

## 🪣 Step-by-Step Procedure

### Step 1: Create S3 Bucket
1. Login to AWS Console.  
2. Search for **S3** and click **Create Bucket**.  
3. Enter unique bucket name → e.g. `elevate-labs-task-1`.  
4. Disable **Block all public access**.  
5. Accept acknowledgement → Click **Create bucket**.

---

### Step 2: Upload File
- Open bucket → Click **Upload**.  
- Select your local file → e.g. `kk-test.jpg`.  
- Click **Upload** → Done ✅

---

### Step 3: Access File via URL
Example object URL:

https://elevate-labs-task-1.s3.us-east-1.amazonaws.com/kk-test.jpg


If access denied → add a bucket policy 👇

---

### Step 4: Add Bucket Policy
```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::elevate-labs-task-1/*"
    }
  ]
}
