# 🛡️ AZ-900 Security Cheat Sheet

---

# 🔐 Core Security Concepts

## 🧠 Zero Trust
- Assume breach
- Verify every request
- No trust based on location

👉 Principles:
- Verify explicitly
- Use least privilege
- Assume breach

👉 **"Never trust, always verify."**

---

## 🛡️ Defense-in-Depth
- Layered security model
- Multiple protection layers

### Layers:
1. Physical
2. Identity & Access
3. Perimeter
4. Network
5. Compute
6. Application
7. Data (core)

👉 **"Multiple layers protect the data."**

---

# 👤 Identity & Access

## 🔑 Microsoft Entra ID
- Identity provider in Azure
- Manages:
  - Users
  - Groups
  - Authentication

👉 Tenant = your identity boundary

---

## 🔐 Authentication Methods

| Method        | Security | Notes |
|--------------|---------|------|
| Password     | Low     | Weakest |
| SSO          | Medium  | Convenience |
| MFA          | High    | Standard |
| Passwordless | Very High | Best option |

👉 **Passwordless = best (secure + user-friendly)**

---

## 🔄 External Identities

| Type | Use Case |
|------|---------|
| B2B  | Partners (guest users) |
| Direct Connect | Tenant-to-tenant collaboration |
| B2C  | Customers (apps) |

👉 **B2B = partners, B2C = customers**

---

## 🔐 Conditional Access
- IF condition → THEN action

### Signals:
- User
- Location
- Device
- Risk

### Actions:
- Allow
- Require MFA
- Block

👉 **Dynamic access control**

---

## 🎭 RBAC (Role-Based Access Control)

👉 Controls:
**Who can do what on which resource**

### Roles:
- Owner
- Contributor
- Reader

### Scope:
- Management Group
- Subscription
- Resource Group
- Resource

👉 Permissions inherit downward

---

# 🔐 Data Protection

## 🔒 Encryption

### Types:
- At Rest → stored data
- In Transit → moving data

👉 Use both!

---

## 🔑 Azure Key Vault
- Stores:
  - Secrets
  - Keys
  - Certificates

### Features:
- Access control
- Key rotation
- Auditing

👉 Avoid hardcoded secrets

---

# 🛡️ Threat Protection

## 🛡️ Microsoft Defender for Cloud

### Purpose:
- Security posture management
- Threat protection

### Works with:
- Azure
- Hybrid
- Multicloud

---

### 🔄 Three Pillars

1. Assess → find vulnerabilities  
2. Secure → apply best practices  
3. Defend → detect & respond  

---

### Key Features:
- Secure Score
- Security recommendations
- Threat alerts
- Azure Policy integration

---

# 🧠 Ultra Quick Exam Memory

- Zero Trust → never trust
- RBAC → who can do what
- Conditional Access → if/then rules
- MFA → multiple factors
- Passwordless → best security
- B2B vs B2C → partners vs customers
- Encryption → at rest + in transit
- Key Vault → secrets storage
- Defender → assess, secure, defend

---

# 🚀 Final Super Shortcut

👉 **Identity + Access + Data + Layers = Azure Security**