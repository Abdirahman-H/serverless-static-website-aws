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
S3: Create bucket & enable static website hosting

Upload files: Add index.html and assets

CloudFront: Create distribution using S3 website endpoint

SSL: Request certificate in us-east-1 (ACM)

Route 53: Create Alias A record pointing to CloudFront

Go Live: Wait for propagation → enjoy your secure website!

🛠 Tech Stack
Amazon S3 – Static file hosting

CloudFront – Global CDN + HTTPS

AWS Certificate Manager – SSL/TLS

Route 53 – DNS Management

📌 Future Enhancements
🔄 Add CI/CD pipeline for auto-deploy

⚙️ Manage infrastructure with Terraform (IaC)

📄 Add custom 404 page