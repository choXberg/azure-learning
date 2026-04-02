# 🌐 Public Cloud

## Definition:
Cloud-Ressourcen werden von einem Anbieter bereitgestellt und von vielen Kunden gemeinsam genutzt.

Beispiele:

- Microsoft Azure
- Amazon Web Services
- Google Cloud Platform

## Merkmale:

- Infrastruktur gehört dem Anbieter
- Zugriff über Internet
- Pay-as-you-go 💸
- Hoch skalierbar

## Vorteile:

- Kein Hardware-Aufwand
- Schnell startklar
- Sehr flexibel

## Nachteile:

- Weniger Kontrolle
- Datenschutz/Compliance kann Thema sein

👉 Praxis: Das ist das, was du mit Azure lernst.


# 🏢 Private Cloud

## Definition:
Cloud-Infrastruktur wird nur von einer Organisation genutzt.

Kann sein:

im eigenen Rechenzentrum (on-premise)
oder dediziert bei einem Anbieter

## Merkmale:

Volle Kontrolle 🔒
- Eigene Hardware / dedizierte Ressourcen
- Höhere Sicherheit (theoretisch)

## Vorteile:

- Maximale Kontrolle
- Gut für sensible Daten

## Nachteile:

- Teuer 💸💸
- Wartung & Betrieb selbst
- Weniger flexibel

👉 Praxis: Klassische Unternehmens-IT oder Banken.

# 🔀 Hybrid Cloud

## Definition:
Kombination aus Private Cloud + Public Cloud

Beispiel:

Datenbank bleibt on-premise
Web-App läuft in Microsoft Azure

## Merkmale:

Verbindung zwischen beiden Welten (VPN / ExpressRoute)
Daten können flexibel verschoben werden

## Vorteile:

Beste aus beiden Welten
Sensible Daten bleiben intern
Skalierung über Cloud möglich

## Nachteile:

Komplexer 🧠
Netzwerk + Security anspruchsvoller

👉 Praxis: Sehr häufig in Unternehmen (auch bei Migration Richtung Cloud)

# 🌍 Multicloud

## Definition:
Ein Unternehmen nutzt mehrere Public-Cloud-Anbieter gleichzeitig.

## 👉 Beispiel:

- Backend läuft auf Amazon Web Services
- AI/Analytics läuft auf Microsoft Azure
- Datenanalyse evtl. auf Google Cloud Platform

# Kurzvergleich:

| Feature              | Public Cloud                                       | Private Cloud                                           | Hybrid Cloud                                           | Multi-Cloud                            |
| -------------------- | -------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------ | -------------------------------------- |
| **Definition**       | Cloud services offered over the internet to anyone | Cloud infrastructure dedicated to a single organization | Combination of public + private cloud with integration | Use of multiple cloud providers        |
| **Ownership**        | Cloud provider (e.g. Microsoft, Amazon)            | Single organization                                     | Shared (organization + provider)                       | Multiple providers                     |
| **Accessibility**    | Public (via internet)                              | Private (restricted access)                             | Both public and private                                | Depends on each provider               |
| **Cost Model**       | Pay-as-you-go                                      | High upfront + maintenance                              | Mixed                                                  | Mixed                                  |
| **Control**          | Low (provider-managed)                             | High (full control)                                     | Medium                                                 | Medium                                 |
| **Scalability**      | Very high                                          | Limited                                                 | High (can burst to public cloud)                       | Very high                              |
| **Security**         | Standardized, provider-managed                     | Highest control, customizable                           | Flexible                                               | Depends on setup                       |
| **Typical Use Case** | Web apps, startups, scalable workloads             | Sensitive data, compliance, legacy systems              | Gradual migration, data separation                     | Vendor independence, risk distribution |
| **Example Scenario** | Hosting a website in Azure                         | Internal company datacenter                             | Database on-prem + app in cloud                        | App split across Azure + AWS           |


# 🔗 Azure Arc

## 🌍 Grundidee

Azure Arc ermöglicht dir:

- 👉 Ressourcen außerhalb von Azure so zu verwalten, als wären sie in Azure

## 🧠 In einem Satz (wichtig!)

👉 Azure Arc erweitert Azure auf andere Umgebungen

## Normalerweise:

Azure verwaltet nur Ressourcen in Azure

Mit Azure Arc:

du kannst auch verwalten:
- 🖥️ On-Prem Server
- ☁️ andere Clouds (z. B. AWS, GCP)
- ☸️ Kubernetes Cluster

👉 und zwar zentral über das Azure Portal

## 🔥 Merksatz 

👉 Azure Arc = Azure Management für alles, egal wo es läuft

# Azure VMware Solution (AVS)

## 👉 Infrastruktur-Service

VMware läuft direkt in Azure

Du bekommst:
- vSphere
- vSAN
- NSX

### 👉 Lift & Shift ohne Umbau

Typische Nutzung:

- Migration bestehender VMware-Workloads
- Legacy-Systeme unverändert weiter betreiben

👉 AVS = „Ich verschiebe meine VMware-Umgebung nach Azure“


### 🔥 Merksätze (prüfungsreif)
- Azure Arc = Manage everything
- Azure VMware Solution = Run VMware in Azure

## Azure Arc vs. Azure VMWare Solution
| Thema      | Azure Arc           | Azure VMware Solution |
| ---------- | ------------------- | --------------------- |
| Zweck      | Management          | Infrastruktur         |
| Ressourcen | bleiben wo sie sind | laufen in Azure       |
| Migration  | ❌ nein              | ✅ ja                  |
| Fokus      | Kontrolle           | Betrieb               |

## 💪 Fazit

- 👉 Arc = Kontrolle
- 👉 AVS = Migration + Betrieb


# 💰 Consumption-Based Model

## 📚 Source
Microsoft Learn – Describe the consumption-based model

---

## 🧠 Summary

- Pay only for what you use (pay-as-you-go)
- No upfront costs
- Resources can scale dynamically
- Costs depend on usage (compute, storage, network)

---

## 🔑 Key Concepts

- CapEx vs OpEx
- Scalability
- Elasticity
- Metered billing

---

## 🧪 Example

A Web API hosted in Azure App Service:

- Low traffic → low cost
- High traffic → scales automatically → higher cost

---

## ⚖️ Pros & Cons

### ✅ Pros
- No upfront investment
- Flexible scaling
- Cost-efficient for variable workloads

### ❌ Cons
- Harder to predict costs
- Requires monitoring
- Risk of unexpected charges

---

## 🔗 Related Topics

- Cloud pricing models
- Azure Cost Management
- Scaling in Azure

---

## ❓ Questions / Open Points

- How to estimate costs reliably?
- Which services are most cost-sensitive?

---

## 💡 Was ich mitgenommen habe

- Important for designing scalable backend systems
- Must monitor usage → otherwise cost risk

---
# Hochverfügbarkeit


## ⬆️ Vertikale Skalierung (Scale Up)
4

👉 Ein System stärker machen

- mehr CPU
- mehr RAM
- bessere Maschine

#### Vertikal → wenn es einfach bleiben soll

Typische Fälle:

- kleine Anwendung
- Monolith
- Datenbank (sehr häufig!)
- schneller Fix („mehr Power geben“)

👉 Beispiel:

deine API wird langsam → mehr RAM → fertig

## Horizontale Skalierung (Scale Out)

👉 Mehr Instanzen hinzufügen

- mehrere Server
- Load Balancer davor
- verteilt Last

#### Horizontal → wenn du skalieren MUSST

Typische Fälle:

- viele User
- Cloud-native Apps
- Microservices
- hohe Verfügbarkeit

👉 Beispiel:

Web API bekommt viel Traffic → mehrere Instanzen

---

# ☁️ Sicherheit und Governance

| Modell | Wer macht mehr? |
| ------ | --------------- |
| IaaS   | du              |
| PaaS   | geteilt         |
| SaaS   | Anbieter        |


👉 Das gilt auch für Security & Governance


# 🏗️ IaaS – Infrastructure as a Service

## 🔐 Sicherheit

👉 Du bist stark verantwortlich

## Vorteile:

volle Kontrolle über:
- OS
- Netzwerk
- Firewall
- kannst eigene Security-Tools einsetzen

👉 gut für spezielle Anforderungen

## 📋 Governance

👉 sehr flexibel, aber auch viel Arbeit

### Vorteile:

- eigene Policies möglich
- komplette Kontrolle über Architektur
- individuell anpassbar

### ⚠️ Nachteil (wichtig!)
- hoher Aufwand
- viele Fehlerquellen

# ⚙️ PaaS – Platform as a Service
## 🔐 Sicherheit

👉 geteilte Verantwortung

## Vorteile:

- OS wird vom Anbieter gepatcht
- integrierte Security (z. B. TLS, Identity)
- weniger Angriffsfläche

👉 du fokussierst dich auf Code

## 📋 Governance

### Vorteile:

- einfache Integration mit Azure Policies
- standardisierte Umgebung
- weniger Chaos als IaaS
- ⚠️ Nachteil
- weniger Kontrolle als IaaS
- 🧩 SaaS – Software as a Service

## 🔐 Sicherheit

👉 Anbieter macht fast alles

## Vorteile:

- automatische Updates
- Security komplett gemanagt
- minimaler Aufwand für dich

## 📋 Governance

### Vorteile:

- einfache Benutzer- und Zugriffssteuerung
- Compliance oft bereits integriert
- schnelle Nutzung ohne Setup
- ⚠️ Nachteil
- wenig Einfluss
- eingeschränkte Anpassbarkeit

### 🧠 Vergleich 

| Modell | Sicherheit                               | Governance                     |
| ------ | ---------------------------------------- | ------------------------------ |
| IaaS   | maximal flexibel, aber du verantwortlich | volle Kontrolle, hoher Aufwand |
| PaaS   | sicher + weniger Aufwand                 | standardisiert + integriert    |
| SaaS   | maximal einfach                          | stark vorgegeben               |


👉 Je höher der Service, desto weniger musst du sichern und steuern


---
# Management of the cloud

## Management of the cloud speaks to managing your cloud resources. In the cloud, you can:

- Automatically scale resource deployment based on need.
- Deploy resources based on a preconfigured template, removing the need for manual configuration.
- Monitor the health of resources and automatically replace failing resources.
- Receive automatic alerts based on configured metrics, so you're aware of performance in real time.

---

## ☁️ Management in the Cloud

Cloud management refers to how you create, configure, monitor, and maintain cloud resources.

There are four primary ways to manage cloud environments:

- Web Portal (GUI)
- Command Line Interface (CLI)
- PowerShell
- APIs

## 🌐 1. Web Portal (GUI)

Example: Microsoft Azure Portal

Characteristics:

- Graphical user interface (browser-based)
- Beginner-friendly and intuitive
- No programming required

### Advantages:

- Easy to learn and explore
- Visual feedback
- Good for quick configuration

### Disadvantages:

- Not suitable for automation
- Hard to repeat tasks consistently
- Slower for large-scale operations

#### 👉 Typical use case:
- Initial setup
- exploration
- troubleshooting

---

## 💻 2. Command Line Interface (CLI)

CLI = general concept of text-based interaction

### Examples:

- Azure CLI
- Bash (Linux shell)
- CMD (Windows)

### Characteristics:

- Managed via terminal commands
- Scriptable and automatable
- Cross-platform

### Example (Azure CLI):

```
az group create --name myRG --location westeurope
```

### Advantages:

- Fast and efficient
- Ideal for automation and CI/CD
- Repeatable processes

### Disadvantages:

- Steeper learning curve
- Less visual feedback

#### 👉 Typical use case:
Automation, deployments, scripting

---

## ⚡ 3. PowerShell

PowerShell is a shell and scripting language developed by Microsoft.

### Characteristics:

- Object-based (.NET objects instead of plain text)
- Strong integration with Microsoft ecosystem
- Uses Verb-Noun command structure

### Example:

```
New-AzResourceGroup -Name myRG -Location westeurope
```

### Advantages:

- Powerful automation capabilities
- Works with structured objects
- Well-suited for Microsoft environments

### Disadvantages:

- Less common outside Microsoft ecosystem
- Can be more complex than CLI

### 👉 Typical use case:

- Administration
- advanced automation
- Microsoft-centric environments

---
## 🔌 4. APIs

Cloud providers expose REST APIs for resource management.

### Characteristics:

- Direct programmatic access
- HTTP-based (REST)

Example (simplified):

```
POST https://management.azure.com/subscriptions/{id}/resourceGroups
```

### Advantages:

- Maximum flexibility
- Foundation of all other tools (Portal, CLI, PowerShell)

### Disadvantages:

- More complex to use directly
- Requires handling authentication and requests

### 👉 Typical use case:
- Custom 
- tools
- integrations
- SDK development

---
## ⚖️ Comparison: CLI vs PowerShell vs Bash

### 🧠 Core Concepts

| Concept    | Description                                |
| ---------- | ------------------------------------------ |
| CLI        | General term for command-line interaction  |
| Bash       | Traditional Unix/Linux shell (text-based)  |
| PowerShell | Object-oriented shell + scripting language |
| Azure CLI  | Tool to manage Azure resources             |

### 🔍 Key Differences

| Feature  | Bash              | PowerShell          | Azure CLI               |
| -------- | ----------------- | ------------------- | ----------------------- |
| Type     | Shell             | Shell + Language    | Tool                    |
| Platform | Linux/macOS       | Cross-platform      | Cross-platform          |
| Output   | Text              | Objects (.NET)      | JSON                    |
| Syntax   | Unix-style        | Verb-Noun           | `az <service> <action>` |
| Focus    | System operations | Microsoft ecosystem | Azure                   |

## 🔄 How They Work Together

### 👉 Important for exams:

- Azure CLI runs inside Bash, PowerShell, or CMD
- PowerShell can execute Azure CLI commands

### Example:

```
az vm list
```

### 👉 PowerShell simply invokes Azure CLI here.

---
## 🧪 Exam-Relevant Key Points

### ✅ Portal

Easy but not automatable

### ✅ CLI

Fast, scriptable, ideal for DevOps

### ✅ PowerShell

Powerful, object-based, Microsoft-focused

### ✅ APIs

Underlying foundation of all management methods

---

## Underlying foundation of all management methods

### 🚀 Summary
- Multiple ways exist to manage cloud resources
- The choice depends on:
- Level of automation
- Complexity
- Environment

### 👉 In practice, they are often combined:

- Portal → learning and quick tasks
- CLI / PowerShell → automation
- APIs → integration and advanced scenarios

---

## Describe sustainability considerations in the cloud

Cloud computing can support sustainability goals when teams actively optimize how resources are deployed and used.

### Why cloud can improve efficiency
Cloud providers operate at large scale, which can improve resource utilization compared to many isolated on-premises environments. In Azure, you can also reduce waste by matching deployed resources to actual demand.

### Sustainability-aligned cloud practices
Examples of practices that support sustainability and cost efficiency include:

- Scaling resources down when demand decreases
- Turning off or deallocating resources that are not in use
- Choosing efficient services and configurations to reduce overprovisioning
- Using governance and monitoring to track usage trends and optimize deployments over time

For example, a development environment that runs only during business hours can be automatically shut down overnight and on weekends. This practice reduces unnecessary consumption while still meeting team needs.

At a fundamentals level, sustainability in the cloud is closely tied to good operational habits: 
- right-size
- automate
- monitor
- continuously optimize.

