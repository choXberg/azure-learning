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

#### Benefits:
- No infrastructure management
- Built-in scaling
- Integrated monitoring
- Supports multiple runtimes and containers

---

### Container-based Deployment

Instead of deploying code directly:

- A **container image** is used
- The image is pulled from a registry (here: MCR)
- Azure runs the container inside App Service

---

### Linux Support

Azure App Service supports:

- Windows
- Linux (used in this lab)

---

### Default Domain

After deployment, each Web App gets a URL:

```
https://<app-name>.azurewebsites.net
```


This is used to test the application.

---

### Monitoring & Telemetry

Azure automatically provides basic metrics:

- Requests
- Data In / Out
- Response time

⚠️ Metrics may take time to appear and require traffic.

---

## Important Architecture Insight

### Resource Group vs Resource Location

- Resource Group location: **East US**
- Web App location: **Canada Central**

#### Key rule:

> Resource Groups are logical containers and do not define resource location.

---

### App Service Plan Dependency

- Web App must be in the same region as the **App Service Plan**
- The plan defines:
  - Region
  - Pricing tier
  - Compute resources

---

## Exam Takeaways (AZ-900)

- Azure App Service = **PaaS**
- App Service supports **containers**
- No need to manage OS or infrastructure
- Resource Groups ≠ deployment region
- Resources define their own region
- Some services require **regional alignment** (App Service Plan)

---

## Common Pitfalls (Very Important)

### ❌ Pitfall 1: Wrong Publish Type
Choosing **Code instead of Container**
→ No container configuration available

---

### ❌ Pitfall 2: Assuming Resource Group defines region
Wrong assumption:
> "All resources must be in the same region as the Resource Group"

Correct:
→ Resources can be in different regions

---

### ❌ Pitfall 3: Ignoring App Service Plan
Trying to set a different region for the Web App

→ Not possible if a plan already exists

---

### ❌ Pitfall 4: No telemetry visible
Thinking monitoring is broken

→ Usually:
- No traffic yet
- Metrics delay

---

### ❌ Pitfall 5: Non-unique app name
Web App names must be **globally unique**

---

## Mini Quiz

### Question 1
What type of cloud service is Azure App Service?

A) IaaS  
B) PaaS  
C) SaaS  

**Answer:** B) PaaS

---

### Question 2
Can Azure App Service host containerized applications?

A) No  
B) Yes  

**Answer:** B) Yes

---

### Question 3
Does the Resource Group location determine where resources are deployed?

A) Yes  
B) No  

**Answer:** B) No

---

### Question 4
Must a Web App be in the same region as its App Service Plan?

A) Yes  
B) No  

**Answer:** A) Yes

---

### Question 5
Why might you not see telemetry data immediately?

A) Azure is broken  
B) No requests were made or delay in metrics  

**Answer:** B

---

### Question 6
What is required for a Web App name?

A) Unique per subscription  
B) Globally unique  
C) Unique per resource group  

**Answer:** B

---

## Summary

- Azure App Service simplifies hosting (PaaS)
- Containers can be deployed easily
- Resource Groups are logical only
- App Service Plan defines region
- Monitoring is built-in but delayed
