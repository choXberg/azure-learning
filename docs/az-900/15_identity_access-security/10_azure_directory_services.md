# 📘 Azure Directory Services (AZ-900)

## 🧠 Überblick: Microsoft Entra ID
- Microsoft Entra ID = Cloud-basierter Identity & Access Management Service (IAM)
- Ermöglicht:
  - Anmeldung (Login) bei Microsoft Cloud-Diensten (Azure, M365)
  - Zugriff auf eigene (custom) Anwendungen
- Vergleich zu On-Prem:
  - Ähnlich wie Active Directory
  - Unterschied: Microsoft betreibt & skaliert die Infrastruktur global

---

## 👥 Wer nutzt Microsoft Entra ID?
- IT-Administratoren
  - Steuern Zugriff auf Ressourcen & Apps
- Entwickler
  - Implementieren Authentifizierung (z. B. SSO)
- Benutzer
  - Self-Service (z. B. Passwort zurücksetzen)
- Cloud-Kunden
  - Automatisch genutzt bei:
    - Azure
    - Microsoft 365
    - Dynamics

---

## ⚙️ Hauptfunktionen

### 🔐 Authentication (Authentifizierung)
- Identitätsprüfung vor Zugriff
- Features:
  - Multi-Factor Authentication (MFA)
  - Self-Service Password Reset
  - Smart Lockout
  - Passwort-Richtlinien

---

### 🔑 Single Sign-On (SSO)
- Ein Login → Zugriff auf mehrere Anwendungen
- Vorteile:
  - Benutzerfreundlichkeit
  - Sicherheit

---

### 📦 Application Management
- Verwaltung von Apps (Cloud & On-Prem)
- Beispiele:
  - SaaS-Integration
  - Application Proxy
  - „My Apps“-Portal

---

### 💻 Device Management
- Geräte registrieren & verwalten (z. B. via Intune)
- Conditional Access:
  - Zugriff nur von bekannten/vertrauenswürdigen Geräten

---

## 🔗 Verbindung mit On-Prem Active Directory

### Problem:
- Ohne Verbindung:
  - Zwei getrennte Identitäten (Cloud + On-Prem)

### Lösung:
- Microsoft Entra Connect
  - Synchronisiert Benutzer zwischen:
    - On-Prem AD
    - Microsoft Entra ID

### Vorteile:
- Einheitliche Identität
- SSO über Cloud & On-Prem
- MFA & Self-Service überall nutzbar

---

## 🏢 Microsoft Entra Domain Services

### 📌 Was ist das?
- Bietet klassische AD-Funktionen ohne eigene Domain Controller

### Unterstützt:
- Domain Join
- Group Policy
- LDAP
- Kerberos / NTLM

---

### 🎯 Wann verwenden?
- Für Legacy-Anwendungen, die:
  - kein modernes Auth unterstützen
- „Lift & Shift“ Szenarien:
  - Alte Apps in die Cloud migrieren

---

### ⚙️ Funktionsweise
- Azure erstellt:
  - 2 gemanagte Domain Controller (Replica Set)
- Kein Aufwand für:
  - Patchen
  - Wartung
  - Konfiguration

➡️ Alles wird von Azure gemanagt (inkl. Backup & Verschlüsselung)

---

## 🔄 Synchronisation

### 🔁 Richtung:
- Einweg-Sync:
  - Entra ID → Domain Services

### Hybrid-Szenario:
On-Prem AD
↓ (Entra Connect)
Microsoft Entra ID
↓ (automatisch)
Domain Services


### Wichtig:
- Änderungen in Domain Services:
  - ❌ werden NICHT zurück synchronisiert

---

## 🧩 Nutzung in Azure
- VMs, Apps & Services können:
  - Domain Join durchführen
  - Authentifizierung nutzen (LDAP, Kerberos)
  - Gruppenrichtlinien anwenden

---

# 🎯 Prüfungsrelevante Kernaussagen

- Microsoft Entra ID = zentrale Identity-Lösung in Azure
- SSO = ein Login für viele Anwendungen
- MFA erhöht Sicherheit
- Entra Connect = Verbindung On-Prem ↔ Cloud
- Domain Services = AD ohne Domain Controller verwalten
- Synchronisation Domain Services = nur One-Way
- Ideal für Legacy Apps in der Cloud