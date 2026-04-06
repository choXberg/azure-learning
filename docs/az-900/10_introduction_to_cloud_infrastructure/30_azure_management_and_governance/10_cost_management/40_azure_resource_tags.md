# 🏷️ Azure Resource Tags (AZ-900)

## 🧠 Overview
- **Tags** = metadata (key-value pairs) assigned to Azure resources
- Used to organize, manage, and track resources

👉 Tags provide additional information about resources

---

## 🎯 Why Use Tags?

Tags help with:

- Organization
- Cost tracking
- Automation
- Governance

---

## 🔑 Key Use Cases

### 📦 Resource Management
- Group resources by:
  - Workload
  - Environment
  - Team
  - Owner

👉 Makes it easier to locate and manage resources

---

### 💰 Cost Management
- Group costs by:
  - Department
  - Project
  - Cost center

👉 Helps with:
- Budget tracking
- Cost allocation
- Forecasting

---

### ⚙️ Operations Management
- Classify resources by importance

👉 Example:
- Mission-critical
- High-impact
- Low-impact

➡️ Supports SLA planning

---

### 🔐 Security
- Classify data sensitivity

👉 Example:
- Public
- Confidential

---

### 📋 Governance & Compliance
- Enforce standards and policies

👉 Example:
- Require tags like:
  - Owner
  - Department

➡️ Helps with compliance (e.g., ISO standards)

---

### 🤖 Automation
- Use tags to trigger automated actions

👉 Example:
- Deploy scripts
- Manage workloads via Azure DevOps

---

## 🧪 Common Tag Set (Best Practice)

| Tag Name     | Description |
|--------------|------------|
| Environment  | Dev / Test / Prod |
| Owner        | Responsible person |
| CostCenter   | Billing / department |
| Workload     | Application name |

---

## ⚙️ Managing Tags

You can manage tags via:

- Azure Portal
- Azure CLI
- PowerShell
- ARM Templates
- REST API

---

## 📜 Tag Governance (Important!)

- Use **Azure Policy** to:
  - Enforce required tags
  - Reapply missing tags
  - Standardize naming

---

## ⚠️ Important Behavior

- Tags are:
  - NOT inherited automatically
  - Applied individually per resource

👉 You can define different tagging strategies at:
- Resource level
- Resource group level
- Subscription level

---

## 🧩 Tag Structure

Tags consist of:

```text id="tag-structure"
Key : Value

| Key         | Value      |
| ----------- | ---------- |
| AppName     | POIneer    |
| Environment | Production |
| Owner       | Dev Team   |
| CostCenter  | IT-001     |
| Impact      | High       |

## 🎯 Key Concepts (Exam Focus)

Tags = metadata for resources

Used for:
- Organization
- Cost tracking
- Governance
- Tags are:
- Key-value pairs
- Not inherited automatically
- Azure Policy can enforce tagging rules

## 🧠 Quick Memory Aid

👉 "Tag it to track it."
---
### Navigation
- [Parent: Module Overview](../README.md)
- [Next: 💰 Factors That Affect Costs in Azure (AZ-900)](10_cost_management_in_azure.md)
- [Home](../../../README.md)

