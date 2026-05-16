

# Task 1 : Cloud-Storage-Setup

AWS S3 Cloud Storage Setup Internship Task. This project demonstrates the creation, configuration, and secure management of a cloud storage bucket using Amazon S3 on AWS Free Tier.

---


# TASK DESCRIPTION

This project demonstrates the setup and configuration of cloud storage using Amazon Web Services (AWS) S3. The task includes creating an S3 bucket, uploading files, configuring permissions, and testing public accessibility of uploaded objects.

Amazon S3 (Simple Storage Service) is a scalable object storage service used for backup, hosting static files, and storing application data securely in the cloud.

---


## Step 1: Create an S3 Bucket

1. Login to AWS Console
2. Navigate to Amazon S3
3. Click Create bucket
4. Configure:

   * Bucket Name: **test-storage-komal**
   * Region: **ap-south-1 (Mumbai)**
   * Block Public Access: ✅ Enabled
5. Click Create bucket

![Bucket](./Images/B1.png)
![Bucket](./Images/b2.png)
![Bucket](./Images/b3.png)
---

## Step 2: Create Folder Structure

Inside the bucket, create the following folders:

* test-documents/
* test-images/
* test-log/

This ensures organized storage.

![Folder Structure](./Images/fu1.png)

---

## Step 3: Upload Example Files

Uploaded files:

* test-documents → **test.txt**
* test-images → **test.jpeg**
* test-log → **battery-report.html**

![Documents](./Images/fu2.png)
![Images](./Images/fu3.png)
![Logs](./Images/fu4.png)

---

## Step 4: Configure Access Permissions

* Block Public Access: ✅ Enabled
* Object Ownership: Bucket owner enforced
* Access controlled using bucket policies & IAM

![Permissions](./Images/pub.png)

---

## Step 5: Enable Default Encryption

* Enabled Server-Side Encryption (SSE-S3)
* Ensures data is encrypted at rest

![Encryption](./Images/encryp.png)

---

## Step 6: Enable Bucket Versioning

* Versioning: ✅ Enabled
* Helps recover deleted/overwritten files

![Versioning](./Images/ver.png)

---

## Step 7: Verify Private Access

1. Copied Object URL
2. Opened in Incognito
3. Result: Access Denied

### test-documents

![Denied](Images/t1.png)

### test-images

![Denied](Images/t2.png)

### test-log

![Denied](./Images/t3.png)

---

## Conclusion

An Amazon S3 bucket was successfully created and configured with secure access controls. Files were uploaded, encryption and versioning were enabled, and access restrictions were verified through AccessDenied responses.

This demonstrates a secure and scalable cloud storage implementation using AWS.

