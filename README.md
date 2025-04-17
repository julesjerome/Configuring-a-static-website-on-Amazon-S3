# Configuring-a-static-website-on-Amazon-S3
Configure a static website on Amazon S3 by creating a bucket, uploading your HTML/CSS files, enabling static website hosting, and setting permissions to make the content publicly accessible. Optionally, connect it to a custom domain using Route 53 and CloudFront.

### **Prerequisites**
AWS account
Source
https://docs.aws.amazon.com/AmazonS3/latest/userguide/HostingWebsiteOnS3Setup.html#step7-test-web-site

### **Step 1: Create a bucket**
1. Sign in to the AWS Management Console and open the Amazon S3 console.
2. Choose Create bucket.
![alt text](image1.PNG)
3. Enter the name you want to use for your bucket.
![alt text](image2.PNG)
4. Choose a Region that is geographically close to you to minimize latency and costs, or to address regulatory requirements. The Region that you choose determines your Amazon S3 website endpoint.
5. Choose Create.
![alt text](image3.PNG)
6. Bucket is created.
![alt text](image4.PNG)

### **Step 2: Enable static website hosting**
1. In the buckets list, choose the name of the bucket that you just created.
2. Under Static website hosting, choose Edit.
![alt text](image5.PNG)
3. Choose Use this bucket to host a website.
4. Under Static website hosting, choose Enable.
5. In the Index document, enter the name typically index.html.
6. In the error document, enter the name 404.html.
![alt text](image6.PNG)
7. Choose Save changes.
8. Under Static website hosting, note the Endpoint.

### **Step 3: Edit Block Public Access settings**
Choose the name of the bucket that you have configured as a static website.
Choose Permissions.
