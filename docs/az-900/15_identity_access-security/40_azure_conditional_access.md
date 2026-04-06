# 🔐 Azure Conditional Access (AZ-900)

## 🧠 Überblick
- **Conditional Access** = Zugriff basierend auf Bedingungen steuern
- Teil von Microsoft Entra ID
- Ziel:
  - Sicherheit erhöhen
  - Benutzerfreundlichkeit erhalten

👉 Prinzip:
**„If → Then“ (Wenn Bedingung erfüllt → dann Aktion)**

---

## 🔍 Wie funktioniert Conditional Access?

### 1️⃣ Signale (Signals)
Während des Logins werden Informationen gesammelt:

- 👤 Wer? (User / Rolle)
- 📍 Wo? (Standort)
- 💻 Gerät (managed / unmanaged)
- 📱 Anwendung

---

### 2️⃣ Entscheidung (Decision)
Basierend auf den Signalen:

- Zugriff erlauben
- Zugriff blockieren
- MFA verlangen

---

### 3️⃣ Durchsetzung (Enforcement)
Aktion wird umgesetzt:

- ✅ Allow (Zugriff erlauben)
- 🔐 Require MFA
- ❌ Block

---

## 🔄 Ablauf (Flow)
User Login
↓
Signale sammeln (User, Location, Device)
↓
Policy prüfen
↓
Aktion:
→ Allow
→ Require MFA
→ Block


---

## ⚙️ Typische Szenarien

### 🔐 MFA abhängig von Bedingungen
- Admin → immer MFA
- Externer Zugriff → MFA

---

### 📱 Zugriff nur über erlaubte Apps
- Nur bestimmte Clients erlaubt (z. B. Outlook App)

---

### 💻 Zugriff nur von sicheren Geräten
- Nur **managed / compliant devices**

---

### 🚫 Blockieren von Risiken
- Unbekannte Standorte
- Verdächtige Login-Versuche

---

## 🎯 Beispiele

- Login aus Büro → ✅ Zugriff ohne MFA  
- Login aus anderem Land → 🔐 MFA erforderlich  
- Login von unsicherem Gerät → ❌ Zugriff blockiert  

---

## 🧠 Vorteile

- Granulare Zugriffskontrolle
- Höhere Sicherheit
- Flexible Policies
- Bessere User Experience (nicht immer MFA nötig)

---

## 🎯 Prüfungsrelevante Kernaussagen

- Conditional Access = **regelbasierter Zugriff**
- Entscheidungen basieren auf:
  - User
  - Location
  - Device
  - App
- Aktionen:
  - Allow
  - Require MFA
  - Block
- MFA kann **dynamisch** erzwungen werden
- Wichtig für:
  - Zero Trust Security

---

## 🧠 Merksatz

👉 **„Zugriff nur unter den richtigen Bedingungen.“**
---
### Navigation
- [Parent: Module Overview](README.md)
- [Previous: 🧠 External Identities – Eselsbrücken & Prüfungs-Shortcut (AZ-900)](35_azure_external_identities_shortcut.md)
- [Next: 🔐 Azure Role-Based Access Control (RBAC)](50_azure_role_based_access_control.md)
- [Home](../README.md)

