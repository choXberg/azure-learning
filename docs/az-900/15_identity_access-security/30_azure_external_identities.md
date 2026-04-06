# 🌐 Azure External Identities (AZ-900)

## 🧠 Überblick
- **External Identity** = Identität außerhalb deines Tenants
  - z. B. Partner, Kunden, Lieferanten, externe Entwickler
- Ermöglicht:
  - Zugriff auf Ressourcen **ohne eigene interne Accounts**

---

## 🎯 Warum sind externe Identitäten wichtig?
- Zusammenarbeit mit:
  - Partnern
  - Lieferanten
  - Kunden
- Vorteile:
  - Kein eigenes User-Management nötig
  - Nutzer verwenden **ihre eigenen Accounts**
- Du kontrollierst:
  - Zugriff (Authorization)
- Externer Provider kontrolliert:
  - Anmeldung (Authentication)

---

## 🔐 Identity Provider (wichtig!)
Externe Nutzer können sich anmelden mit:
- Firmenkonto (anderer Tenant)
- Social Login (Google, Facebook)
- Microsoft Account
- Behörden-Identitäten

---

## 🔄 Abgrenzung zu SSO

| Thema | Beschreibung |
|------|-------------|
| SSO | Login innerhalb eines Tenants |
| External Identities | Zugriff über Tenant-Grenzen hinweg |

---

## ⚙️ External Identity Features

### 🤝 B2B Collaboration
- Externe Nutzer werden als **Guest User** in deinem Tenant angelegt
- Zugriff auf:
  - Apps
  - Ressourcen
- Nutzung:
  - Klassische Zusammenarbeit

---

### 🔗 B2B Direct Connect
- Verbindung zwischen zwei Tenants (Trust)
- Kein Gast-User im Tenant notwendig
- Aktuell:
  - Fokus auf Microsoft Teams (Shared Channels)
- Nutzer bleiben in ihrem eigenen Tenant

---

### 👥 External ID for Customers (Azure AD B2C)
- Für:
  - Kunden / Endnutzer (B2C Szenario)
- Nutzung:
  - Eigene Apps (SaaS / Custom Apps)
- Verwaltung:
  - Separater Tenant

---

## 🧩 Vergleich der Modelle

| Feature                | B2B Collaboration | B2B Direct Connect | External ID (B2C) |
|------------------------|------------------|--------------------|-------------------|
| Zielgruppe             | Partner / Gäste  | Partner (Teams)    | Kunden            |
| Benutzer im Tenant     | ✅ Ja (Guest)     | ❌ Nein            | ❌ Separat        |
| Typischer Use Case     | App-Zugriff      | Teams Collaboration| Kunden-Apps       |

---

## 👉 Unterschied  B2B Direct Connect zu B2B Collaboration:

| Feature              | B2B Collaboration | B2B Direct Connect         |
| -------------------- | ----------------- | -------------------------- |
| Guest User           | ✅ Ja              | ❌ Nein                     |
| Tenant-Wechsel nötig | Oft ja            | ❌ Nein                     |
| Teams Integration    | Eingeschränkt     | ✅ Native (Shared Channels) |

---
## Kurzvergleich (perfekt für Prüfung)

| Thema       | B2B                  | B2C                            |
| ----------- | -------------------- | ------------------------------ |
| Bedeutung   | Business to Business | Business to Consumer           |
| Zielgruppe  | Partner / Firmen     | Kunden / Endnutzer             |
| Zugriff auf | Interne Ressourcen   | Öffentliche Apps               |
| User-Typ    | Guest User im Tenant | Externe User im eigenen System |
| Login       | Firmenkonto          | Social Login / E-Mail          |

## 🧠 Ultimativer Merksatz

- 👉 B2B = Partner arbeiten mit dir
- 👉 B2C = Kunden nutzen dein Produkt

## 🎯 Prüfungs-Shortcut
- „Partner greift auf meine Ressourcen zu“ → B2B
- „Kunde loggt sich in App ein“ → B2C

## 🔄 Zugriff verwalten (sehr wichtig!)

### 👀 Access Reviews
- Regelmäßige Überprüfung:
  - Braucht der User noch Zugriff?
- Beteiligte:
  - User selbst oder Entscheider
- Ergebnis:
  - Zugriff behalten oder entfernen

---

## 🎯 Prüfungsrelevante Kernaussagen

- External Identities = Zugriff **außerhalb deines Tenants**
- Authentication = externer Provider
- Authorization = dein Tenant (Entra ID)
- B2B Collaboration = Guest User im Tenant
- B2B Direct Connect = kein Guest User
- B2C = für Kunden (separater Tenant)
- Access Reviews = Zugriff regelmäßig prüfen

---

## 🧠 Merksatz

👉 **„Extern anmelden – intern kontrollieren.“**
---
### Navigation
- [Parent: Module Overview](README.md)
- [Previous: 🔐 Azure Authentication Methods (AZ-900)](20_azure_authentication_methods.md)
- [Next: 🧠 External Identities – Eselsbrücken & Prüfungs-Shortcut (AZ-900)](35_azure_external_identities_shortcut.md)
- [Home](../README.md)

