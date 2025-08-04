Serverless Static Website on AWS
This project demonstrates how to host a serverless static website using AWS S3, CloudFront (CDN + HTTPS), and Route 53 for a custom domain.


Features
🌐 Static website hosted entirely on AWS S3

⚡ CloudFront CDN for global low-latency delivery

🔒 HTTPS enabled using AWS Certificate Manager

🏷 Custom domain managed via Route 53

💰 Fully serverless & cost-efficient hosting

Architecture
S3 – Hosts static files (HTML, CSS, JS)

CloudFront – Caches and distributes content globally

ACM – Provides SSL/TLS certificate for HTTPS

Route 53 – Manages custom domain DNS

markdown
Copy
Edit
Browser → CloudFront → S3 Bucket
           ↓
       Route 53 (DNS)
Live Demo
🌍 https://abdirahmanweb.net/ (Replace with your domain)

How to Reproduce
Create an S3 bucket and enable static website hosting

Upload your index.html (and any assets)

Deploy CloudFront distribution using the S3 website endpoint

Request an SSL certificate in us-east-1 (for CloudFront)

Add an Alias A record in Route 53 pointing to CloudFront

Wait for propagation → Your site is live with HTTPS

Tech Stack
AWS S3 – Static website hosting

AWS CloudFront – Content delivery network

AWS Certificate Manager – SSL/TLS

AWS Route 53 – DNS management

Portfolio Value
This project demonstrates:

Knowledge of AWS networking & DNS

Ability to set up serverless hosting

Using CloudFront for performance & security

Future Improvements
Add CI/CD for automatic deployment

Use Terraform for Infrastructure as Code (IaC)

Add a custom 404 page
