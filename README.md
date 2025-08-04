🌐 Serverless Static Website on AWS



A serverless static website hosted entirely on AWS using:

S3 for static hosting

CloudFront for CDN + HTTPS

Route 53 for custom domain & DNS

Live Demo → https://abdirahmanweb.net/

✨ Features
🌐 Static website with global availability

⚡ CloudFront CDN for ultra-fast delivery

🔒 HTTPS using AWS Certificate Manager

🏷 Custom domain via Route 53

💰 Serverless & cost-efficient

🏗 Architecture
scss
Copy
Edit
Browser 🌍
   │
   ▼
CloudFront CDN ⚡
   │
   ▼
S3 Bucket (Static Hosting) 📂
   │
   ▼
Route 53 (DNS) 🏷
📖 Steps to Reproduce
1. S3: Create bucket & enable static website hosting

2. Upload files: Add index.html and assets

3. CloudFront: Create distribution using S3 website endpoint

4. SSL: Request certificate in us-east-1 (ACM)

5. Route 53: Create Alias A record pointing to CloudFront

6. Go Live: Wait for propagation → enjoy your secure website!

🛠 Tech Stack
Amazon S3 – Static file hosting

CloudFront – Global CDN + HTTPS

AWS Certificate Manager – SSL/TLS

Route 53 – DNS Management

📌 Future Enhancements
🔄 Add CI/CD pipeline for auto-deploy

⚙️ Manage infrastructure with Terraform (IaC)

📄 Add custom 404 page