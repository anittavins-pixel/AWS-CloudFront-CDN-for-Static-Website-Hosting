# AWS-CloudFront-CDN-for-Static-Website-Hosting
This project demonstrates the implementation of a secure, scalable, Content Delivery Network (CDN) using Amazon CloudFront and Amazon S3 for hosting a static website.  The architecture leverages CloudFront Origin Access Control (OAC) to keep the S3 bucket private while enabling secure content delivery through CloudFront edge locations, 
🚀 Features
Static website hosting on Amazon S3
Global content delivery using Amazon CloudFront
Origin Access Control (OAC) for secure S3 access
HTTPS content delivery
Automatic caching through CloudFront edge locations
Reduced latency and improved website performance
Secure architecture with a private S3 origin
CloudFront cache invalidation support
🛠️ AWS Services Used
Service	PurposeAmazon S3	Store website files
Amazon CloudFront	Content Delivery Network (CDN)
Origin Access Control (OAC)	Secure CloudFront access to S3
IAM Policies	Access control and permissions
AWS Edge Locations	Global content caching
📋 Implementation Steps
Step 1: Create an S3 Bucket
Create a new Amazon S3 bucket.
Upload website content:
index.html
CSS files
JavaScript files
Images
Step 2: Keep the Bucket Private
Enable Block Public Access.
Remove public read permissions.
Use CloudFront as the only access layer.
Step 3: Create a CloudFront Distribution
Origin Type: Amazon S3
Select the S3 bucket as the origin
Enable Origin Access Control (OAC)
Use recommended cache settings
Step 4: Configure Security
Redirect HTTP to HTTPS
Enable secure content delivery
Configure CloudFront to access S3 using OAC
Step 5: Update S3 Bucket Policy

Grant CloudFront access to the bucket while keeping it private.

Step 6: Configure Default Root Object
Plain Text
1
index.html
Show more lines
Step 7: Deploy and Validate
Wait for distribution deployment.
Access the CloudFront domain.
Verify website functionality.
🔐 Security Implementation
Before
Plain Text
1
Internet Users
2
│
3
▼
4
Public S3 Bucket
Show more lines
After
Plain Text
1
Internet Users
2
│
3
▼
4
CloudFront
5
│
6
▼
7
Private S3 Bucket
Show more lines
Benefits

✅ No direct access to S3 files

✅ Secure origin access using OAC

✅ HTTPS enforced

✅ Reduced attack surface

✅ Improved content protection

📈 Performance Benefits
Faster page load times
Lower latency
Global content caching
Improved user experience
Reduced requests to the origin bucket
Automatic content distribution across AWS Edge Locations
🎯 Skills Demonstrated
AWS CloudFront
Amazon S3
CDN Implementation
HTTPS Configuration
Origin Access Control (OAC)
Cloud Architecture
Static Website Hosting
AWS Security Best Practices
DNS and Content Delivery Concepts
📸 Project Outcome

Successfully implemented a globally distributed CDN architecture that delivers static website content securely and efficiently through Amazon CloudFront while maintaining a private Amazon S3 origin.

📚 Learning Highlights
Understanding CloudFront caching mechanisms
Configuring Origin Access Control (OAC)
Managing S3 bucket policies
Securing static website hosting
Implementing AWS CDN best practices
🔖 Tags
Plain Text
1
AWS • Amazon S3 • CloudFront • CDN • Cloud Computing • DevOps • Cloud Architecture • Static Website Hosting • Security • OAC

⭐ If you found this project useful, feel free to star the repository and connect with me on LinkedIn! 🚀
