# Describe Azure Storage Services

## Overview

Azure Storage provides five core data services:

- Blob Storage
- Azure Files
- Queue Storage
- Azure Disks
- Table Storage

These services are designed for different data types and use cases.

---

## Benefits of Azure Storage

- Durable and highly available (via redundancy options)
- Secure (encryption + access control)
- Massively scalable
- Fully managed by Azure
- Globally accessible via HTTP/HTTPS

Access methods:

- REST API
- SDKs (e.g. .NET, Java, Python)
- Azure CLI / PowerShell
- Azure Portal
- Azure Storage Explorer

---

## Blob Storage

### Overview

- Object storage for unstructured data
- Stores data as blobs (binary large objects)

### Use Cases

- Images and documents for web apps
- Video and audio streaming
- Backups and disaster recovery
- Logs and analytics data
- Data lake / big data workloads

### Access

- Via URL (HTTP/HTTPS)
- REST API, SDKs, CLI, PowerShell

---

## Blob Storage Access Tiers

Blob Storage provides cost optimization based on access frequency:

### Hot Tier
- Frequent access
- Highest storage cost
- Lowest access cost

---

### Cool Tier
- Infrequent access (≥ 30 days)
- Lower storage cost
- Higher access cost

---

### Cold Tier
- Rare access (≥ 90 days)
- Lower storage cost than Cool
- Higher access cost

---

### Archive Tier

- Rarely accessed (≥ 180 days)
- Lowest storage cost
- Highest access cost
- High latency (rehydration required)

---

## Azure Files

### Overview

- Managed file shares in the cloud
- Accessible via:

  - SMB (Windows, Linux, macOS)
  - NFS (Linux, macOS)

### Features

- Mountable like a network drive
- Shared access across environments
- Supports hybrid scenarios

### Use Cases

- Lift-and-shift file servers
- Shared application storage
- Hybrid cloud file access

---

## Azure Queues

### Overview

- Messaging service for asynchronous communication

### Features

- Stores millions of messages
- Max message size: 64 KB
- Access via HTTP/HTTPS

### Use Cases

- Decoupling application components
- Background processing
- Event-driven architectures

Example:
- Queue + Azure Functions

---

## Azure Disks

### Overview

- Block-level storage for Azure Virtual Machines
- Managed disks (handled by Azure)

### Features

- High performance
- High durability
- Simplified management

### Use Cases

- OS disks for VMs
- Data disks for applications

---

## Azure Table Storage

### Overview

- NoSQL key-value store
- Schema-less design

### Features

- Stores structured, non-relational data
- Fast and scalable

### Use Cases

- Large datasets
- Simple queries
- Applications needing flexible schema

---

## Comparison Overview

| Service       | Data Type        | Use Case                          |
|---------------|------------------|----------------------------------|
| Blob          | Unstructured     | Files, media, backups, analytics |
| Files         | File shares      | Shared storage (SMB/NFS)         |
| Queue         | Messages         | Async processing                 |
| Disks         | Block storage    | VM storage                       |
| Table         | NoSQL            | Structured non-relational data   |

---

## Exam Tips

- Blob Storage = most important (unstructured data)
- Blob tiers = cost vs access frequency (Hot → Archive)
- Azure Files = SMB/NFS file shares
- Queue Storage = async messaging
- Azure Disks = VM storage (block-level)
- Table Storage = NoSQL key-value store
- Choose service based on data type and usage pattern