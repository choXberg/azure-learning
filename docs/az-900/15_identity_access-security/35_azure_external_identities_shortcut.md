# 🧠 External Identities – Eselsbrücken & Prüfungs-Shortcut (AZ-900)

## 🧩 Die 3 Modelle einfach merken

### 🤝 B2B Collaboration → „Bring them in“
- Externe Nutzer kommen **in deinen Tenant**
- Werden als **Guest User** angelegt
- Zugriff auf deine Apps & Ressourcen

💡 Bild:
> „Externer bekommt einen Besucherausweis für mein Büro“

---

### 🔗 B2B Direct Connect → „Stay where you are“
- Externe bleiben **in ihrem eigenen Tenant**
- Kein Guest User notwendig
- Direkte Verbindung zwischen Tenants (Trust)

💡 Bild:
> „Wir arbeiten zusammen, aber jeder bleibt in seinem eigenen Büro“

---

### 👥 B2C (External ID for Customers) → „Build for customers“
- Für **Kunden / Endnutzer**
- Eigene Apps (SaaS / Custom Apps)
- Eigener separater Tenant

💡 Bild:
> „Ich betreibe einen Shop für Kunden“

---

## 🚀 Super-Merksätze

- **B2B → Gast im eigenen Tenant**
- **Direct Connect → Verbindung ohne Gast**
- **B2C → Kunden & externe Nutzer (separat)**

---

## ⚡ 5-Sekunden-Prüfungs-Shortcut

| Frage | Richtige Antwort |
|------|-----------------|
| Externer User greift auf meine App zu | **B2B Collaboration** |
| Zwei Firmen arbeiten zusammen ohne Gäste | **B2B Direct Connect** |
| App für Kunden (z. B. Login mit Google) | **B2C** |

---

## 🧠 Mini-Visualisierung
B2B → [Gast in meinem Tenant]
Direct Connect→ [Zwei Tenants verbunden]
B2C → [Kunden außerhalb, eigener Tenant]


---

## ⚠️ Typische Prüfungsfallen

### ❗ Falle 1
> „Externe Benutzer greifen auf interne Ressourcen zu“

➡️ ❌ Nicht B2C  
➡️ ✅ **B2B Collaboration**

---

### ❗ Falle 2
> „Benutzer bleiben in ihrem eigenen Tenant“

➡️ ❌ Nicht B2B  
➡️ ✅ **B2B Direct Connect**

---

### ❗ Falle 3
> „Consumer App / Kundenlogin“

➡️ ❌ Nicht B2B  
➡️ ✅ **B2C**

---

## 🎯 Ultra-Kurz-Merksatz (Prüfung)

👉 **„B2B = reinholen, Direct = verbinden, B2C = verkaufen“**
---
### Navigation
- [Parent: Module Overview](README.md)
- [Previous: 🌐 Azure External Identities (AZ-900)](30_azure_external_identities.md)
- [Next: 🔐 Azure Conditional Access (AZ-900)](40_azure_conditional_access.md)
- [Home](../README.md)

