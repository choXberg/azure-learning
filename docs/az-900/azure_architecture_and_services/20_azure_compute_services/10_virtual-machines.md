# Azure Virtual Machines (VMs)

## 🧠 Overview
Azure Virtual Machines (VMs) are an **Infrastructure as a Service (IaaS)** offering.

They allow you to run virtualized servers in Azure with full control over:

- Operating System (OS)
- Installed software
- Configuration

💡 **Key Point:**  
> You manage the OS, updates, and applications — Azure manages the hardware.

---

## 🎯 When to Use Virtual Machines

Use VMs when you need:

- Full control over the OS
- Custom software or configurations
- Legacy application support

---

## 📌 Common Use Cases

- **Testing & Development**
  - Quickly create and delete environments

- **Cloud Application Hosting**
  - Run scalable applications in Azure

- **Datacenter Extension**
  - Extend on-premises infrastructure to Azure

- **Disaster Recovery**
  - Failover workloads to Azure

- **Lift-and-Shift Migration**
  - Move existing workloads with minimal changes

---

## 🧱 VM Resources (Sizing)

When creating a VM, you define:

- **Size** (vCPU, RAM)
- **Storage** (HDD, SSD)
- **Networking** (VNet, IP, ports)

---

## ⚙️ Key Sizing Dimensions

| Dimension            | Description |
|---------------------|------------|
| vCPU                | Compute power |
| RAM                 | Memory capacity |
| Disk                | Storage size, IOPS, throughput |
| Network throughput  | Data transfer performance |
| Premium SSD support | High-performance storage |
| Hardware generation | Underlying platform version |

💡 **Key Point:**  
> Choose size based on workload (CPU, memory, storage, network).

---

## 🧬 VM Size Families (Exam Important)

| Family   | Focus                | Example Use Case |
|----------|---------------------|-----------------|
| B-series | Burstable           | Dev/Test with occasional spikes |
| D-series | General purpose     | Web/app servers |
| E-series | Memory optimized    | In-memory DBs |
| F-series | Compute optimized   | CPU-heavy workloads |
| M-series | Large memory        | Enterprise DBs |
| L-series | Storage optimized   | Big data processing |
| N-series | GPU                 | AI / graphics |

💡 **Key Point:**  
> First choose **family**, then choose **size**.

---

## 🔍 VM Naming Convention (Exam Favorite)

Example:
```
Standard_D2s_v5
```

Breakdown:

- **D** → Family (General purpose)
- **2** → Number of vCPUs
- **s** → Premium SSD support
- **v5** → Hardware generation

💡 **Key Point:**  
> VM names encode performance and capabilities.

---

## 📈 Scaling and Resiliency

### 🔁 Virtual Machine Scale Sets

**Definition:**  
Group of identical, load-balanced VMs.

**Features:**
- Automatic scaling (out/in)
- Centralized configuration
- Load balancing integration

💡 **Use Case:**  
> Applications with variable demand

---

### 🛡️ Virtual Machine Availability Sets

**Definition:**  
Improve resiliency within a region.

**Concepts:**

- **Update Domain**
  - VMs updated/rebooted together (planned maintenance)

- **Fault Domain**
  - VMs share hardware risks (power/network)

💡 **Goal:**  
> Avoid all VMs failing at the same time

---

## ⚠️ Availability Sets vs Availability Zones

- Availability Sets → protect within a datacenter
- Availability Zones → protect across datacenters

💡 **Exam Tip:**  
> Availability Zones are usually preferred (better isolation)

---

## 💰 Cost Note
- Availability Sets themselves are **free**
- You pay only for the VM instances

---

## 🎯 Exam Key Points

- VMs = **IaaS (you manage OS)**
- Use VMs for **full control / custom workloads**
- VM size = vCPU + RAM + Disk + Network
- **Scale Sets** = scaling + load balancing
- **Availability Sets** = fault + update isolation
- VM naming gives **technical details**

---

## 🧠 Quick Summary

| Topic                | Key Idea |
|---------------------|----------|
| VM                  | Full control server (IaaS) |
| Size                | Defines performance |
| Scale Sets          | Auto scaling |
| Availability Sets   | High availability |
| Naming              | Encodes specs |