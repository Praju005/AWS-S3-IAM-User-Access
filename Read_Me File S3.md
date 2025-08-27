# AWS S3 IAM User Access Project

## Project Description
This project demonstrates how to create an **IAM user** within the same AWS account and give them permissions to manage Amazon S3 buckets.  
The user can log in separately, create new buckets, and manage S3 resources independently.

---

## Steps Followed

### 1. Create S3 Bucket in Main Account
- **Bucket Name:** `my-projectt01`
- In the main AWS account, go to **S3 → Create Bucket** → Enter bucket name → Leave defaults → Create.

---

### 2. Create IAM User
- **User Name:** `DemoUser`
- Set **Access Type:** AWS Management Console Access.
- Created a password for the user during setup.
- Attached **AdministratorAccess** policy (for testing full access).

---

### 3. Get IAM User Login Link
- After creating the user, copied the **IAM Sign-in link** from the console.
- Used this link in **Incognito Mode** to log in as `DemoUser`.

---

### 4. Create New Bucket as DemoUser
- Logged in as `DemoUser`.
- Created a new bucket: **my-projectt-02**.
- Verified it appears in the main account because it's in the same AWS account.

---

## Output
- IAM user (`DemoUser`) successfully created a new S3 bucket in the same account.
- Both the main account and `DemoUser` have full access to all created buckets.

---

## Author
Prajakta Pandaram
