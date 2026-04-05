# Describe Azure DNS

## Overview

Azure DNS is a hosting service for DNS domains that provides name resolution using Microsoft Azure infrastructure.

- Manage DNS records using Azure tools, APIs, and credentials
- Fully integrated with Azure services

Note:
Azure DNS is used for DNS hosting, not for purchasing domain names.

---

## Benefits of Azure DNS

- High reliability and performance
- Strong security features
- Easy management via Azure tools
- Support for private DNS domains
- Alias records for Azure resources

---

## Reliability and Performance

- Hosted on Azure's global DNS infrastructure
- Uses anycast networking:
  - Requests are routed to the nearest DNS server
- Provides:
  - High availability
  - Low latency

---

## Security

Based on Azure Resource Manager (ARM), providing:

- Azure RBAC (Role-Based Access Control)
- Activity logs
- Resource locks

Benefits:

- Fine-grained access control
- Protection against accidental changes

---

## Ease of Use

- Integrated into Azure Portal
- Uses same:
  - Credentials
  - Billing
  - Support model

Management options:

- Azure Portal
- Azure CLI
- Azure PowerShell
- REST API and SDKs

---

## Private DNS (Custom Domains in VNets)

- Supports private DNS zones
- Use custom domain names inside virtual networks

Example:

- Instead of internal Azure names → use your own domain (e.g. app.internal.local)

Benefits:

- Cleaner architecture
- Easier service discovery

---

## Alias Records

- Point DNS records directly to Azure resources

Examples:

- Public IP address
- Azure Traffic Manager
- Azure CDN endpoint

Key advantage:

- Automatically updates when underlying IP changes
- No manual DNS updates required

---

## Important Notes

- Azure DNS does NOT sell domain names
- Domains must be purchased via:
  - App Service Domains
  - Third-party registrars

- After purchase, domains can be hosted in Azure DNS

---

## Exam Tips

- Azure DNS = DNS hosting service (name resolution)
- Uses anycast → fastest DNS response
- Integrated with Azure RBAC for security
- Supports private DNS zones for VNets
- Alias records auto-update when IP changes
- Cannot buy domains directly via Azure DNS