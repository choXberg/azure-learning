# Azure Arc – Summary

## Overview

Azure Arc extends Azure management capabilities to **hybrid and multicloud environments**.

It allows you to manage resources **outside of Azure** (on-premises and other cloud providers) as if they were native Azure resources.

---

## Purpose

Azure Arc helps you:

- Simplify **hybrid and multicloud management**
- Apply **consistent governance and compliance**
- Use Azure tools across all environments

---

## How Azure Arc Works

Azure Arc integrates with **Azure Resource Manager (ARM)** to:

- Project non-Azure resources into Azure
- Manage them using standard Azure tools and services

---

## Key Capabilities

Azure Arc enables you to:

- **Manage all resources in one place**
  - Azure
  - On-premises
  - Multicloud

- Treat external resources as if they run in Azure:
  - Virtual machines
  - Kubernetes clusters
  - Databases

- Apply:
  - Azure Policy
  - Monitoring
  - Security controls

- Use familiar Azure services regardless of location

---

## Hybrid & Multicloud Benefits

- Unified governance across environments
- Centralized inventory and management
- Consistent policy enforcement
- Reduced complexity

---

## DevOps & IT Operations

Azure Arc supports both:

- **Traditional IT operations (ITOps)**
- **Modern DevOps practices**

This enables gradual adoption of cloud-native approaches.

---

## Custom Locations

- Provides an abstraction layer on top of Kubernetes clusters
- Allows deploying Azure services to Arc-enabled environments

---

## Supported Resource Types (Outside Azure)

Azure Arc can manage:

- Servers
- Kubernetes clusters
- Azure data services
- SQL Server
- Virtual machines (preview)

---

## Practical Example

An organization uses:

- Azure
- On-premises datacenter
- Another cloud provider

With Azure Arc:

- All environments are managed from Azure
- Policies and monitoring are applied consistently
- No need for separate management tools

---

## Key Takeaways (Exam Focus)

- Azure Arc = **Hybrid + Multicloud management**
- Extends Azure to:
  - On-premises
  - Other clouds
- Uses **Azure Resource Manager**
- Enables:
  - Unified governance
  - Policy enforcement
  - Centralized management
- Supports multiple resource types outside Azure