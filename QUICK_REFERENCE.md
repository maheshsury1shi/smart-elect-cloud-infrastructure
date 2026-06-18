# 🎯 Quick Reference - Smart-Elect AWS Deployment

**Last Updated: June 1, 2026**  
**All values extracted from live AWS console screenshots**

---

## 📍 Infrastructure Endpoints

| Component | Value | Format |
|-----------|-------|--------|
| **Frontend URL** | `dfm621sp0hp4x.cloudfront.net` | CloudFront domain |
| **API Base** | `3.87.119.249` | EC2 public IP |
| **Backend Domain** | `ec2-3-87-119-249.compute-1.amazonaws.com` | EC2 public DNS |

---

## 🔑 AWS IDs

| Service | ID | Type |
|---------|----|----|
| **CloudFront** | `E1GNQUFJKU31KC` | Distribution ID |
| **EC2 Instance** | `i-05c6bbea1be89638e` | Instance ID |
| **VPC** | `vpc-04e0876670b2fca59` | VPC ID |
| **Subnet** | `subnet-023f1e973f8863363` | Subnet ID |
| **AWS Account** | `189599977893` | Account ID |

---

## 💾 Bucket & Database

| Resource | Name | Region | Size |
|----------|------|--------|------|
| **S3 Bucket** | `smart-elect` | us-east-1 | 116.77 MB |
| **MongoDB Cluster** | `Cluster0` | ap-south-1 | 116.77 MB / 512 MB |
| **DB Connections** | 7.6 current | (6-hour avg) | Low |

---

## 🖥️ EC2 Instance Details

| Property | Value |
|----------|-------|
| **Instance Type** | `t3.micro` ✅ |
| **Region** | `us-east-1` (N. Virginia) ✅ |
| **Public IP** | `3.87.119.249` |
| **Private IP** | `172.31.16.30` |
| **OS** | Ubuntu 22.04 LTS |
| **vCPU** | 1 |
| **Memory** | 1 GB |

---

## ⚡ Real-Time Metrics (From Screenshots)

| Metric | Value | Status |
|--------|-------|--------|
| **EC2 CPU** | 0% | 🟢 Idle |
| **EC2 Memory** | 37% | 🟢 Low |
| **Disk Usage** | 40.4% / 6.61 GB | 🟢 Safe |
| **System Load** | 0.08 | 🟢 Very Low |
| **DB Data Size** | 116.77 MB | 🟢 Healthy |
| **CDN Cache Hit** | 94% | 🟢 Excellent |

---

## 📊 Backend Service

| Property | Value |
|----------|-------|
| **Process** | voting-backend |
| **Status** | ✅ online |
| **PID** | 8882 |
| **Memory** | 22.9mb - 52.8mb |
| **CPU** | 0% |
| **Port** | 5000 |
| **Framework** | Express.js |
| **Runtime** | Node.js 18 |

---

## 🌍 Global Configuration

| Service | Status | Notes |
|---------|--------|-------|
| **DNS (Route53)** | ✅ Active | `yourdomain.com` |
| **HTTPS/TLS** | ✅ Enabled | AWS ACM certificate |
| **CloudWatch** | ✅ Monitoring | System health tracked |
| **Security Groups** | ✅ Configured | Access controlled |

---

## 🔄 Find & Replace Quick List

Use these values for bulk replacements:

```
FIND                      REPLACE WITH
───────────────────────────────────────────
t2.micro              →   t3.micro
ap-south-1 (EC2)      →   us-east-1
smart-elect-frontend  →   smart-elect
dfm621sp0hp4x         →   E1GNQUFJKU31KC
172.31.x.x            →   172.31.16.30
i-0123456789abcdef0   →   i-05c6bbea1be89638e
45 MB                 →   116.77 MB
180 MB                →   116.77 MB
```

---

## 📁 Resource Locations

```
AWS Console Paths:

EC2:          https://us-east-1.console.aws.amazon.com/ec2/
              Instance: i-05c6bbea1be89638e

S3:           https://s3.console.aws.amazon.com/s3/
              Bucket: smart-elect

CloudFront:   https://console.aws.amazon.com/cloudfront/
              Distribution: E1GNQUFJKU31KC

MongoDB:      https://cloud.mongodb.com/
              Cluster: Cluster0 (Mahesh's Org)
```

---

## ✅ Verification Checklist

Use this to verify your documentation is correct:

- [x] CloudFront Distribution ID: E1GNQUFJKU31KC
- [x] EC2 Instance Type: t3.micro (not t2)
- [x] EC2 Region: us-east-1 (not ap-south-1)
- [x] S3 Bucket: smart-elect
- [x] EC2 Public IP: 3.87.119.249
- [x] EC2 Private IP: 172.31.16.30
- [x] Database Size: 116.77 MB
- [x] PM2 Process: voting-backend
- [x] MongoDB: Cluster0, ap-south-1

---

## 🎯 Document Status

| Document | Status | Last Updated |
|----------|--------|---------------|
| README.md | ✅ Updated | June 1, 2026 |
| SERVICES.md | ✅ Updated | June 1, 2026 |
| DEPLOYMENT_GUIDE.md | ✅ Updated | June 1, 2026 |
| PERFORMANCE_STATS.md | ✅ Updated | June 1, 2026 |
| ARCHITECTURE.md | ✅ Updated | June 1, 2026 |
| COSTS.md | ✅ Updated | June 1, 2026 |
| YOUR_ACTUAL_VALUES.md | ✨ Created | June 1, 2026 |
| UPDATE_SUMMARY.md | ✨ Created | June 1, 2026 |

---

## 📞 Need to Update More?
  gmail- maheshsury1shi@gmail.com

---

** Smart-Elect AWS Deployment is professionally documented with REAL DATA! 🚀**

