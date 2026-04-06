# 🔐 Encryption and Key Management in Azure (AZ-900)

## 🧠 Overview
- **Encryption** = protects data confidentiality
- Makes data unreadable to unauthorized users
- Strong security requires:
  - Encryption at rest
  - Encryption in transit

---

## 🔒 Types of Encryption

### 1️⃣ Encryption at Rest
- Protects stored data
- Examples:
  - Databases (Azure SQL)
  - Disks (VMs)
  - Storage accounts

---

### 2️⃣ Encryption in Transit
- Protects data while moving
- Examples:
  - Between services
  - Between apps and users
  - API communication

---

## 🎯 Key Principle
👉 Use **both at rest + in transit** for full protection

---

## 🧪 Practical Example

- App stores customer data in:
  - Azure Storage
  - Azure SQL  

👉 Data should be encrypted:
- While stored (at rest)
- While transferred (in transit)

---

## 🔑 Azure Key Vault

- Central service for secure storage of:
  - Secrets (passwords, connection strings)
  - Encryption keys
  - Certificates (TLS/SSL)

---

## ⚙️ Why Use Key Vault?

### 🔐 Security
- Avoid hardcoding secrets in code/config
- Centralized secret management

---

### 🔄 Key Management Features

- Access control (who can use keys)
- Key rotation (update keys regularly)
- Auditing (track usage)

---

### 👥 Separation of Duties
- Different roles for:
  - Viewing keys
  - Using keys
  - Rotating keys

---

### 🔔 Best Practices
- Use key rotation policies
- Set alerts before key expiration
- Use **managed identities** to access secrets securely

---

## 🎯 Key Concepts (Exam Focus)

- Encryption protects **data confidentiality**
- Two types:
  - At rest
  - In transit
- **Azure Key Vault** = central service for:
  - Secrets
  - Keys
  - Certificates
- Avoid storing secrets in code
- Use:
  - Access control
  - Key rotation
  - Auditing

---

## 🧠 Quick Memory Aid

👉 **"Encrypt data everywhere, store keys securely."**