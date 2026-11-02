# AWS-S3-Static-Website-Hosting-and-Lifecycle-Managemet
Project Overview

This project demonstrates how to host a static website using Amazon S3 and manage stored objects using S3 Lifecycle Policies.

Amazon S3 is used to host website files such as HTML, CSS, and JavaScript. S3 Lifecycle Management is used to automatically transition objects between storage classes based on configured rules.

AWS Services Used

- Amazon S3
- S3 Static Website Hosting
- S3 Lifecycle Management
- S3 Bucket Policy

Project Objectives

1. Host a static website using Amazon S3.
2. Upload website files into an S3 bucket.
3. Configure static website hosting.
4. Configure bucket permissions.
5. Create an S3 Lifecycle Policy.
6. Automate object storage transitions.

Project Implementation

Part 1: S3 Static Website Hosting

Step 1: Create an S3 Bucket

- Open AWS Management Console.
- Navigate to Amazon S3.
- Click Create bucket.
- Enter a unique bucket name.
- Select the AWS Region.
- Create the bucket.

Step 2: Create Website Files

Create the following files:

- index.html
- style.css
- script.js (optional)

Step 3: Enable Static Website Hosting

- Open the S3 bucket.
- Navigate to Properties.
- Find Static Website Hosting.
- Click Edit.
- Enable Static Website Hosting.
- Select Host a static website.
- Enter index.html as the index document.
- Save changes.

Step 4: Upload Website Files

- Open the Objects tab.
- Click Upload.
- Upload the HTML, CSS, and JavaScript files.

Step 5: Configure Bucket Policy

- Open the Permissions tab.
- Configure public access for this demo website.
- Add a bucket policy allowing public s3:GetObject access.

Step 6: Test the Website

- Open the Properties tab.
- Find Static Website Hosting.
- Open the website endpoint.
- Verify that the website loads successfully.

Part 2: S3 Lifecycle Policy Management

Step 1: Open S3 Bucket

- Open the S3 bucket.
- Navigate to the Management tab.

Step 2: Create Lifecycle Rule

- Click Create lifecycle rule.
- Enter rule name: S3-Lifecycle-Rule.
- Select the required object scope.

Step 3: Configure Lifecycle Actions

Example configuration:

Action| Days
Transition to Standard-IA| 30 days
Transition to Glacier Flexible Retrieval| 90 days
Expire objects| 365 days

Step 4: Save Lifecycle Rule

- Review the lifecycle configuration.
- Click Create rule.
- Verify the lifecycle rule.

Architecture

Static Website:

User → Web Browser → Amazon S3 → Website Files

Lifecycle Management:

File Upload → S3 Standard → Standard-IA → Glacier Flexible Retrieval → Expiration

Expected Results

- Successfully hosted a static website using Amazon S3.
- Uploaded and managed website files.
- Configured S3 bucket permissions.
- Created an S3 Lifecycle Policy.
- Automated object storage transitions and expiration.

Skills Learned

- Amazon S3 bucket management.
- Static website hosting.
- Bucket policies and permissions.
- S3 storage classes.
- Lifecycle rule configuration.
- AWS Console practical experience.

Conclusion

This project provided hands-on experience with Amazon S3 static website hosting and automated storage lifecycle management. It helped me understand website hosting, object storage, access permissions, and storage cost optimization in AWS.

Author

Arun K

GitHub: https://github.com/ArunK-BM
