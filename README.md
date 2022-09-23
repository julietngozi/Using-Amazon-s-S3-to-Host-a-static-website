Using Amazon’s Unlimited Simple Storage Service (S3) To Host A Static Website Where Individual Web Pages Include Static Content. Also Using This Service To Store Developer Codes Before Hosting Them On Virtual Servers (EC2) For Dynamic Web Apps.

WHAT IS SIMPLE STORAGE SERVICE (S3)
It is an Amazon service that helps you to store unlimited data in the cloud. 

BENEFITS

	It is secure
	You only pay for what you use.
	Scalable 
	Great performance

Let’s say you have a website. Static website is one that is not dynamic in nature, it is a website that in informational. You have users with different account e.g a blog post or article.

TIPS 

	Create a bucket

	Enable static website hosting

	Edit block public access settings

	Add a bucket policy that make your bucket content publicly available 

	Configure an error document

	Test your website endpoint

	Clean up

In AWS you can use S3 to host a static website.

	The developers writes a code and put it in a folder, and you as a cloud engineer you need to make sure that user see it or available. You need to grab the folder and put it in S3.

	To make sure that the website is highly available, there is a website that all developers store their codes.

	Download the code

	Open your drive and it will show S3 dynamic and static

	Click static, when you right click you will see download and click on it.

	Crate a folder on your desktop and call it AWS Lab files then put the file in that folder.

	Then go to your download folder and download

	Create a folder in your desktop and call it source code, then paste that folder that you have. Note you need to extract it.

	Then open next.

	These are the source code.


THEN FELLOW THESE STEPS

Step 1 go to Amazon website console

Step 2 click on S3

Step 3 Click on create bucket

Step 4 name: S3 Static website

Step 5 N’ Virginia

•	Since you want it to be readable by public then uncheck Block Public.

•	Under default encryption (choose enable)

Step 6 click on create

Note: Bucket is a folder here you have subfolder and files and 2 persons in the world cannot have the same bucket name.

Step 7 click on your bucket name

![step 7](https://user-images.githubusercontent.com/104633983/191887144-8f948641-a04f-48be-b711-0ef8ea2d907c.PNG)

Step 8 click upload

•	Then open the folder from your file and drag them and put them in your folder

Step 9 click upload 

Step 10 click on exit after successful

It display the following:

•	Access
•	Css
•	Js
•	Index

Step 11 click on properties

Step 12 click on edit

Step 13 click on enable static

•	Under index document: type index.html

•	If there is error you type but if not leave it.

Step 14 click on save changes

•	Click on the link under static website and copy it, open it in a new tab

•	It will show error message i.e 404 forbidden

![error 404](https://user-images.githubusercontent.com/104633983/191887631-87d0a1a4-7f90-42f8-a199-41f849a00f03.PNG)

Step 15 click on permission 

•	In access control link click on edit

Step 16 copy the code 

•	Edit bucket policy

•	Under policy permission paste the code 

•	Copy the name of your bucket and put it in the Json log 

Step 17 click on save.

•	It will bring out your static website

![service](https://user-images.githubusercontent.com/104633983/191889110-2895d210-f407-4517-a744-cb9747cbccdd.PNG)


Using this service to store developer codes before hosting them on virtual servers (EC2) for dynamic web apps.

1.	Create S3 Bucket 
2.	
3.	Upload web files to S3 bucket
4.	 
5.	Create IAM Role
6.	
7.	Create an EC2 instance
8.	
9.	SSH with MobaXterm 
10.	
11.	Install a LMP web server on Amazon Linux2 
12.	
Step 1 : Create S3 Bucket 

You will need to create an S3 bucket to put your website’s files and folders.

![step 1](https://user-images.githubusercontent.com/104633983/191889593-3069ba12-13c3-4acc-9d15-5e6982555b4a.PNG)

Under Block Public Access settings for this bucket section, check the Block all public access checkbox. This is done to make the bucket not accessible to the public. 

Click on Disable for Bucket Versioning. 

Under Default encryption section, click on Enable for Server-side encryption. Then check Amazon S3 Key (SSE-S3). 

Then click on Create bucket. 

Step 2 : Upload web files to S3 bucket 

After creating the bucket, you need to upload your website’s files and folders into it. 

From the S3 dashboard, click on the name of the bucket you just created. 

On the Objects tab, you can see that the bucket is currently empty, click on the Upload button. 

![vi](https://user-images.githubusercontent.com/104633983/191890205-8e213cbb-c19f-4464-83f7-6a2cb59508ef.PNG)

This should take you to the Upload page. Drag and Drop the website files that was downloaded from this . 



Step 3 : Create IAM Role 

Now, EC2 want to pull code from S3. So you want to create IAM Role to give EC2 permission to access S3. 

To do this, from the Services drop-down, select IAM from the Security, Identity& Compliance section. From the IAM dashboard, click on Roles. 

Then Click on Create role. 

![role](https://user-images.githubusercontent.com/104633983/191890620-1bad4b35-2d19-4f32-8339-96c47113508e.PNG)

Step 4 : Create an EC2 instance 

To do this, from the Services drop-down, select EC2 from the Compute section. This should display the EC2 dashboard. From the EC2 dashboard, click on Launch instance. 

Under configure instance details

![t](https://user-images.githubusercontent.com/104633983/191968610-aabd2f80-1f10-4879-b280-7f7e687d3e62.PNG)

Click Next

You can add tag Name: DynamicSite. Then click on Next: Configure Security Group. 

Select Create a new security group. Give it Name: DynamicWebsite3 and description:   DynamicWebApp1. For SSH rule select My IP for Source. 

Click on Add Rule and select HTTP for Type and Anywhere for Source. Last rule select HTTPS for Type and Anywhere for Source.

Click on Review and Launch. 



