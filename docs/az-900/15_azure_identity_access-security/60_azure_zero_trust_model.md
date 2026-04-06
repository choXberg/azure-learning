# 🔐 Zero Trust Model (AZ-900)

## 🧠 Overview
- **Zero Trust** = security model that assumes **breach by default**
- No implicit trust:
  - Every request must be verified
- Works for:
  - Cloud environments
  - Mobile workforce
  - Distributed systems

👉 Core idea:
**"Never trust, always verify."**

---

## 🔑 Core Principles

### 1️⃣ Verify Explicitly
- Always authenticate and authorize
- Use all available signals:
  - User identity
  - Location
  - Device state
  - Risk level

---

### 2️⃣ Use Least Privilege Access
- Grant only required permissions
- Techniques:
  - Just-In-Time (JIT)
  - Just-Enough-Access (JEA)
  - Risk-based policies

---

### 3️⃣ Assume Breach
- Design systems as if attacker is already inside
- Actions:
  - Segment access
  - Use encryption end-to-end
  - Monitor and detect threats

---

## 🔄 Traditional vs Zero Trust

| Traditional Model            | Zero Trust Model              |
|-----------------------------|-------------------------------|
| Trust based on network      | Trust based on verification   |
| Internal network = safe     | No network is trusted         |
| VPN = secure access         | Every request validated       |
| Static access decisions     | Continuous evaluation         |

---

## ⚙️ How It Works

1. User attempts access  
2. System evaluates signals:
   - Identity
   - Device
   - Location
   - Risk  
3. Decision:
   - Allow
   - Require MFA
   - Block  

👉 Decisions are **context-aware and continuous**

---

## 🧪 Example Scenario

- User logs in:
  - From public network
  - Using unmanaged device  

👉 System response:
- Low-risk app → allow  
- Sensitive app → require MFA  
- High risk → block  

---

## 🎯 Key Concepts (Exam Focus)

- Zero Trust = **assume breach**
- No trust based on network location
- Access is:
  - Verified
  - Context-aware
  - Continuously evaluated
- Based on:
  - Identity
  - Device
  - Risk signals

---

## 🧠 Quick Memory Aid

👉 **"Never trust, always verify."**