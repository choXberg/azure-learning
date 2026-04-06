# Describe Azure Storage Accounts

[learn.microsoft.com](https://learn.microsoft.com/en-us/training/modules/describe-azure-storage-services/2-accounts)

## Overview

An Azure Storage Account provides a unique namespace for your data in Azure.

- Accessible globally via HTTP or HTTPS
- Data is:
  - Secure
  - Highly available
  - Durable
  - Massively scalable

---

## Storage Account Types

The storage account type determines:

- Supported services
- Performance characteristics
- Redundancy options
- Use cases

### Standard General-Purpose v2 (Recommended)

- Services:
  - Blob Storage (incl. Data Lake Storage)
  - Queue Storage
  - Table Storage
  - Azure Files
- Redundancy:
  - LRS, GRS, RA-GRS, ZRS, GZRS, RA-GZRS
- Use case:
  - Default choice for most scenarios

---

### Premium Block Blobs

- Services:
  - Blob Storage (block + append blobs)
- Redundancy:
  - LRS, ZRS
- Use case:
  - High transaction rates
  - Low latency requirements
  - Smaller objects

---

### Premium File Shares

- Services:
  - Azure Files only
- Redundancy:
  - LRS, ZRS
- Use case:
  - High-performance file shares
  - Supports SMB and NFS

---

### Premium Page Blobs

- Services:
  - Page blobs only
- Redundancy:
  - LRS
- Use case:
  - Specialized scenarios (e.g. virtual disks)

---

## Redundancy Options (Overview)

- LRS (Locally Redundant Storage)
- GRS (Geo-Redundant Storage)
- RA-GRS (Read-Access Geo-Redundant Storage)
- ZRS (Zone-Redundant Storage)
- GZRS (Geo-Zone-Redundant Storage)
- RA-GZRS (Read-Access Geo-Zone-Redundant Storage)

Note:
Redundancy defines how data is replicated for durability and availability.

---

## Storage Account Namespace

- Each storage account has a unique name in Azure
- This creates a globally unique namespace

Naming rules:

- Length: 3–24 characters
- Allowed characters:
  - Lowercase letters
  - Numbers
- Must be globally unique across Azure

---

## Storage Account Endpoints

Each storage service has its own endpoint format:

| Service                     | Endpoint Format                                                   |
|----------------------------|-------------------------------------------------------------------|
| Blob Storage               | https://<account-name>.blob.core.windows.net                     |
| Data Lake Storage Gen2     | https://<account-name>.dfs.core.windows.net                      |
| Azure Files                | https://<account-name>.file.core.windows.net                     |
| Queue Storage              | https://<account-name>.queue.core.windows.net                    |
| Table Storage              | https://<account-name>.table.core.windows.net                    |

---

## Key Concepts

- One storage account can host multiple storage services
- Each service has its own endpoint
- Global namespace ensures unique access to data

---

## Exam Tips

- Storage account = entry point for Azure Storage services
- General-purpose v2 = default and most common choice
- Premium accounts = high performance / low latency
- Storage account name must be globally unique
- Each service has its own endpoint URL
- Redundancy options define durability and availability
---
- [Next: Azure Storage Redundancy Options](20_azure_storage_redundancy_options.md)
- [Home](../../../README.md)

