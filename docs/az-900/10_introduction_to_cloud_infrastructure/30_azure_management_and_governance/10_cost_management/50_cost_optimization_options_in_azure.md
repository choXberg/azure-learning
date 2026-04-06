# 💰 Cost Optimization Options in Azure (AZ-900)

## 🧠 Overview
- After estimating and monitoring costs, the next step is **optimizing pricing**
- Azure provides different pricing models depending on workload needs

👉 Goal:
- Reduce costs
- Match pricing model to workload profile

---

## 🔑 Main Cost Optimization Options

### 🔒 Reservations
- Best for **predictable, long-running workloads**
- Commit to:
  - Specific resource (e.g., VM type)
  - 1 or 3 years

👉 Benefits:
- Significant cost savings

👉 Use when:
- Workload is stable
- Resource usage is predictable

---

### ⚖️ Azure Savings Plan for Compute
- Flexible alternative to reservations
- Commit to:
  - **Hourly spend (€ per hour)**
  - 1 or 3 years

👉 Benefits:
- Flexibility across compute services
- Automatic best pricing applied

👉 Use when:
- Usage is steady
- Resource types may change

---

### 🔥 Spot Pricing (Spot VMs)
- Uses unused Azure capacity
- Lowest cost option

👉 Benefits:
- Very high discounts

👉 Trade-off:
- ⚠️ Can be interrupted (evicted at any time)

👉 Use when:
- Workloads are fault-tolerant
- Jobs can restart

---

## 🧩 Decision Guide

| Scenario | Best Option |
|----------|------------|
| Stable, predictable workload | Reservations |
| Flexible compute usage | Savings Plan |
| Interruptible / batch workload | Spot VMs |

---

## 🧪 Practical Examples

- **Production SQL (24/7)** → Reservations  
- **Web/API workload (variable compute)** → Savings Plan  
- **Batch jobs / rendering / testing** → Spot VMs  

---

## 🔄 Continuous Optimization

- Regularly review workload patterns
- Adjust pricing model as needs change

👉 Examples:
- Spot → Reservations (if workload becomes critical)
- Pay-as-you-go → Savings Plan (if usage stabilizes)

---

## 🎯 Key Concepts (Exam Focus)

- Match pricing model to workload type
- Reservations = fixed + predictable
- Savings Plan = flexible + discounted
- Spot = cheapest but interruptible
- Optimization is **continuous process**

---

## 🧠 Quick Memory Aid

👉 **"Stable = Reservation, Flexible = Savings, Cheap = Spot"**
---
### Navigation
- [Parent: Module Overview](../README.md)
- [Next: 💰 Factors That Affect Costs in Azure (AZ-900)](10_cost_management_in_azure.md)
- [Home](../../../README.md)

