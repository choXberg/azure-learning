# Azure Storage Services Overview

## Overview

Azure Storage provides multiple services for different data types:

- Blob Storage
- Azure Files
- Queue Storage
- Table Storage

Each service is optimized for specific use cases.

---

## Blob Storage

- Object storage for unstructured data

Examples:

- Images
- Videos
- Backups
- Logs

Features:

- Massive scalability
- Supports Data Lake (analytics workloads)

Use case:
- Storing large amounts of unstructured data

---

## Azure Files

- Managed file shares in the cloud

Protocols:

- SMB (Windows)
- NFS (Linux)

Features:

- Mountable like a network drive
- Shared access across systems

Use case:
- Lift-and-shift file servers
- Shared file storage

---

## Queue Storage

- Message storage for asynchronous processing

Features:

- Store messages between components
- Decouple applications

Use case:
- Background processing
- Microservices communication

---

## Table Storage

- NoSQL key-value store

Features:

- Schema-less design
- Fast access

Use case:
- Structured, non-relational data
- Large datasets with simple queries

---

## Comparison Overview

| Service       | Data Type        | Use Case                          |
|---------------|------------------|----------------------------------|
| Blob          | Unstructured     | Files, media, backups            |
| Files         | File shares      | Shared storage (SMB/NFS)         |
| Queue         | Messages         | Async communication              |
| Table         | Key-value (NoSQL)| Structured non-relational data   |

---

## Key Differences

- Blob = object storage (most common)
- Files = traditional file system in cloud
- Queue = messaging between components
- Table = NoSQL database

---

## Exam Tips

- Blob Storage = unstructured data (most important)
- Azure Files = SMB/NFS file shares
- Queue Storage = async messaging
- Table Storage = NoSQL key-value store
- Choose service based on data type and usage pattern
---
- [Previous: Azure Storage Redundancy Options](20_azure_storage_redundancy_options.md)
- [Next: Describe Azure Storage Services](40_azure_storage_services.md)
- [Home](../../../README.md)

