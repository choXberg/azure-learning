# Cloud Models – Use Cases

## Overview

This document summarizes typical use cases for the four cloud models:

- Private Cloud
- Public Cloud
- Hybrid Cloud
- Multi-Cloud

---

## Private Cloud

### Description
A cloud environment dedicated to a single organization. Can be hosted on-premises or by a third-party provider.

### Typical Use Cases

- **Highly sensitive data**
  - Healthcare systems
  - Financial institutions
- **Regulatory compliance**
  - GDPR-restricted workloads
- **Legacy systems**
  - Systems that cannot be migrated easily
- **Full control required**
  - Custom security or networking requirements

### Example

- Company runs its own datacenter for internal ERP systems

---

## Public Cloud

### Description
Cloud services provided over the internet and available to anyone.

### Typical Use Cases

- **Web applications**
  - APIs, websites, SaaS platforms
- **Startups / MVPs**
  - Fast time-to-market
- **Scalable workloads**
  - Traffic spikes (e.g. e-commerce)
- **Dev/Test environments**
  - Temporary infrastructure

### Example

- Hosting a REST API in Azure App Service
- Storing files in AWS S3

---

## Hybrid Cloud

### Description
Combination of private and public cloud environments connected together.

### Typical Use Cases

- **Gradual cloud migration**
  - Move workloads step by step
- **Cloud bursting**
  - Handle peak loads in public cloud
- **Sensitive + scalable split**
  - Database on-prem, frontend in cloud
- **Backup & disaster recovery**
  - Replication to public cloud

### Example

- On-prem database + Azure-hosted web frontend
- Backup to cloud storage

---

## Multi-Cloud

### Description
Use of multiple cloud providers simultaneously.

### Typical Use Cases

- **Avoid vendor lock-in**
- **Best-of-breed services**
  - AI from one provider, storage from another
- **High availability**
  - Redundancy across providers
- **Global strategy**
  - Different providers in different regions

### Example

- Azure for backend services + AWS for storage
- Google Cloud for AI + Azure for infrastructure

---

## Quick Comparison

| Scenario                          | Recommended Model |
|----------------------------------|------------------|
| Maximum control & security        | Private Cloud    |
| Fast scaling & low cost           | Public Cloud     |
| Mix of control and flexibility    | Hybrid Cloud     |
| Multiple providers strategy       | Multi-Cloud      |

---

## Exam Tips (AZ-900)

- **Private Cloud** = Full control, higher cost  
- **Public Cloud** = Scalable, shared resources  
- **Hybrid Cloud** = Private + Public combined  
- **Multi-Cloud** = Multiple cloud providers  

> ⚠️ Important:
> Hybrid ≠ Multi-Cloud  
> Hybrid = mixed environments  
> Multi-Cloud = multiple providers

---

## Summary

Choosing the right cloud model depends on:

- Security requirements
- Cost considerations
- Scalability needs
- Existing infrastructure
- 
---

[Cloud Concepts](README.md)
---
### Navigation
- [Parent: Module Overview](README.md)
- [Previous: ☁️ Cloud Models – Kurz & Knackig](30_cloud_models.md)
- [Next: ☁️ Consumption-Based Model (Pay-as-you-go)](50_consumption_based_model.md)
- [Home](../../README.md)

