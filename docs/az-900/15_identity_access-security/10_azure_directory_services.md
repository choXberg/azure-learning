# 📘 Azure Directory Services (AZ-900)

## 🧠 Overview: Microsoft Entra ID
- Microsoft Entra ID = Cloud-based Identity & Access Management Service (IAM)
- Enables:
  - Login to Microsoft Cloud services (Azure, M365)
  - Access to custom applications
- Comparison to On-Prem:
  - Similar to Active Directory
  - Difference: Microsoft operates & scales infrastructure globally

---

## 👥 Who Uses Microsoft Entra ID?
- IT Administrators
  - Control access to resources & apps
- Developers
  - Implement authentication (e.g., SSO)
- Users
  - Self-Service (e.g., password reset)
- Cloud Customers
  - Automatically used for:
    - Azure
    - Microsoft 365
    - Dynamics

---

## ⚙️ Main Features

### 🔐 Authentication
- Identity verification before access
- Features:
  - Multi-Factor Authentication (MFA)
  - Self-Service Password Reset
  - Smart Lockout
  - Password policies

---

### 🔑 Single Sign-On (SSO)
- One login → Access to multiple applications
- Benefits:
  - User-friendly
  - Security

---

### 📦 Application Management
- Management of apps (cloud & on-prem)
- Examples:
  - SaaS integration
  - Application Proxy
  - "My Apps" portal

---

### 💻 Device Management
- Register & manage devices (e.g., via Intune)
- Conditional Access:
  - Access only from known/trusted devices

---

## 🔗 Connection with On-Prem Active Directory

### Problem:
- Without connection:
  - Two separate identities (cloud + on-prem)

### Solution:
- Microsoft Entra Connect
  - Synchronizes users between:
    - On-Prem AD
    - Microsoft Entra ID

### Benefits:
- Unified identity
- SSO across cloud & on-prem
- MFA & self-service available everywhere

---

## 🏢 Microsoft Entra Domain Services

### 📌 What is this?
- Provides classic AD functionality without own domain controllers

### Supports:
- Domain Join
- Group Policy
- LDAP
- Kerberos / NTLM

---

### 🎯 When to use?
- For legacy applications that:
  - Don't support modern auth
- "Lift & Shift" scenarios:
  - Migrate old apps to the cloud

---

### ⚙️ How it works
- Azure creates:
  - 2 managed domain controllers (Replica Set)
- No effort needed for:
  - Patching
  - Maintenance
  - Configuration

➡️ Everything is managed by Azure (incl. backup & encryption)

---

## 🔄 Synchronization

### 🔁 Direction:
- One-way sync:
  - Entra ID → Domain Services

### Hybrid scenario:
On-Prem AD
↓ (Entra Connect)
Microsoft Entra ID
↓ (automatic)
Domain Services


### Important:
- Changes in Domain Services:
  - ❌ are NOT synchronized back

---

## 🧩 Usage in Azure
- VMs, apps & services can:
  - Perform domain join
  - Use authentication (LDAP, Kerberos)
  - Apply group policies

---

# 🎯 Exam-Relevant Core Statements

- Microsoft Entra ID = central identity solution in Azure
- SSO = one login for many applications
- MFA increases security
- Entra Connect = connection on-prem ↔ cloud
- Domain Services = manage AD without domain controller
- Synchronization Domain Services = only one-way
- Ideal for legacy apps in the cloud
---
### Navigation
- [Parent: Module Overview](README.md)
- [Next: 🔐 Azure Authentication Methods (AZ-900)](20_azure_authentication_methods.md)
- [Home](../README.md)

