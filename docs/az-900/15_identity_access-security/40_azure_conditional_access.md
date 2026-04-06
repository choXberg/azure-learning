# 🔐 Azure Conditional Access (AZ-900)

## 🧠 Overview
- **Conditional Access** = Control access based on conditions
- Part of Microsoft Entra ID
- Goal:
  - Increase security
  - Maintain user-friendliness

👉 Principle:
**"If → Then" (If condition met → then action)**

---

## 🔍 How does Conditional Access work?

### 1️⃣ Signals
During login, information is collected:

- 👤 Who? (User / Role)
- 📍 Where? (Location)
- 💻 Device (managed / unmanaged)
- 📱 Application

---

### 2️⃣ Decision
Based on the signals:

- Allow access
- Block access
- Require MFA

---

### 3️⃣ Enforcement
Action is implemented:

- ✅ Allow (Allow access)
- 🔐 Require MFA
- ❌ Block

---

## 🔄 Flow
User Login
↓
Collect signals (User, Location, Device)
↓
Check policy
↓
Action:
→ Allow
→ Require MFA
→ Block


---

## ⚙️ Typical Scenarios

### 🔐 MFA depending on conditions
- Admin → always MFA
- External access → MFA

---

### 📱 Access only via approved apps
- Only specific clients allowed (e.g., Outlook App)

---

### 💻 Access only from secure devices
- Only **managed / compliant devices**

---

### 🚫 Block risks
- Unknown locations
- Suspicious login attempts

---

## 🎯 Examples

- Login from office → ✅ Access without MFA  
- Login from another country → 🔐 MFA required  
- Login from insecure device → ❌ Access blocked  

---

## 🧠 Advantages

- Granular access control
- Higher security
- Flexible policies
- Better user experience (MFA not always required)

---

## 🎯 Exam-relevant core statements

- Conditional Access = **rule-based access**
- Decisions based on:
  - User
  - Location
  - Device
  - App
- Actions:
  - Allow
  - Require MFA
  - Block
- MFA can be **dynamically** enforced
- Important for:
  - Zero Trust Security

---

## 🧠 Mnemonic

👉 **"Access only under the right conditions."**
---
### Navigation
- [Parent: Module Overview](README.md)
- [Previous: 🧠 External Identities – Mnemonics & Exam Shortcut (AZ-900)](35_azure_external_identities_shortcut.md)
- [Next: 🔐 Azure Role-Based Access Control (RBAC)](50_azure_role_based_access_control.md)
- [Home](../README.md)

