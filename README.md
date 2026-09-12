# Hosting a Static Website with AWS S3
This documentation demonstrates how I practiced hosting a static website using **Amazon S3**. At the end of this setup, a static website is available publicly through an S3 endpoint.

# Step-By-Step Setup
1.	The first thing I did was to create an S3 Bucket on my AWS Console. Below are the steps i took to create the bucket;

•	Logged into my AWS Management Console

•	Searched for S3

•	Clicked on Create Bucket

•	Selected the Bucket type

•	Entered a unique bucket name

•	Selected a region

•	Disabled ** Block all public access** (This enabled the accessibility of the static website over the internet).

Named the bucket “boywonder”

![General Purpose Bucket](images/image1.png)

![Block Public access](images/image2.png)

2.	Uploading Website Files
I downloaded a Website template, extracted the files from the zipped folder and uploaded the files into my bucket.

![Downloads](images/image3.png)

![Objects](images/image4.png)

3.	Enabling Static Website Hosting
After uploading my objects in the bucket, I went ahead to enable static website hosting.
I scrolled down to Static website Hosting in the Properties Section. 
I enabled it and set: Index document index.html (HTML Document) and Error document error.html (optional)

![Enabling static website](images/image5.png)

4.	Added my Bucket policy in the permissions section to provide public accessibility to the objects in the bucket.[View Policy](StaticWebsite/Policy.txt)

![Bucket Policy](images/image6.png)

5.	Static website stored and hosted! Below is the index page opened on my edge browser directly from my console.
Endpoint URL for my website:[View Live Website](https://boywonder.s3.us-east-1.amazonaws.com/index.html)

![POP Design](images/image7.png)



