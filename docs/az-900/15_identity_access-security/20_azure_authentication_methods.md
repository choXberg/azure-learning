# 🔐 Azure Authentication Methods (AZ-900)

## 🧠 Overview
- **Authentication** = Identity verification (User, Service, Device)
- Goal:
  - Increase security
  - Improve user-friendliness

---

## 🔑 Important Methods

- Password
- Single Sign-On (SSO)
- Multifactor Authentication (MFA)
- Passwordless Authentication

---

## ⚖️ Security vs. Comfort

| Method        | Security | Comfort |
|---------------|-----------|--------|
| Password       | ❌ Low | ✅ High |
| MFA            | ✅ High    | ⚖️ Medium |
| Passwordless   | ✅ Very High | ✅ High |

👉 **Passwordless = best combination of security & usability**

---

## 🔑 Single Sign-On (SSO)

### 📌 What is this?
- One login → Access to multiple applications

### ✅ Benefits:
- Fewer passwords (reduce "Password Sprawl")
- Fewer reset/lockout problems
- Simpler user management

### ⚠️ Important:
- Security depends on **first login**

---

## 🔐 Multifactor Authentication (MFA)

### 📌 What is this?
- Additional factor during login

### 🔑 Three Factors:

1. **Knowledge** (Something you know)
   - Password, PIN

2. **Possession** (Something you have)
   - Smartphone, Token

3. **Inherence** (Something you are)
   - Fingerprint, Face

---

### ✅ Benefit:
- Password alone is not enough → much more secure

---

## 🔐 Microsoft Entra MFA
- Azure service for MFA
- Examples:
  - SMS / Call
  - App Notification (e.g., Authenticator)

---

## 🚫 Passwordless Authentication

### 📌 What is this?
- No password needed
- Login with:
  - Device + Biometrics or PIN

### ✅ Benefits:
- No password theft possible
- Better usability
- Very high security

---

## 🔑 Passwordless Options in Azure

### 💻 Windows Hello for Business
- For personal company PCs
- Login with:
  - PIN
  - Biometrics
- Device-bound → very secure
- Supports SSO

---

### 📱 Microsoft Authenticator App
- Smartphone becomes login factor
- Process:
  - Push notification
  - Confirm number
  - Biometrics / PIN

---

### 🔑 FIDO2 Security Keys
- Hardware token (USB, NFC, Bluetooth)
- No password necessary
- Phishing-resistant

---

## 🔐 Authentication Methods Comparison (AZ-900)

| Criterion            | Password              | SSO (Single Sign-On)         | MFA (Multifactor Auth)       | Passwordless                |
|----------------------|----------------------|------------------------------|------------------------------|-----------------------------|
| Basic Idea            | One factor (Knowledge)  | One login for many apps     | Multiple factors             | No password               |
| Security           | ❌ Low           | ⚠️ Depends on login        | ✅ High                      | ✅ Very High                |
| User-Friendliness | ✅ High            | ✅ Very High                 | ⚖️ Medium                   | ✅ High                     |
| Risk               | High (Phishing, Leak)| Medium (depends on login)  | Low                      | Very Low                |
| Typical Factors    | Password             | Password / Token             | Password + Device/Biometrics   | Device + Biometrics/PIN       |
| Phishing Protection  | ❌ No              | ❌ No                      | ⚠️ Partial                 | ✅ Yes (e.g., FIDO2)         |
| Password Dependency| ✅ Yes                | ✅ Yes                        | ✅ Yes                        | ❌ No                     |
| Examples            | Standard Login       | Azure / M365 Login           | SMS, Authenticator App       | Windows Hello, FIDO2        |
| Exam Rating    | Weakest Method   | Comfort Feature              | Standard Security Measure | Best Solution                |

---

## 🧠 Schnell-Merksätze

- **Password** → simple, but insecure  
- **SSO** → convenient, but not automatically secure  
- **MFA** → standard for secure systems  
- **Passwordless** → Future (secure + convenient)

---

## 🎯 Typical Exam Logic

👉 Question: *Which method offers highest security AND comfort?*  
➡️ **Passwordless**

👉 Question: *Which method reduces password flood?*  
➡️ **SSO**

👉 Question: *Which method protects against stolen password?*  
➡️ **MFA**

👉 Question: *Which method is most vulnerable to attacks?*  
➡️ **Password**

---

## 🎯 Exam-relevant Key Statements

- **SSO** = one login for many apps
- **MFA** = multiple factors → higher security
- **Passwordless** = safest + most comfortable method
- MFA is based on:
  - Knowledge
  - Possession
  - Biometry
- FIDO2 Keys = particularly secure (no password, no phishing)

---

## 🧠 Mnemonic

👉 **"The less password, the safer."**
---
### Navigation
- [Parent: Module Overview](README.md)
- [Previous: 📘 Azure Directory Services (AZ-900)](10_azure_directory_services.md)
- [Next: 🌐 Azure External Identities (AZ-900)](30_azure_external_identities.md)
- [Home](../README.md)

