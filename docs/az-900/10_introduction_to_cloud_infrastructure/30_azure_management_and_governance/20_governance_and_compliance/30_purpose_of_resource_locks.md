# Resource Locks in Azure – Summary

## Overview
Resource locks in Azure help **prevent accidental deletion or modification** of critical resources.

Even if users have sufficient permissions (via Azure RBAC), locks add an extra layer of protection.

---

## Key Features

- Protect resources from **accidental changes or deletion**
- Work **independently of RBAC permissions**
- Can be applied at different levels:
  - Resource
  - Resource Group
  - Subscription
- **Inheritance applies**:
  - Locks at a higher level apply to all child resources

---

## Types of Resource Locks

### 1. Delete Lock (CanNotDelete)

- Users can:
  - Read resources
  - Modify resources
- Users **cannot delete** the resource

---

### 2. ReadOnly Lock

- Users can:
  - Read resources only
- Users **cannot modify or delete** the resource

> Note: This is similar to assigning the **Reader role** to all users.

---

## Behavior and Enforcement

- Locks override permissions from Azure RBAC
- Even resource owners must respect locks
- Prevents **accidental operations**, not intentional ones (locks can be removed)

---

## Managing Resource Locks

You can manage locks using:

- Azure Portal (Settings → Locks)
- Azure CLI
- Azure PowerShell
- Azure Resource Manager (ARM) templates

---

## Modifying Locked Resources

To change or delete a locked resource:

1. **Remove the lock**
2. Perform the desired action (if permissions allow)

---

## Key Takeaways (Exam Focus)

- Resource locks = **Protection against accidental changes**
- Two types:
  - **Delete (CanNotDelete)** → cannot delete
  - **ReadOnly** → cannot modify or delete
- Locks:
  - Apply at multiple levels
  - Are **inherited**
  - Override RBAC permissions
- Must be **removed before changes** can be made
---
### Navigation
- [Parent: Module Overview](../README.md)
- [Next: Microsoft Purview – Summary](10_microsoft_purview.md)
- [Home](../../../README.md)

