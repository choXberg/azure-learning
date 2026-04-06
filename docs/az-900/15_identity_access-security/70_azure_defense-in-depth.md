# 🛡️ Defense-in-Depth (AZ-900)

## 🧠 Overview
- **Defense-in-Depth** = layered security strategy
- Goal:
  - Protect data
  - Prevent unauthorized access
- Idea:
  - Multiple security layers instead of relying on one

👉 If one layer fails → others still protect the system

---

## 🎯 Key Concept
- Security is built in **layers around data**
- Data is the **core asset to protect**
- Each layer:
  - Slows attackers down
  - Provides detection opportunities

---

## 🧩 Layers of Defense-in-Depth

### 1️⃣ Physical Security
- Protect datacenters and hardware
- Prevent unauthorized physical access

---

### 2️⃣ Identity & Access
- Control who can access resources
- Key practices:
  - Single Sign-On (SSO)
  - Multifactor Authentication (MFA)
  - Logging and auditing

---

### 3️⃣ Perimeter
- Protect against external network attacks
- Key tools:
  - DDoS protection
  - Firewalls

---

### 4️⃣ Network
- Control communication between resources
- Key practices:
  - Deny by default
  - Limit inbound/outbound traffic
  - Network segmentation

---

### 5️⃣ Compute
- Secure virtual machines and devices
- Key practices:
  - Patch systems regularly
  - Use endpoint protection
  - Secure VM access

---

### 6️⃣ Application
- Secure application code and design
- Key practices:
  - Avoid vulnerabilities
  - Secure secrets (e.g., Azure Key Vault)
  - Security in development lifecycle

---

### 7️⃣ Data (Core Layer)
- Protect sensitive data
- Key practices:
  - Encryption at rest
  - Encryption in transit
  - Access control

👉 Most attacks target **data**

---

## 🔄 How It Works

- Layers are stacked around data
- Attack must pass through multiple defenses
- Each layer:
  - Reduces attack surface
  - Provides monitoring and alerts

---

## 🎯 Key Concepts (Exam Focus)

- Defense-in-Depth = **layered security model**
- No single point of failure
- Data is the **most critical asset**
- Security layers:
  - Physical → Identity → Perimeter → Network → Compute → Application → Data
- Use:
  - Encryption
  - Access control
  - Monitoring

---

## 🧠 Quick Memory Aid

👉 **"Layered security protects data at the core."**
---
### Navigation
- [Parent: Module Overview](README.md)
- [Previous: 🔐 Zero Trust Model (AZ-900)](60_azure_zero_trust_model.md)
- [Next: 🔐 Encryption and Key Management in Azure (AZ-900)](80_azure_encryption_and_key_management.md)
- [Home](../README.md)

