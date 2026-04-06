# Identify Azure File Movement Options

## Overview

Azure provides tools for moving and managing individual files or small datasets:

- AzCopy (command-line tool)
- Azure Storage Explorer (GUI tool)
- Azure File Sync (hybrid sync solution)

These tools complement large-scale migration services like Azure Migrate and Azure Data Box.

---

## AzCopy

### Overview

AzCopy is a command-line utility for transferring data to and from Azure Storage.

---

### Capabilities

- Upload files to Azure
- Download files from Azure
- Copy data between storage accounts
- Synchronize files or blobs (one direction only)

---

### Key Characteristics

- Scriptable and automation-friendly
- High performance
- Supports cross-cloud transfers

Important:

- Synchronization is **one-way only**
- You define source → destination
- No bi-directional sync

---

### Use Cases

- Automated data transfer
- Batch operations
- CI/CD pipelines

---

## Azure Storage Explorer

### Overview

Azure Storage Explorer is a graphical tool for managing Azure Storage.

- Runs on:
  - Windows
  - macOS
  - Linux

---

### Capabilities

- Upload and download files
- Manage blobs and storage accounts
- Copy data between storage accounts

---

### Key Characteristics

- User-friendly GUI
- Uses AzCopy in the background
- No scripting required

---

### Use Cases

- Manual file management
- Exploring storage accounts
- Small-scale data transfers

---

## Azure File Sync

### Overview

Azure File Sync synchronizes on-premises file servers with Azure Files.

- Enables hybrid cloud scenarios
- Provides bi-directional synchronization

---

### Key Features

- Bi-directional sync between:
  - Local server
  - Azure Files

- Supports standard protocols:
  - SMB
  - NFS
  - FTPS

- Multiple global caches possible

---

### Cloud Tiering

- Frequently accessed files → stored locally
- Infrequently accessed files → stored in Azure

Benefits:

- Saves local storage space
- Maintains performance

---

### Additional Benefits

- Replace failed servers easily
- Centralized file storage in Azure
- Acts like a distributed file system

---

## Comparison Overview

| Tool                    | Type        | Sync Type        | Use Case                          |
|--------------------------|------------|------------------|----------------------------------|
| AzCopy                   | CLI        | One-way          | Automation, scripting             |
| Storage Explorer         | GUI        | One-way          | Manual file management            |
| Azure File Sync          | Hybrid     | Bi-directional   | On-prem ↔ Azure synchronization   |

---

## Exam Tips

- AzCopy = command-line, one-way sync
- Storage Explorer = GUI tool (uses AzCopy internally)
- Azure File Sync = bi-directional sync with on-prem servers
- File Sync supports cloud tiering (hot local, cold in cloud)
- Use AzCopy for automation, Storage Explorer for manual tasks