# Summary – Introduction to Cloud Infrastructure

## ☁️ Cloud Concepts

* Cloud computing delivers IT resources over the internet
* Pay-as-you-go (OpEx instead of CapEx)
* Benefits:

  * Scalability
  * Flexibility
  * Cost efficiency

### Cloud Models

* Public: shared infrastructure
* Private: dedicated environment
* Hybrid: combination of both

### Shared Responsibility Model

* Azure: physical infrastructure
* Customer: data, access, configuration

---

## 🏗️ Azure Architecture

### Physical Infrastructure

* Datacenter → Availability Zone → Region → Geography

### Availability Zones

* Provide high availability
* Protect against datacenter failures

---

## ⚙️ Compute Services

* Virtual Machines → full control (IaaS)
* Containers → lightweight, portable
* Azure Functions → serverless, event-driven
* App Service → managed hosting platform

---

## 🌐 Networking

* Virtual Network (VNet): private network in Azure
* VPN: encrypted connection over internet
* ExpressRoute: private dedicated connection
* DNS: domain name resolution

---

## 💾 Storage

* Blob Storage: unstructured data
* File Storage: shared file system
* Queue Storage: messaging
* Table Storage: NoSQL data

### Redundancy Options

* LRS, ZRS, GRS, GZRS

---

## 📊 Management & Governance

### Cost Management

* Pricing Calculator
* Azure Cost Management
* Tags for cost tracking

### Governance

* Azure Policy
* Resource Locks
* Microsoft Purview

### Monitoring

* Azure Monitor → metrics + logs
* Azure Advisor → recommendations
* Service Health → outages

---

## 🛠️ Tools

* Azure Portal (GUI)
* Azure CLI / PowerShell (automation)
* ARM Templates (infrastructure as code)
* Azure Arc (hybrid/multi-cloud)

---

## 🎯 Key Takeaways

* Azure provides scalable, global infrastructure
* Services are categorized (compute, networking, storage)
* Governance and monitoring are essential
* Choose services based on use case, not just technology
