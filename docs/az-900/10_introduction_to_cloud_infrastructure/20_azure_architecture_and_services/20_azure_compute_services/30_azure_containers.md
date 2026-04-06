# 📦 Azure Containers – Zusammenfassung (AZ-900 relevant)

## 🧠 Was sind Container?

- **Leichtgewichtige Virtualisierung**
- Mehrere Container laufen auf **einem Host (VM oder physisch)**
- **Kein eigenes Betriebssystem pro Container** (im Gegensatz zu VMs)
- Schnell startbar, skalierbar und wiederherstellbar
- Ideal für **dynamische Workloads**

👉 Wichtiger Unterschied zu VMs:
- VM = eigenes OS + mehr Overhead  
- Container = teilen sich OS + sehr effizient

---

## ⚖️ Container vs. Virtual Machines

| Feature              | Virtual Machine            | Container                    |
|---------------------|--------------------------|------------------------------|
| Betriebssystem      | Eigenes OS pro VM        | Gemeinsames Host-OS          |
| Startzeit           | Langsam                  | Sehr schnell                 |
| Ressourcenverbrauch | Hoch                     | Niedrig                      |
| Skalierung          | Schwerfälliger           | Sehr flexibel                |

👉 **Exam Key Point:**  
Container = **leichtgewichtiger + schneller + skalierbarer**

---

## ☁️ Azure Container Services (wichtig für Prüfung!)

### 🚀 Azure Container Instances (ACI)
- Schnellster Einstieg
- **Kein VM-Management**
- **PaaS**
- Für einfache / kurzfristige Workloads

👉 Use Case:
- Kleine Apps, Jobs, Tests

---

### ⚙️ Azure Container Apps
- Aufbauend auf Containern
- **Auto-Scaling + Load Balancing integriert**
- Ebenfalls **PaaS**
- Für moderne Apps ohne Infrastruktur-Aufwand

👉 Use Case:
- Microservices, APIs, Web-Apps

---

### 🧩 Azure Kubernetes Service (AKS)
- **Container-Orchestrierung (sehr wichtig!)**
- Verwaltet:
  - Deployment
  - Scaling
  - Networking
- Komplexer, aber sehr mächtig

👉 Use Case:
- Große, verteilte Systeme
- Enterprise / Microservices

---

## 🏗️ Orchestrierung (prüfungsrelevant!)

- Bedeutet: **Verwaltung vieler Container**
- Aufgaben:
  - Start/Stop
  - Skalierung
  - Load Balancing
  - Self-Healing

👉 In Azure: **AKS**

---

## 🧱 Typische Nutzung: Microservices

- Anwendung wird in **kleine, unabhängige Services** aufgeteilt:
  - Frontend
  - Backend
  - Datenbank

### Vorteile:
- Unabhängig deploybar
- Separat skalierbar
- Bessere Wartbarkeit

---

## 🎯 Wann verwendet man Container?

- Wenn du:
  - **schnell skalieren** willst
  - **flexibel deployen** möchtest
  - **Microservices Architektur** nutzt
  - Ressourcen effizient nutzen willst

---

## 🧪 Prüfungsrelevante Kernpunkte

- Container ≠ VM (leichtgewichtiger, kein eigenes OS)
- **Docker** ist ein gängiger Container-Standard
- **ACI = einfach & schnell**
- **Container Apps = PaaS + Scaling**
- **AKS = Orchestrierung**
- Microservices sind ein typischer Use Case

---

## 🧠 Merksatz für die Prüfung

> **ACI = schnell starten**  
> **Container Apps = einfach skalieren**  
> **AKS = komplex orchestrieren**
---
### Navigation
- [Parent: Module Overview](README.md)
- [Previous: Azure Virtual Desktop (AVD)](20_azure_virtual_desktop.md)
- [Next: ⚡ Azure Functions – Summary (AZ-900 relevant)](40_azure_functions.md)
- [Home](../../../README.md)

