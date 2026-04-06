# 🛡️ Microsoft Defender for Cloud (AZ-900)

## 🧠 Overview
- **Microsoft Defender for Cloud** = security posture management + threat protection service
- Monitors:
  - Azure
  - On-premises
  - Hybrid
  - Multicloud (AWS, GCP)

👉 Goals:
- Improve security posture
- Detect and respond to threats

---

## 🌐 Coverage

### Azure-native
- Built into Azure
- No additional deployment required for many services

---

### Hybrid & Multicloud
- Supports:
  - On-premises resources (via Azure Arc)
  - AWS & GCP environments
- Provides **single control plane** for security

---

## 🔐 Core Capabilities

### 1️⃣ Continuously Assess
- Evaluate security posture continuously
- Identify vulnerabilities in:
  - Virtual machines
  - Containers
  - Databases

👉 Integration:
- Microsoft Defender for Endpoint
- Vulnerability management tools

---

### 2️⃣ Secure
- Harden resources using best practices
- Based on:
  - **Microsoft Cloud Security Benchmark (MCSB)**

Features:
- Security recommendations
- Azure Policy integration
- Secure Score:
  - Measures overall security posture
  - Helps prioritize improvements

---

### 3️⃣ Defend
- Detect and respond to threats

#### 🚨 Security Alerts
- Provide:
  - Affected resources
  - Attack details
  - Remediation steps
- Can trigger automation (Logic Apps)
- Uses **kill-chain analysis**:
  - Correlates related alerts into full attack story

---

## 🛠️ Protection Areas

### ☁️ PaaS Services
- App Service
- Azure SQL
- Azure Storage

---

### 💾 Data Services
- Security assessments for:
  - SQL
  - Storage

---

### 🌐 Network
- Reduce attack surface:
  - Just-in-Time VM access
  - Port restrictions

---

### 💻 Compute
- Protect:
  - Virtual machines
  - Servers (including hybrid)

---

### 📦 Containers
- Protect Kubernetes clusters (Azure & AWS EKS)

---

## 🔄 Hybrid Protection

- Protect on-prem servers using:
  - Azure Arc
- Prioritize alerts across environments

---

## 🌍 Multicloud Protection

- AWS:
  - CSPM recommendations
  - Protect EC2, EKS
- GCP:
  - Security posture visibility

---

## ⚙️ Key Features

- Centralized security management
- Vulnerability assessment
- Threat detection
- Policy enforcement (via Azure Policy)
- Secure Score tracking

---

## 🎯 Key Concepts (Exam Focus)

- Defender for Cloud = **CSPM + Threat Protection**
- Works across:
  - Azure
  - Hybrid
  - Multicloud
- Three pillars:
  - Assess
  - Secure
  - Defend
- Uses:
  - Azure Policy
  - Secure Score
- Detects threats and provides remediation guidance

---

## 🧠 Quick Memory Aid

👉 **"Assess → Secure → Defend"**
---
### Navigation
- [Parent: Module Overview](README.md)
- [Previous: 🔐 Encryption and Key Management in Azure (AZ-900)](80_azure_encryption_and_key_management.md)
- [Next: ⚡ AZ-900 Last-Minute Cheat Sheet (1-Minute Review)](cheat_sheet_last_minute.md)
- [Home](../README.md)

