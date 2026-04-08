# Azure VM Architecture (AZ-900)

## Overview

When you create a Virtual Machine (VM) in Azure, you are not creating a single resource.  
Instead, Azure automatically provisions multiple related resources that work together.

Understanding this composition is essential for AZ-900 and real-world Azure usage.

---

## Core Concept

A Virtual Machine in Azure is a combination of compute, networking, and storage resources.

```
Virtual Machine
↓
Network Interface (NIC)
↓
Virtual Network (VNet)
↓
Subnet
```

Additional components:
Public IP → NIC → VM
Network Security Group (NSG) → NIC or Subnet
Managed Disk → VM


---

## Key Components

### 1. Virtual Machine
- The compute resource
- Runs the operating system (e.g., Windows Server, Linux)

---

### 2. Network Interface (NIC)
- Connects the VM to a Virtual Network
- Handles IP configuration (private IP, optional public IP)
- A VM is attached to at least one NIC

---

### 3. Virtual Network (VNet)
- Azure’s private network
- Enables communication between resources
- Scoped to a specific region

---

### 4. Subnet
- A logical subdivision of a VNet
- Helps organize and secure resources

---

### 5. Public IP Address
- Enables external access (e.g., RDP or SSH)
- Not required for internal communication

---

### 6. Network Security Group (NSG)
- Acts as a firewall
- Controls inbound and outbound traffic
- Can be attached to:
  - NIC
  - Subnet

Example:
- Allow RDP (3389)
- Block ICMP (ping) by default

---

### 7. Managed Disk
- Stores the operating system and data
- Azure-managed storage
- Automatically attached to the VM

---

## How Communication Works

Two VMs in the same VNet can communicate with each other:

- via **private IP**
- via **Azure-provided DNS (hostname resolution)**

### Example:

```powershell
ping vm2
```

## Requirements:

- Same VNet
- No blocking NSG rules
- OS firewall allows traffic

## Important Notes (AZ-900 Exam)
- A VM is not a standalone resource
- Multiple resources are created automatically
- Networking is handled via the NIC, not directly by the VM
- VNets are region-specific
- Internal communication does not require a public IP

## Common Mistakes
- ❌ VM not in the correct VNet → no connectivity
- ❌ Region mismatch → resources cannot be linked
- ❌ NSG blocking traffic → communication fails
- ❌ OS firewall blocking ping (ICMP)
- ❌ Assuming VM is a single resource

## Key Takeaway

In Azure, everything is a resource — and most solutions are composed of multiple interconnected resources.

Understanding these relationships is more important than memorizing individual services.