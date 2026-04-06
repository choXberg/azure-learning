# 🌐 Azure Application Hosting Options – Summary (AZ-900 relevant)

## 🧠 Overview

Azure provides multiple ways to host applications:

- **Virtual Machines (VMs)** → Maximum control
- **Containers** → Flexible and lightweight
- **Azure App Service** → Fully managed (PaaS)

👉 Key idea:
- Trade-off between **control vs. operational effort**

---

## ⚖️ Hosting Spectrum (Exam Concept)

| Option        | Control        | Management Effort | Typical Use Case                |
|---------------|--------------|------------------|--------------------------------|
| Virtual Machines | High         | High             | Full customization             |
| Containers     | Medium       | Medium           | Microservices, portability     |
| App Service    | Low          | Low              | Web apps, APIs (fast setup)    |

👉 **Exam Key Point:**
- More control = more responsibility

---

## 🖥️ Virtual Machines (VMs)

- Full control over:
  - OS
  - Runtime
  - Configuration
- Familiar (like on-premises)

👉 Downsides:
- Requires **management and maintenance**

---

## 📦 Containers

- Lightweight and portable
- Isolate application components
- Easier scaling than VMs

👉 Often used for:
- Microservices architectures

---

## ⚙️ Azure App Service (Very Important!)

- **PaaS offering**
- No infrastructure management required
- Used for:
  - Web apps
  - REST APIs
  - Mobile back ends
  - Background jobs

👉 Key benefits:
- Automatic scaling
- High availability
- Built-in load balancing
- Continuous deployment (GitHub, Azure DevOps, Git)

---

## 🌍 Supported Technologies

- Languages & frameworks:
  - .NET / .NET Core
  - Java
  - Node.js
  - Python
  - PHP

- OS support:
  - Windows
  - Linux

---

## 🧩 Types of App Service

### 🌐 Web Apps
- Host websites and web applications
- Supports multiple frameworks

---

### 🔌 API Apps
- Host RESTful APIs
- Supports Swagger
- Can be published to Azure Marketplace

---

### ⚙️ WebJobs
- Run background tasks or scripts
- Can be:
  - Scheduled
  - Triggered

👉 Example:
- Data processing
- Scheduled jobs

---

### 📱 Mobile Apps
- Backend for mobile applications
- Features:
  - Cloud data storage
  - Authentication (Google, Facebook, etc.)
  - Push notifications

---

## 🎯 When to use what?

- **VMs**
  → Full control required

- **Containers**
  → Flexible, scalable architectures

- **App Service**
  → Fast, managed hosting for web apps & APIs

---

## 🧪 Exam-Relevant Key Points

- App Service = **PaaS for web apps & APIs**
- No infrastructure management
- Supports:
  - Auto-scaling
  - High availability
  - CI/CD
- WebJobs = background processing
- Mobile Apps = backend for mobile apps
- VM = most control, most effort
- Containers = balance between control and flexibility

---

## 🧠 Quick Memory Aid

> **VM = control**  
> **Containers = flexibility**  
> **App Service = simplicity**
---
### Navigation
- [Parent: Module Overview](README.md)
- [Previous: 🤖 Azure AI, Machine Learning, and IoT/Edge – Summary (AZ-900 relevant)](50_azure_ai_ml_iot_edge_services.md)
- [Next: 🌐 Azure Application Hosting Options – Summary (AZ-900 relevant)](README.md)
- [Home](../../../README.md)

