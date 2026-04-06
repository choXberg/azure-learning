# 🤖 Azure AI, Machine Learning, and IoT/Edge – Summary (AZ-900 relevant)

## 🧠 Overview

Azure provides services to build:
- **Intelligent solutions (AI & ML)**
- **Connected solutions (IoT & Edge)**

👉 Goal:
- Use **prebuilt services** or **custom models** depending on complexity

---

## 🤖 Azure AI Services

- **Prebuilt AI capabilities via APIs**
- No need to train models yourself

### Supported scenarios:
- Language (text analysis, translation)
- Speech (speech-to-text, text-to-speech)
- Vision (image recognition)
- Document processing

👉 **Azure OpenAI Service**
- Supports **generative AI**
  - Chat
  - Content generation
- Includes **security and governance controls**

---

## 🧩 Agentic AI (Important Concept)

- Combines:
  - AI models
  - Instructions
  - Context
  - Tool usage

👉 Used for:
- **Multi-step problem solving**

⚠️ Exam tip:
- Not a separate service
- It's an **application pattern** built using:
  - Azure AI Services
  - Azure OpenAI

---

## 🧪 Azure Machine Learning (Azure ML)

- Used to:
  - **Build**
  - **Train**
  - **Manage** custom ML models

👉 Best when:
- You need **full control over models**
- You perform:
  - Experiments
  - Model lifecycle management

---

## 🌐 IoT and Edge Services

### 🔌 Azure IoT Hub
- Central service for IoT communication
- Enables:
  - **Secure**
  - **Bi-directional communication**
  between devices and cloud

---

### 📊 Azure IoT Central
- **SaaS solution**
- Simplifies:
  - Device management
  - Monitoring

👉 Good for:
- Quick IoT solution deployment

---

### ⚡ Azure IoT Edge
- Runs workloads **closer to devices**
- Extends cloud capabilities to the edge

👉 Benefits:
- Lower latency
- Offline capabilities

---

## 🔄 Typical IoT Flow

1. Devices send telemetry → **IoT Hub**
2. Data processed in cloud (analytics, AI)
3. Insights/models sent back → **IoT Edge**
4. Local processing near devices

👉 IoT Central can manage the entire solution

---

## 🎯 Choosing the Right Service (Exam Key!)

### Decision Guide:

- **Azure AI Services**
  → Use **prebuilt AI via APIs**

- **Azure Machine Learning**
  → Use **custom models**

- **Azure IoT Services**
  → Use for **device connectivity & telemetry**

---

## 🧪 Exam-Relevant Key Points

- Azure AI Services = **ready-to-use AI APIs**
- Azure OpenAI = **generative AI**
- Agentic AI = **pattern, not a service**
- Azure ML = **custom ML models**
- IoT Hub = **device communication**
- IoT Central = **SaaS IoT platform**
- IoT Edge = **processing near devices**

---

## 🧠 Quick Memory Aid

> **AI Services = prebuilt AI**  
> **Azure ML = build your own models**  
> **IoT = connect devices**
---
### Navigation
- [Parent: Module Overview](README.md)
- [Previous: ⚡ Azure Functions – Summary (AZ-900 relevant)](40_azure_functions.md)
- [Next: 🌐 Azure Application Hosting Options – Summary (AZ-900 relevant)](60_azure_application_hosting_options.md)
- [Home](../../../README.md)

