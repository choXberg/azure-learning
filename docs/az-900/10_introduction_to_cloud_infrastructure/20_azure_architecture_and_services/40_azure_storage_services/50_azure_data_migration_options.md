# Identify Azure Data Migration Options

## Overview

Azure provides two main approaches for migrating data to the cloud:

- Azure Migrate (online / real-time migration)
- Azure Data Box (offline / physical migration)

Choice depends on:

- Data size
- Network bandwidth
- Time constraints

---

## Azure Migrate

### Overview

Azure Migrate is a centralized service for migrating:

- Infrastructure
- Applications
- Data

From on-premises environments to Azure.

---

### Key Features

- Unified migration platform
  - Single portal for managing migrations
- Assessment tools
  - Evaluate readiness before migration
- Migration tools
  - Move workloads to Azure

---

### Integrated Capabilities

Azure Migrate includes tools for:

- Discovery and assessment
- Server migration
- Database migration
- Web app migration

Also supports:

- Integration with other Azure services
- Third-party (ISV) tools

---

### Use Cases

- Lift-and-shift migrations
- Full datacenter migration to Azure
- Incremental or staged migrations

---

## Azure Data Box

### Overview

Azure Data Box is a physical data transfer solution.

- Microsoft ships a storage device to you
- You copy data locally
- Device is returned to Microsoft
- Data is uploaded to Azure

---

### Key Characteristics

- Max capacity: up to ~80 TB
- Secure and rugged device
- End-to-end tracking via Azure Portal
- Data encrypted during transfer

---

### Workflow

1. Order Data Box via Azure Portal
2. Receive device
3. Copy data locally
4. Ship device back to Microsoft
5. Data uploaded to Azure automatically

---

### Use Cases

- Large data migrations (tens of TB or more)
- Limited network bandwidth
- One-time bulk data transfer
- Periodic large uploads
- Data export from Azure (e.g. compliance, recovery)

---

### Security

- Data protected during transport
- Devices wiped after use
- Compliant with NIST 800-88r1 standards

---

## Comparison Overview

| Feature            | Azure Migrate                  | Azure Data Box                  |
|--------------------|-------------------------------|--------------------------------|
| Migration Type     | Online                        | Offline (physical)             |
| Data Transfer      | Over network                  | Physical device                |
| Speed              | Depends on bandwidth          | Fast for large datasets        |
| Data Size          | Small to large                | Very large (TB scale)          |
| Use Case           | Continuous migration          | Bulk transfer                  |

---

## Exam Tips

- Azure Migrate = online migration service (assessment + migration)
- Azure Data Box = physical device for large data transfer
- Use Data Box when:
  - Data is very large
  - Network is too slow
- Use Azure Migrate for:
  - Full environment migration
  - Continuous or staged migration
- Data Box = offline, Azure Migrate = online