# 📦 Azure Containers – Summary (AZ-900 relevant)

## 🧠 What are Containers?

- **Lightweight virtualization**
- Multiple containers run on **one host (VM or physical)**
- **No own operating system per container** (unlike VMs)
- Quickly startable, scalable and recoverable
- Ideal for **dynamic workloads**

👉 Important difference to VMs:
- VM = own OS + more overhead  
- Container = share OS + very efficient

---

## ⚖️ Container vs. Virtual Machines

| Feature              | Virtual Machine            | Container                    |
|---------------------|--------------------------|------------------------------|
| Operating System    | Own OS per VM             | Shared host OS               |
| Startup Time        | Slow                      | Very fast                    |
| Resource Consumption| High                      | Low                          |
| Scaling             | Cumbersome                | Very flexible                |

👉 **Exam Key Point:**  
Container = **lighter weight + faster + more scalable**

---

## ☁️ Azure Container Services (important for the exam!)

### 🚀 Azure Container Instances (ACI)
- Fastest entry
- **No VM management**
- **PaaS**
- For simple / short-term workloads

👉 Use Case:
- Small apps, jobs, tests

---

### ⚙️ Azure Container Apps
- Building on containers
- **Auto-scaling + load balancing integrated**
- Also **PaaS**
- For modern apps without infrastructure effort

👉 Use Case:
- Microservices, APIs, web-apps

---

### 🧩 Azure Kubernetes Service (AKS)
- **Container orchestration (very important!)**
- Manages:
  - Deployment
  - Scaling
  - Networking
- More complex, but very powerful

👉 Use Case:
- Large, distributed systems
- Enterprise / microservices

---

## 🏗️ Orchestration (exam relevant!)

- Means: **Management of many containers**
- Tasks:
  - Start/Stop
  - Scaling
  - Load Balancing
  - Self-Healing

👉 In Azure: **AKS**

---

## 🧱 Typical Usage: Microservices

- Application is divided into **small, independent services**:
  - Frontend
  - Backend
  - Database

### Advantages:
- Independently deployable
- Separately scalable
- Better maintainability

---

## 🎯 When to use Containers?

- If you:
  - want to **scale quickly**
  - want to **deploy flexibly**
  - use **microservices architecture**
  - want to use resources efficiently

---

## 🧪 Exam-relevant Core Points

- Container ≠ VM (lighter weight, no own OS)
- **Docker** is a common container standard
- **ACI = simple & fast**
- **Container Apps = PaaS + Scaling**
- **AKS = Orchestration**
- Microservices are a typical use case

---

## 🧠 Mnemonic for the Exam

> **ACI = start quickly**  
> **Container Apps = scale easily**  
> **AKS = orchestrate complexly**
---
### Navigation
- [Parent: Module Overview](README.md)
- [Previous: Azure Virtual Desktop (AVD)](20_azure_virtual_desktop.md)
- [Next: ⚡ Azure Functions – Summary (AZ-900 relevant)](40_azure_functions.md)
- [Home](../../../README.md)

