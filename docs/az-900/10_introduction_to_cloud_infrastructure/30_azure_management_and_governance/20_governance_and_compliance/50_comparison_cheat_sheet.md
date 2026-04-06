# Azure Governance & Compliance – Comparison Cheat Sheet

## Overview

This cheat sheet compares four important Azure services:

- Microsoft Purview
- Azure Policy
- Resource Locks
- Service Trust Portal

---

## Quick Comparison Table

| Service                  | Purpose                                      | What it does                                      | When to use it                          |
|-------------------------|----------------------------------------------|---------------------------------------------------|-----------------------------------------|
| Microsoft Purview       | Data governance & compliance                 | Discovers, classifies, and tracks data            | Manage and understand your data estate  |
| Azure Policy            | Enforce rules & compliance                   | Audits, denies, or remediates resources           | Enforce standards and configurations    |
| Resource Locks          | Protect resources                            | Prevents deletion or modification                 | Avoid accidental changes                |
| Service Trust Portal    | Transparency & documentation                 | Provides reports, audits, certifications          | Prove compliance and review standards   |

---

## Detailed Comparison

### Microsoft Purview

- Focus: **Data governance**
- Works across:
  - On-premises
  - Azure
  - Multicloud
  - SaaS
- Key features:
  - Data discovery
  - Data classification
  - Data lineage

👉 **Think:** "Understand and govern my data"

---

### Azure Policy

- Focus: **Enforcement and compliance**
- Can:
  - Audit resources
  - Deny noncompliant resources
  - Remediate configurations
- Supports:
  - Built-in policies
  - Custom policies
  - Initiatives (grouped policies)

👉 **Think:** "Enforce rules in my environment"

---

### Resource Locks

- Focus: **Protection**
- Types:
  - Delete (CanNotDelete)
  - ReadOnly
- Prevents:
  - Accidental deletion
  - Accidental modification
- Overrides RBAC permissions

👉 **Think:** "Protect critical resources"

---

### Service Trust Portal

- Focus: **Transparency and compliance documentation**
- Provides:
  - Audit reports
  - Certifications (ISO, SOC, etc.)
  - Security and privacy documentation
- Requires login and NDA for some documents

👉 **Think:** "Show compliance and trust"

---

## Key Differences (Exam Focus)

- **Azure Policy vs Resource Locks**
  - Policy → controls what *can be created or configured*
  - Locks → protect existing resources from changes

- **Azure Policy vs RBAC**
  - RBAC → who can do what
  - Policy → what is allowed

- **Microsoft Purview vs Azure Policy**
  - Purview → focuses on **data**
  - Policy → focuses on **resources/configuration**

- **Service Trust Portal**
  - Does NOT enforce anything
  - Only provides **information and documentation**

---

## Memory Trick

- **Purview** → Data 📊  
- **Policy** → Rules 📏  
- **Locks** → Protection 🔒  
- **Service Trust Portal** → Proof 📄  

---

## Final Exam Tip

If the question is about:

- **Data governance** → Microsoft Purview  
- **Enforcing rules** → Azure Policy  
- **Preventing deletion/changes** → Resource Locks  
- **Viewing compliance reports** → Service Trust Portal  