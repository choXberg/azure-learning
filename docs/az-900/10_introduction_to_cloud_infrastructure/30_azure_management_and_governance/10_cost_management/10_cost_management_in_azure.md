# 💰 Factors That Affect Costs in Azure (AZ-900)

## 🧠 Overview
- Azure uses a **consumption-based model**
- You pay only for what you use
- Costs scale with usage:
  - More usage → higher cost
  - Less usage → lower cost

---

## 🔑 Key Cost Factors

### 1️⃣ Resource Type
- Cost depends on:
  - Type of resource (VM, Storage, etc.)
  - Configuration (size, performance, redundancy)
  - Region

#### Examples:
- **Storage Account**
  - Storage type (Blob, etc.)
  - Access speed
  - Redundancy (replicas)
  - Region

- **Virtual Machine**
  - OS licensing
  - CPU & cores
  - Storage
  - Network

👉 Same resource in different regions = different cost

---

### 2️⃣ Consumption

#### 💡 Pay-as-you-go
- Pay only for usage during billing period
- Flexible and scalable

---

### 💸 Cost Optimization Options

#### Reservations
- Commit for **1 or 3 years**
- Lower price for predictable workloads
- Applies to:
  - VMs
  - Databases
  - Storage

---

#### Savings Plan (Compute)
- Commit to **hourly spend**
- Flexible across compute services
- Azure applies best pricing automatically

---

#### Spot VMs
- Use unused Azure capacity
- Very low cost
- ⚠️ Can be interrupted (evicted)

---

### 3️⃣ Maintenance
- Unused resources still cost money

#### Examples:
- Deleting a VM may NOT delete:
  - Disks
  - Networking resources

👉 Best practice:
- Regularly clean up unused resources
- Use resource groups for organization

---

### 4️⃣ Geography
- Costs vary by region due to:
  - Energy costs
  - Labor
  - Taxes

👉 Example:
- Europe → cheaper than intercontinental transfer

---

### 5️⃣ Network Traffic

#### Key Concepts:
- **Inbound (ingress)** → usually free  
- **Outbound (egress)** → charged  

---

#### Billing Zones
- Regions grouped for pricing
- Data transfer cost depends on zone

👉 Example:
- Same region → cheaper  
- Cross-region → more expensive  

---

### 6️⃣ Subscription Type
- Different subscriptions include:
  - Free credits
  - Free services

#### Example:
- Free account:
  - $ credit (first 30 days)
  - 12 months free services
  - Always-free services

---

### 7️⃣ Azure Marketplace
- Third-party solutions and services

#### Includes:
- Preconfigured VMs
- Managed services
- Specialized software

👉 Costs include:
- Azure resources
- Vendor pricing

---

## 🎯 Key Concepts (Exam Focus)

- Azure = **pay-as-you-go model**
- Cost depends on:
  - Resource type
  - Usage
  - Region
  - Network traffic
- Optimization options:
  - Reservations
  - Savings Plan
  - Spot VMs
- Inbound traffic = usually free
- Outbound traffic = charged
- Marketplace = additional vendor cost

# 💰 Azure Pricing Models – Comparison

| Model            | Flexibility | Discount | Risk |
|------------------|------------|----------|------|
| Pay-as-you-go    | ✅ High     | ❌ None   | ❌ None |
| Reservations     | ❌ Low      | ✅ High   | ❌ None |
| Savings Plan     | ✅ High     | ✅ Medium | ❌ None |
| Spot VMs         | ⚠️ Limited  | ✅ Very High | ✅ High |

---

## 🧠 Key Insight

- **Pay-as-you-go** → Maximum flexibility, no discount  
- **Reservations** → Maximum savings, low flexibility  
- **Savings Plan** → Balance between flexibility and savings  
- **Spot VMs** → Cheapest option, but unreliable  

---

## 🧠 Memory Aid

👉 **"Use – Reserve – Budget – Risk"**

| Keyword   | Model            |
|----------|------------------|
| Use      | Pay-as-you-go    |
| Reserve  | Reservations     |
| Budget   | Savings Plan     |
| Risk     | Spot VMs         |

---

## 🎯 Exam Logic

### ❓ Maximum flexibility
➡️ Pay-as-you-go  
➡️ or Savings Plan (if discount is required)

---

### ❓ Predictable workloads
➡️ Reservations  

---

### ❓ Flexibility + cost savings
➡️ Savings Plan ✅ (most common correct answer)

---

### ❓ Lowest cost, interruption acceptable
➡️ Spot VMs  

---

## 🧠 Ultra Short Exam Tip

👉 **"Fixed = Reservation, Flexible + Discount = Savings Plan, Cheap + Risk = Spot"**

---

## 🧠 Quick Memory Aid

👉 **"Type + Usage + Region + Network = Cost"**
---
### Navigation
- [Parent: Module Overview](../README.md)
- [Next: 💰 Factors That Affect Costs in Azure (AZ-900)](10_cost_management_in_azure.md)
- [Home](../../../README.md)

