# 🔐 Azure Authentication Methods (AZ-900)

## 🧠 Überblick
- **Authentifizierung (Authentication)** = Identitätsprüfung (User, Service, Gerät)
- Ziel:
  - Sicherheit erhöhen
  - Benutzerfreundlichkeit verbessern

---

## 🔑 Wichtige Methoden

- Passwort
- Single Sign-On (SSO)
- Multifactor Authentication (MFA)
- Passwordless Authentication

---

## ⚖️ Sicherheit vs. Komfort

| Methode        | Sicherheit | Komfort |
|---------------|-----------|--------|
| Passwort       | ❌ Niedrig | ✅ Hoch |
| MFA            | ✅ Hoch    | ⚖️ Mittel |
| Passwordless   | ✅ Sehr hoch | ✅ Hoch |

👉 **Passwordless = beste Kombination aus Sicherheit & Usability**

---

## 🔑 Single Sign-On (SSO)

### 📌 Was ist das?
- Ein Login → Zugriff auf mehrere Anwendungen

### ✅ Vorteile:
- Weniger Passwörter („Password Sprawl“ reduzieren)
- Weniger Reset-/Lockout-Probleme
- Einfacheres User-Management

### ⚠️ Wichtig:
- Sicherheit hängt vom **ersten Login** ab

---

## 🔐 Multifactor Authentication (MFA)

### 📌 Was ist das?
- Zusätzlicher Faktor beim Login

### 🔑 Drei Faktoren:

1. **Wissen** (Something you know)
   - Passwort, PIN

2. **Besitz** (Something you have)
   - Smartphone, Token

3. **Sein** (Something you are)
   - Fingerabdruck, Gesicht

---

### ✅ Vorteil:
- Passwort allein reicht nicht mehr → deutlich sicherer

---

## 🔐 Microsoft Entra MFA
- Azure-Service für MFA
- Beispiele:
  - SMS / Anruf
  - App-Notification (z. B. Authenticator)

---

## 🚫 Passwordless Authentication

### 📌 Was ist das?
- Kein Passwort mehr nötig
- Login mit:
  - Gerät + Biometrie oder PIN

### ✅ Vorteile:
- Kein Passwort-Diebstahl möglich
- Bessere Usability
- Sehr hohe Sicherheit

---

## 🔑 Passwordless Optionen in Azure

### 💻 Windows Hello for Business
- Für persönliche Firmen-PCs
- Login mit:
  - PIN
  - Biometrie
- Gerätegebunden → sehr sicher
- Unterstützt SSO

---

### 📱 Microsoft Authenticator App
- Smartphone wird Login-Faktor
- Ablauf:
  - Push-Nachricht
  - Nummer bestätigen
  - Biometrie / PIN

---

### 🔑 FIDO2 Security Keys
- Hardware-Token (USB, NFC, Bluetooth)
- Kein Passwort notwendig
- Phishing-resistent

---

# 🔐 Authentication Methods Vergleich (AZ-900)

| Kriterium            | Passwort              | SSO (Single Sign-On)         | MFA (Multifactor Auth)       | Passwordless                |
|----------------------|----------------------|------------------------------|------------------------------|-----------------------------|
| Grundidee            | Ein Faktor (Wissen)  | Ein Login für viele Apps     | Mehrere Faktoren             | Kein Passwort               |
| Sicherheit           | ❌ Niedrig           | ⚠️ Abhängig vom Login        | ✅ Hoch                      | ✅ Sehr hoch                |
| Benutzerfreundlichkeit | ✅ Hoch            | ✅ Sehr hoch                 | ⚖️ Mittel                   | ✅ Hoch                     |
| Risiko               | Hoch (Phishing, Leak)| Mittel (abhängig von Login)  | Niedrig                      | Sehr niedrig                |
| Typische Faktoren    | Passwort             | Passwort / Token             | Passwort + Gerät/Biometrie   | Gerät + Biometrie/PIN       |
| Schutz vor Phishing  | ❌ Nein              | ❌ Nein                      | ⚠️ Teilweise                 | ✅ Ja (z. B. FIDO2)         |
| Abhängigkeit Passwort| ✅ Ja                | ✅ Ja                        | ✅ Ja                        | ❌ Nein                     |
| Beispiele            | Standard Login       | Azure / M365 Login           | SMS, Authenticator App       | Windows Hello, FIDO2        |
| Prüfungsbewertung    | Schwächste Methode   | Komfort-Feature              | Standard-Sicherheitsmaßnahme | Beste Lösung                |

---

## 🧠 Schnell-Merksätze

- **Passwort** → einfach, aber unsicher  
- **SSO** → bequem, aber nicht automatisch sicher  
- **MFA** → Standard für sichere Systeme  
- **Passwordless** → Zukunft (sicher + bequem)

---

## 🎯 Typische Prüfungslogik

👉 Frage: *Welche Methode bietet höchste Sicherheit UND Komfort?*  
➡️ **Passwordless**

👉 Frage: *Welche Methode reduziert Passwort-Flut?*  
➡️ **SSO**

👉 Frage: *Welche Methode schützt bei gestohlenem Passwort?*  
➡️ **MFA**

👉 Frage: *Welche Methode ist am anfälligsten für Angriffe?*  
➡️ **Passwort**

---

## 🎯 Prüfungsrelevante Kernaussagen

- **SSO** = ein Login für viele Apps
- **MFA** = mehrere Faktoren → höhere Sicherheit
- **Passwordless** = sicherste + komfortabelste Methode
- MFA basiert auf:
  - Wissen
  - Besitz
  - Biometrie
- FIDO2 Keys = besonders sicher (kein Passwort, kein Phishing)

---

## 🧠 Merksatz

👉 **„Je weniger Passwort, desto sicherer.“**