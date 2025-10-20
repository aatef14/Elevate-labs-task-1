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

Download this for more precise steps

[View Task Document](ELEVATE-LABS-task-1.docx)


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

  ![Screenshot](![WhatsApp Image 2025-10-20 at 12 39 05_8962c44f](https://github.com/user-attachments/assets/d6e519bf-84c0-49f1-a007-74950e8aa984)
)


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

### Example of successful Access

 ![Screenshot](![WhatsApp Image 2025-10-20 at 13 00 27_e279d356](https://github.com/user-attachments/assets/1127c2f0-588f-492d-a99e-30e6233045e5)
)
