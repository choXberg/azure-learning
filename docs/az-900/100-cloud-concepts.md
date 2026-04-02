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

| Modell        | Kontrolle | Kosten  | Skalierbarkeit | Typisch für            |
| ------------- | --------- | ------- | -------------- | ---------------------- |
| Public Cloud  | gering    | niedrig | sehr hoch      | Startups, moderne Apps |
| Private Cloud | hoch      | hoch    | begrenzt       | Banken, Behörden       |
| Hybrid Cloud  | mittel    | mittel  | hoch           | Enterprise Migration   |

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

