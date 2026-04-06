# 🌐 Azure External Identities (AZ-900)

## 🧠 Overview
- **External Identity** = Identity outside your tenant
  - e.g., Partners, customers, suppliers, external developers
- Enables:
  - Access to resources **without internal accounts**

---

## 🎯 Why are external identities important?
- Collaboration with:
  - Partners
  - Suppliers
  - Customers
- Advantages:
  - No need for own user management
  - Users use **their own accounts**
- You control:
  - Access (Authorization)
- External provider controls:
  - Login (Authentication)

---

## 🔐 Identity Provider (important!)
External users can log in with:
- Company account (another tenant)
- Social login (Google, Facebook)
- Microsoft Account
- Government identities

---

## 🔄 Differentiation from SSO

| Topic | Description |
|------|-------------|
| SSO | Login within one tenant |
| External Identities | Access across tenant boundaries |

---

## ⚙️ External Identity Features

### 🤝 B2B Collaboration
- External users are created as **Guest User** in your tenant
- Access to:
  - Apps
  - Resources
- Usage:
  - Classic collaboration

---

### 🔗 B2B Direct Connect
- Connection between two tenants (Trust)
- No guest user in tenant necessary
- Currently:
  - Focus on Microsoft Teams (Shared Channels)
- Users remain in their own tenant

---

### 👥 External ID for Customers (Azure AD B2C)
- For:
  - Customers / end users (B2C scenario)
- Usage:
  - Own apps (SaaS / Custom Apps)
- Management:
  - Separate tenant

---

## 🧩 Comparison of Models

| Feature                | B2B Collaboration | B2B Direct Connect | External ID (B2C) |
|------------------------|------------------|--------------------|-------------------|
| Target group           | Partners / Guests| Partners (Teams)   | Customers         |
| Users in tenant        | ✅ Yes (Guest)    | ❌ No              | ❌ Separate       |
| Typical use case       | App access       | Teams Collaboration| Customer apps     |

---

## 👉 Difference B2B Direct Connect vs B2B Collaboration:

| Feature              | B2B Collaboration | B2B Direct Connect         |
| -------------------- | ----------------- | -------------------------- |
| Guest User           | ✅ Yes             | ❌ No                      |
| Tenant switch needed | Often yes         | ❌ No                      |
| Teams Integration    | Limited           | ✅ Native (Shared Channels)|

---
## Quick comparison (perfect for exam)

| Topic       | B2B                  | B2C                            |
| ----------- | -------------------- | ------------------------------ |
| Meaning     | Business to Business | Business to Consumer           |
| Target group| Partners / Companies | Customers / End users          |
| Access to   | Internal resources   | Public apps                    |
| User type   | Guest User in tenant | External user in own system    |
| Login       | Company account      | Social login / Email           |

## 🧠 Ultimate mnemonic

- 👉 B2B = Partners work with you
- 👉 B2C = Customers use your product

## 🎯 Exam shortcut
- "Partner accesses my resources" → B2B
- "Customer logs into app" → B2C

## 🔄 Manage access (very important!)

### 👀 Access Reviews
- Regular review:
  - Does the user still need access?
- Involved:
  - User themselves or decision makers
- Result:
  - Keep or remove access

---

## 🎯 Exam-relevant core statements

- External Identities = Access **outside your tenant**
- Authentication = external provider
- Authorization = your tenant (Entra ID)
- B2B Collaboration = Guest User in tenant
- B2B Direct Connect = no Guest User
- B2C = for customers (separate tenant)
- Access Reviews = check access regularly

---

## 🧠 Mnemonic

👉 **"Log in externally – control internally."**
---
### Navigation
- [Parent: Module Overview](README.md)
- [Previous: 🔐 Azure Authentication Methods (AZ-900)](20_azure_authentication_methods.md)
- [Next: 🧠 External Identities – Mnemonics & Exam Shortcut (AZ-900)](35_azure_external_identities_shortcut.md)
- [Home](../README.md)

