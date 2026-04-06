# Azure Policy – Summary

## Overview
Azure Policy is a service that helps you **enforce, audit, and maintain compliance** of your Azure resources.

It allows you to define rules (policies) that control how resources are created and managed.

---

## Key Capabilities

Azure Policy enables you to:

- **Enforce rules** on resource configurations  
- **Audit compliance** of existing resources  
- **Prevent noncompliant resources** from being created  
- **Automatically remediate** noncompliant resources (in some cases)  
- **Ensure governance at scale**

---

## How Azure Policy Works

- Policies define rules and conditions for resources
- Azure evaluates resources against these policies
- Noncompliant resources are:
  - **Flagged** (audit)
  - **Blocked** (deny)
  - **Automatically fixed** (remediation, if configured)

---

## Scope and Inheritance

Policies can be assigned at different levels:

- Resource
- Resource Group
- Subscription
- Management Group

**Important:**
- Policies are **inherited**
- A policy assigned at a higher level applies to all lower levels

Example:
A policy on a resource group applies to all resources inside that group.

---

## Built-in Policies

Azure provides many built-in policies for:

- Compute
- Networking
- Storage
- Security
- Monitoring

Example:
- Restrict allowed VM sizes
- Require specific tags (e.g., `AppName`)
- Enforce security configurations

---

## Automatic Remediation

Azure Policy can:

- Add missing tags
- Fix configuration issues automatically

You can also define **exceptions** when needed.

---

## Integration with DevOps

Azure Policy integrates with CI/CD pipelines (e.g., Azure DevOps):

- Enforces rules **before deployment**
- Validates configurations **after deployment**

---

## Policy Guardrails for AI-Assisted Changes

Even when using AI tools (like Copilot):

- Policies still enforce:
  - Allowed locations
  - Required tags
  - Approved resource types (SKUs)
  - Security baselines

Ensures compliance regardless of how changes are created.

---

## Azure Policy Initiatives

An **initiative** is a group of related policies.

### Purpose:
- Manage multiple policies together
- Track compliance for broader goals

### Example:
**"Enable Monitoring in Azure Security Center" initiative**

Includes policies such as:

- Monitor unencrypted SQL databases
- Monitor OS vulnerabilities
- Monitor missing endpoint protection

(Some initiatives contain **100+ policies**)

---

## Key Takeaways (Exam Focus)

- Azure Policy = **Governance + Compliance enforcement**
- Works across all resource levels with **inheritance**
- Can:
  - **Audit**
  - **Deny**
  - **Remediate**
- Supports:
  - Built-in policies
  - Custom policies
  - Policy grouping via **initiatives**
- Enforces rules even with **AI-assisted changes**