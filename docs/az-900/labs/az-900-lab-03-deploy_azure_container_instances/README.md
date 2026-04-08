# Lab 03 – Deploy Azure Container Instances (ACI)

## Overview

In this lab, a containerized web application was deployed using **Azure Container Instances (ACI)**.

The container runs a simple "Welcome to ACI" web page and is exposed via a public DNS endpoint.

---

## What was done

- Created an **Azure Container Instance**
- Used a public container image from **Microsoft Container Registry (MCR)**
- Configured:
  - Container name
  - Region
  - OS (Linux)
- Assigned a **public DNS name**
- Exposed the container over HTTP (port 80)
- Verified deployment via browser

---

## Configuration Summary

| Setting | Value |
|--------|------|
| Container name | mycontainer |
| Region | East US |
| Image source | Other registry |
| Image | mcr.microsoft.com/azuredocs/aci-helloworld |
| OS | Linux |
| DNS name label | mycontainerdnsxxxxx |

---

## Key Concepts

### Azure Container Instances (ACI)

:contentReference[oaicite:0]{index=0} is a service that allows you to:

- Run containers without managing virtual machines
- Deploy containers quickly
- Pay only for what you use

---

### Public Access via FQDN

Each container can be exposed via a public URL:

```
http://<dns-name>.<region>.azurecontainer.io
```

Example:
```
http://mycontainerdns12345.eastus.azurecontainer.io
```
---

### Lightweight Container Hosting

ACI is ideal when you need:

- Fast startup
- No orchestration
- Minimal configuration

---

## Exam Takeaways (AZ-900)

- ACI enables **container execution without infrastructure management**
- No Kubernetes required
- Supports **public IP and DNS**
- Charged based on **usage (CPU + memory)**
- Ideal for **short-lived or simple workloads**

---

<details>
<summary>⚠️ Common Pitfalls</summary>

### ❌ DNS name not unique
Deployment fails if DNS label already exists

---

### ❌ Container not reachable
Cause:
- No public DNS configured
- Port not exposed

---

### ❌ Confusing ACI with AKS
ACI:
- Single containers
- No orchestration

AKS:
- Full Kubernetes cluster

---

### ❌ Logs enabled unnecessarily
Logs can be disabled (as in this lab)

</details>

---

## 🧪 Quiz

### Question 1
What is Azure Container Instances primarily used for?

A) Managing virtual machines  
B) Running containers without managing infrastructure  
C) Hosting relational databases  

<details>
<summary>Show answer</summary>

**Answer:** B

</details>

---

### Question 2
Does Azure Container Instances require Kubernetes?

A) Yes  
B) No  

<details>
<summary>Show answer</summary>

**Answer:** B

</details>

---

### Question 3
What must be globally unique when exposing a container publicly?

A) Container name  
B) DNS name label  
C) Resource group  

<details>
<summary>Show answer</summary>

**Answer:** B

</details>

---

### Question 4
What is the purpose of the FQDN?

A) Internal communication  
B) Public access to the container  
C) Monitoring  

<details>
<summary>Show answer</summary>

**Answer:** B

</details>

---

### Question 5
What kind of workloads is ACI best suited for?

A) Large enterprise ERP systems  
B) Short-lived or simple container workloads  
C) Long-running VM workloads  

<details>
<summary>Show answer</summary>

**Answer:** B

</details>

---

<details>
<summary>🧠 Deep Dive</summary>

### ACI vs App Service vs AKS

- **ACI**
  - Fast, simple container execution
  - No orchestration
  - Ideal for short-lived workloads

- **App Service**
  - PaaS for web apps
  - Supports containers
  - Built-in scaling

- **AKS (Azure Kubernetes Service)**
  - Full orchestration platform
  - Complex, scalable systems

---

### Restart Policy (Important Concept)

Typical options:

- Always → container restarts automatically
- OnFailure → restarts only on failure
- Never → runs once

</details>

---

## Summary

- ACI allows running containers without managing infrastructure
- Public access via DNS is easy to configure
- No orchestration required
- Ideal for lightweight and temporary workloads