# Azure Monitor

## What is Azure Monitor?

**Azure Monitor** is a platform for **collecting, analyzing, and acting on telemetry data** from your applications and infrastructure.

It works across:
- Azure
- On-premises environments
- Multicloud setups

👉 It provides end-to-end observability of your systems.

---

## How Azure Monitor Works

Azure Monitor collects data from multiple layers:

- Applications
- Operating systems
- Network infrastructure

This data is:
- Stored centrally
- Analyzed via queries
- Visualized in dashboards
- Used to trigger alerts

---

## Core Components

### 📊 Logs and Metrics

- **Metrics** → numerical data (e.g., CPU usage, memory)
- **Logs** → detailed event data (e.g., errors, traces)

👉 Both are used for monitoring and troubleshooting.

---

## Azure Log Analytics

**Log Analytics** is the tool used to query and analyze collected data.

### Capabilities:
- Run queries on log data
- Filter events (e.g., errors in the last hour)
- Perform advanced analysis
- Visualize trends over time

👉 Uses a powerful query language (KQL – Kusto Query Language)

---

## Azure Monitor Alerts

**Alerts** notify you when specific conditions are met.

### Components:

- **Alert Rule**
  - Defines the condition (e.g., CPU > 80%)

- **Action Group**
  - Defines what happens when triggered:
    - Email
    - SMS
    - Webhook
    - Automation

### Types of Alerts:

- **Metric-based alerts**
  - Example: CPU usage above 80%

- **Log-based alerts**
  - Example: specific error pattern detected

👉 Action groups are reusable across:
- Azure Monitor
- Azure Service Health
- Azure Advisor

---

## Application Insights

**Application Insights** is a feature of Azure Monitor focused on **application performance monitoring (APM)**.

### Setup Options:

- Add SDK to your application code
- Use an agent (no code changes required)

### What it monitors:

- Request rates, response times, failure rates
- Dependency calls and performance
- Page load times and user behavior
- Server performance (CPU, memory, network)

### Availability Tests:

- Sends synthetic requests to your app
- Ensures your app is responding even during low traffic

---

## Benefits

- Centralized monitoring across environments
- Real-time insights into system health
- Proactive alerting
- Deep application performance visibility
- Supports troubleshooting and optimization

---

## 🧠 Exam Tip

- Azure Monitor = **central monitoring platform**
- Key components:
  - Logs & Metrics
  - Log Analytics (queries)
  - Alerts (rules + action groups)
  - Application Insights (APM)

👉 Think: **Collect → Analyze → Act**