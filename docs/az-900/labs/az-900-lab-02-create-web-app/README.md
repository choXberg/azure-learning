# Lab 02 – Create a Web App (Azure App Service)

## Overview

In this lab, an Azure App Service Web App was created using a **container-based deployment**.

The application was deployed from a public container image hosted in the **Microsoft Container Registry (MCR)**.

---

## What was done

- Created an **Azure Web App**
- Deployment type: **Container**
- Operating System: **Linux**
- Container source: **Public registry (MCR)**
- Image: `azuredocs/aci-helloworld`
- Tested the application via the **default domain URL**

---

## Key Concepts

### Azure App Service

Azure App Service is a **Platform as a Service (PaaS)** offering that allows you to host:

- Web apps
- REST APIs
- Background services

---

### Container-based Deployment

Instead of deploying code directly:

- A **container image** is used
- The image is pulled from a registry (here: MCR)
- Azure runs the container inside App Service

---

### Monitoring & Telemetry

Azure automatically provides basic metrics:

- Requests
- Data In / Out
- Response time

⚠️ Metrics may take time to appear and require traffic.

---

## Architecture Insight

- Resource Group location: **East US**
- Web App location: **Canada Central**

> Resource Groups are logical containers and do not define resource location.

---

## Exam Takeaways (AZ-900)

- Azure App Service = **PaaS**
- Supports **containerized applications**
- No infrastructure management required
- Resource Groups ≠ deployment region
- App Service Plan defines region

---

<details>
<summary>⚠️ Common Pitfalls</summary>

### ❌ Wrong Publish Type
Choosing **Code instead of Container**
→ No container configuration available

---

### ❌ Resource Group misconception
Assuming all resources must be in the same region

→ Incorrect

---

### ❌ Ignoring App Service Plan
Web App must match the region of the App Service Plan

---

### ❌ No telemetry visible
Usually:
- No traffic yet
- Metrics delay

---

### ❌ Non-unique app name
Web App names must be **globally unique**

</details>

---

## 🧪 Quiz

### Question 1
What type of cloud service is Azure App Service?

A) IaaS  
B) PaaS  
C) SaaS  

<details>
<summary>Show answer</summary>

**Answer:** B) PaaS

</details>

---

### Question 2
Can Azure App Service host containerized applications?

A) No  
B) Yes  

<details>
<summary>Show answer</summary>

**Answer:** B) Yes

</details>

---

### Question 3
Does the Resource Group location determine where resources are deployed?

A) Yes  
B) No  

<details>
<summary>Show answer</summary>

**Answer:** B) No

</details>

---

### Question 4
Must a Web App be in the same region as its App Service Plan?

A) Yes  
B) No  

<details>
<summary>Show answer</summary>

**Answer:** A) Yes

</details>

---

### Question 5
Why might you not see telemetry data immediately?

A) Azure is broken  
B) No requests were made or delay in metrics  

<details>
<summary>Show answer</summary>

**Answer:** B

</details>

---

### Question 6
What is required for a Web App name?

A) Unique per subscription  
B) Globally unique  
C) Unique per resource group  

<details>
<summary>Show answer</summary>

**Answer:** B

</details>

---

<details>
<summary>🧠 Deep Dive (Optional)</summary>

### App Service Plan

The App Service Plan defines:

- Region
- Pricing tier
- Compute resources

A Web App must always run in the same region as its App Service Plan.

---

### Resource Groups

Resource Groups:

- Are logical containers
- Store metadata
- Do NOT enforce region constraints

</details>

---

## Summary

- Azure App Service simplifies hosting (PaaS)
- Containers can be deployed easily
- Resource Groups are logical only
- App Service Plan defines region
- Monitoring is built-in but delayed