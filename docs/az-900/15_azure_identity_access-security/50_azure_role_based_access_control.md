# 🔐 Azure Role-Based Access Control (RBAC)

## 🧠 Overview
- **Azure RBAC** = system to manage access to Azure resources
- Based on the **principle of least privilege**:
  - Users only get the permissions they need
  - No unnecessary access

---

## ⚙️ Core Concept

Instead of assigning permissions individually:
- Assign **roles** to users or groups
- Each role contains a set of permissions

👉 Example:
- New engineer joins → assign to "Engineer role"
- Automatically gets required access

---

## 🎭 Roles

- Azure provides **built-in roles**, such as:
  - Owner → full access
  - Contributor → manage resources (no access control)
  - Reader → read-only access

- You can also create **custom roles**

---

## 👥 Role Assignment

- Assign roles to:
  - Users
  - Groups
  - Applications / services

👉 Users inherit all permissions from assigned roles

---

## 📦 Scope (VERY IMPORTANT)

RBAC is applied to a **scope**:

- Management Group (highest level)
- Subscription
- Resource Group
- Resource (lowest level)

---

## 🔄 Hierarchy & Inheritance

- RBAC is **hierarchical**
- Permissions flow **top → down**

👉 Example:
- Owner at Management Group → access to all subscriptions & resources
- Reader at Subscription → read access to everything inside

---

## 🔐 Enforcement

- RBAC is enforced by **Azure Resource Manager (ARM)**
- Applies to:
  - Azure Portal
  - Azure CLI
  - PowerShell
  - APIs

👉 Important:
- RBAC controls **resource-level access**
- ❌ NOT application/data-level security

---

## ➕ Allow Model

- RBAC follows an **allow model**

👉 If any role grants permission:
- ✅ Access is allowed

Example:
- Role 1 → Read
- Role 2 → Write  
➡️ Result: **Read + Write access**

---

## 🎯 Key Concepts (Exam Focus)

- RBAC = access control via roles
- Based on **least privilege principle**
- Roles = collection of permissions
- Scope defines **where access applies**
- Permissions are **inherited downward**
- Managed via **Azure Resource Manager**
- Uses **allow model**

---

## 🧠 Quick Memory Aid

👉 **"RBAC = Who can do what, on which resource."**