# AZ-900 Lab 08 – Implement Azure Functions

## 🎯 Ziel
Erstellen einer Azure Function App und Ausführen einer HTTP-getriggerten Funktion (Serverless Computing).

---

## 🧠 Wichtige Konzepte

### Azure Functions
- Serverless Compute Service
- Code wird nur bei Bedarf ausgeführt (Event-driven)
- Keine Verwaltung von Servern notwendig

---

### Hosting Plan

#### Consumption Plan
- Automatische Skalierung
- Pay-per-execution (nur zahlen, wenn Code läuft)
- Ideal für sporadische Workloads

---

### Function App
- Container für mehrere Functions
- Gemeinsame Konfiguration (Runtime, Region, Monitoring)

---

### Trigger & Bindings

#### Trigger
Starten die Funktion:

- HTTP Trigger
- Timer Trigger
- Blob Trigger
- Queue Trigger
- Event Grid Trigger

#### Bindings
- Einfache Integration mit anderen Azure Services
- Input/Output ohne viel Code

---

## ⚙️ Umsetzung im Lab

### 1. Log Analytics Workspace
- Zentraler Ort für Logs und Monitoring
- Wird für Analyse und Troubleshooting genutzt

---

### 2. Function App erstellen

Wichtige Einstellungen:
- Runtime: .NET 8 (LTS)
- Hosting: Consumption Plan
- OS: Windows
- Region: East US

---

### 3. HTTP Trigger Function

Standard-Code (vereinfacht):

```csharp
public static async Task<IActionResult> Run(
    HttpRequest req,
    ILogger log)
{
    string name = req.Query["name"];
    return new OkObjectResult($"Hello, {name}");
}
```

---

### 4. Testen der Function

Beispiel URL:

```
https://<function>.azurewebsites.net/api/HttpTrigger1?code=XYZ&name=Chris
```

Antwort:

```
Hello, Chris
```

---

## 🔐 Function Keys (WICHTIG für Prüfung!)

Es gibt verschiedene Schlüsseltypen:

- Function Key → Zugriff auf eine einzelne Function
- Host Key → Zugriff auf alle Functions in der App
- Master Key → Vollzugriff (Admin)

👉 Wird genutzt zur Authentifizierung ohne Azure AD

---

## 📊 Monitoring

### Application Insights
- Logging
- Performance Tracking
- Fehleranalyse

### Invocations
- Jede Function-Ausführung wird geloggt
- Query via Application Insights möglich

---

## 💡 Prüfungsrelevante Punkte

- Azure Functions = Serverless
- Consumption Plan = automatische Skalierung + Pay-per-use
- Trigger starten Functions
- Function App = Container für Functions
- Application Insights = Monitoring & Logging
- Function Keys = Zugriffssicherung

---

## ⚠️ Kostenhinweis

- Consumption Plan ist günstig, aber:
- Ressourcen nach Lab löschen empfohlen

---

## 🧪 Beispiel Prüfungsfragen

### Frage 1
Was ist ein Vorteil von Azure Functions?

A) Man muss VMs manuell skalieren  
B) Automatische Skalierung ohne Serververwaltung  
C) Höhere Fixkosten  
D) Kein Logging möglich  

✅ Antwort: B

---

### Frage 2
Was startet eine Azure Function?

A) Binding  
B) Trigger  
C) Function Key  
D) Resource Group  

✅ Antwort: B

---

### Frage 3
Was ist Application Insights?

A) Datenbank  
B) Monitoring-Tool  
C) VM-Service  
D) Netzwerkdienst  

✅ Antwort: B

---

### Frage 4
Wann bezahlst du bei Consumption Plan?

A) Immer  
B) Nur wenn Code ausgeführt wird  
C) Nur bei Deployment  
D) Nur bei Fehlern  

✅ Antwort: B

---

## 🧩 Eigene Notizen

- Function Triggers = Startmechanismus
- HTTP Trigger sehr häufig für APIs
- Function URL enthält Sicherheitskey
- Logging über Application Insights extrem wichtig