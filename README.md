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
