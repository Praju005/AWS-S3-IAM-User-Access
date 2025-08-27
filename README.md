# 🌐 AWS S3 Cross-Account Access Project

## 📖 Description
This project demonstrates how to set up **cross-account access** in **Amazon S3** using **IAM Users** and **Bucket Policies**.  
Bucket `my-projectt01` was created, a user `DemoUser` was granted full S3 access, and another bucket `my-projectt-02` was created using the IAM user credentials.

---

## 🏗 Architecture Diagram
```
   +-------------------+         +--------------------+
   |  Main AWS Account |         |  IAM User (DemoUser)|
   |  S3: my-projectt01| <-----> | S3: my-projectt-02  |
   +-------------------+         +--------------------+
                |                          |
                +-----------> Policy <------+
```
(*Replace with real architecture diagram screenshot*)

---

## 🛠 Prerequisites
- AWS Account
- S3 Service Enabled
- IAM Permissions to create Users & Buckets

---

## 🚀 Step-by-Step Process

1. **Create an S3 Bucket**  
   - Name: `my-projectt01`
   - Region: Select your preferred region

2. **Create IAM User**  
   - Username: `DemoUser`
   - Assign: **Programmatic & Console Access**
   - Attach Policy: `AmazonS3FullAccess`

3. **Add Bucket Policy**  
   Paste the bucket policy in S3 → Permissions → Bucket Policy section.

4. **Login as IAM User**  
   - Use IAM user link from `Security Credentials`
   - Create a new bucket: `my-projectt-02`

---

## 🧪 Testing the Setup
- Login as `DemoUser`
- Try uploading/downloading objects from both buckets.
- Verify cross-account permissions work correctly.

---

## 📂 Project Structure
```
AWS-S3-CrossAccount/
│-- screenshots/
│   └-- step1.png
│   └-- step2.png
│-- README.md
```

---

## 👩‍💻 Author
**Prajakta Pandaram**  
Cloud Enthusiast ☁️ | AWS Projects | DevOps Learner  

---

