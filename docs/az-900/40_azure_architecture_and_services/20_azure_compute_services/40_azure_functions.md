# ⚡ Azure Functions – Summary (AZ-900 relevant)

## 🧠 What are Azure Functions?

- **Event-driven, serverless compute service**
- No need to manage:
  - Virtual Machines
  - Containers
- Code runs **only when triggered by an event**

👉 Key idea:
- **No event = no running resources**

---

## ⚙️ Serverless Computing (Core Concept)

- Infrastructure is **fully managed by Azure**
- You focus only on **writing code**
- Resources are:
  - Automatically allocated
  - Automatically deallocated

👉 **Billing model:**
- Pay **only for execution time (CPU usage)**
- No cost when nothing runs

---

## 🚀 Triggers & Execution

Functions run in response to events such as:

- HTTP requests (REST APIs)
- Timer schedules
- Messages (e.g., queues, events)

👉 Flow:
Event → Function runs → Output (API, storage, etc.)

---

## 📈 Benefits of Azure Functions

- **No infrastructure management**
- **Automatic scaling**
- **Cost-efficient (pay-per-use)**
- Ideal for **short-lived tasks (seconds)**

👉 Best when:
- Workloads are **event-based**
- Demand is **unpredictable or variable**

---

## 🔄 Scaling Behavior

- Automatically scales **based on incoming events**
- Handles:
  - Sudden spikes
  - Low/idle periods

👉 **Exam Key Point:**
- Scaling is **fully automatic**

---

## 🧩 Stateless vs Stateful

### Stateless (default)
- Each execution is independent
- No memory of previous runs

### Stateful (Durable Functions)
- Maintains state between executions
- Tracks workflows and long-running processes

👉 **Durable Functions = stateful functions**

---

## 🏗️ Flexibility

- Can run:
  - Fully serverless
  - Inside more controlled environments if needed
- Can integrate with:
  - Virtual Networks
  - Isolated environments

---

## 🎯 When to use Azure Functions?

Use when you need:

- Event-driven execution
- Short, lightweight processing
- Automatic scaling
- Minimal operational overhead

👉 Typical use cases:
- APIs
- Background jobs
- Data processing
- Automation tasks

---

## 🧪 Exam-Relevant Key Points

- Azure Functions = **serverless + event-driven**
- No need to manage infrastructure
- **Pay only when code runs**
- Supports:
  - HTTP, timer, message triggers
- **Automatic scaling**
- Stateless by default, stateful via **Durable Functions**

---

## 🧠 Quick Memory Aid

> **Event triggers execution**  
> **No event = no cost**  
> **Auto-scale + serverless**