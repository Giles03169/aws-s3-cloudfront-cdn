# 📦 CloudFront CDN Deployment — Step-by-Step

## 1. S3 Bucket (from previous project)
- Bucket: `my-static-site-giles`
- Hosting enabled with `index.html` + `error.html`

## 2. Create CloudFront Distribution
- Origin: your S3 static website endpoint
- Origin access: Public
- Viewer protocol policy: Redirect HTTP to HTTPS
- Default root object: `index.html`
- SSL: Default CloudFront certificate
- WAF: None

## 3. Wait for deployment (approx. 5–10 mins)

## 4. Test site at CloudFront domain
- Format: `https://davm4eq005r87.cloudfront.net/
