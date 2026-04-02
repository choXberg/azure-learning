# 🌐 Public Cloud

## Definition
Cloud resources are provided by a vendor and shared by many customers.

Examples:

- Microsoft Azure
- Amazon Web Services
- Google Cloud Platform

## Characteristics

- The infrastructure belongs to the provider
- Access happens over the internet
- Pay-as-you-go 💸
- Highly scalable

## Advantages

- No hardware effort
- Quick to get started
- Very flexible

## Disadvantages

- Less control
- Data protection/compliance can be a concern

👉 In practice: this is what you learn when working with Azure.

# 🏢 Private Cloud

## Definition
Cloud infrastructure is used by only one organization.

It can be:

- in its own datacenter (on-premises)
- dedicated at a provider

## Characteristics

- Full control 🔒
- Own hardware / dedicated resources
- Higher security (in theory)

## Advantages

- Maximum control
- Good for sensitive data

## Disadvantages

- Expensive 💸💸
- You handle maintenance and operations yourself
- Less flexible

👉 In practice: classic enterprise IT or banks.

# 🔀 Hybrid Cloud

## Definition
Combination of private cloud + public cloud

Example:

- Database remains on-premises
- Web app runs in Microsoft Azure

## Characteristics

- Connection between both worlds (VPN / ExpressRoute)
- Data can be moved flexibly

## Advantages

- Best of both worlds
- Sensitive data stays internal
- Scaling through the cloud is possible

## Disadvantages

- More complex 🧠
- Networking + security are more demanding

👉 In practice: very common in companies, especially during cloud migration.

# 🌍 Multicloud

## Definition
A company uses multiple public cloud providers at the same time.

## 👉 Example

- Backend runs on Amazon Web Services
- AI/analytics runs on Microsoft Azure
- Data analytics may run on Google Cloud Platform

# Short Comparison

| Feature              | Public Cloud                                       | Private Cloud                                           | Hybrid Cloud                                           | Multi-Cloud                            |
| -------------------- | -------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------ | -------------------------------------- |
| **Definition**       | Cloud services offered over the internet to anyone | Cloud infrastructure dedicated to a single organization | Combination of public + private cloud with integration | Use of multiple cloud providers        |
| **Ownership**        | Cloud provider (e.g. Microsoft, Amazon)            | Single organization                                     | Shared (organization + provider)                       | Multiple providers                     |
| **Accessibility**    | Public (via internet)                              | Private (restricted access)                             | Both public and private                                | Depends on each provider               |
| **Cost Model**       | Pay-as-you-go                                      | High upfront + maintenance                              | Mixed                                                  | Mixed                                  |
| **Control**          | Low (provider-managed)                             | High (full control)                                     | Medium                                                 | Medium                                 |
| **Scalability**      | Very high                                          | Limited                                                 | High (can burst to public cloud)                       | Very high                              |
| **Security**         | Standardized, provider-managed                     | Highest control, customizable                           | Flexible                                               | Depends on setup                       |
| **Typical Use Case** | Web apps, startups, scalable workloads             | Sensitive data, compliance, legacy systems              | Gradual migration, data separation                     | Vendor independence, risk distribution |
| **Example Scenario** | Hosting a website in Azure                         | Internal company datacenter                             | Database on-prem + app in cloud                        | App split across Azure + AWS           |

# 🔗 Azure Arc

## 🌍 Core Idea

Azure Arc allows you to:

- 👉 manage resources outside Azure as if they were in Azure

## 🧠 In One Sentence

👉 Azure Arc extends Azure to other environments.

## Normally

Azure manages only resources inside Azure.

With Azure Arc, you can also manage:

- 🖥️ on-premises servers
- ☁️ other clouds (for example AWS, GCP)
- ☸️ Kubernetes clusters

👉 and do it centrally through the Azure portal.

## 🔥 Memory Aid

👉 Azure Arc = Azure management for everything, no matter where it runs

# Azure VMware Solution (AVS)

## 👉 Infrastructure Service

VMware runs directly in Azure.

You get:

- vSphere
- vSAN
- NSX

### 👉 Lift and Shift Without Rebuilding

Typical use:

- Migrating existing VMware workloads
- Continuing to run legacy systems unchanged

👉 AVS = "I move my VMware environment into Azure"

### 🔥 Exam-Ready Memory Aids

- Azure Arc = Manage everything
- Azure VMware Solution = Run VMware in Azure

## Azure Arc vs. Azure VMware Solution

| Topic      | Azure Arc            | Azure VMware Solution |
| ---------- | -------------------- | --------------------- |
| Purpose    | Management           | Infrastructure        |
| Resources  | stay where they are  | run in Azure          |
| Migration  | ❌ no                | ✅ yes                |
| Focus      | Control              | Operations            |

## 💪 Conclusion

- 👉 Arc = control
- 👉 AVS = migration + operations

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

- How can costs be estimated reliably?
- Which services are most cost-sensitive?

---

## 💡 What I Took Away

- Important for designing scalable backend systems
- Usage must be monitored, otherwise there is cost risk

---

# High Availability

## ⬆️ Vertical Scaling (Scale Up)

👉 Make a single system more powerful

- more CPU
- more RAM
- a better machine

#### Vertical → when you want to keep it simple

Typical cases:

- small application
- monolith
- database (very common)
- quick fix ("give it more power")

👉 Example:

Your API becomes slow → add more RAM → done

## Horizontal Scaling (Scale Out)

👉 Add more instances

- multiple servers
- a load balancer in front
- distributes the load

#### Horizontal → when you HAVE to scale

Typical cases:

- many users
- cloud-native apps
- microservices
- high availability

👉 Example:

The web API gets a lot of traffic → run multiple instances

---

# ☁️ Security and Governance

| Model | Who does more? |
| ----- | -------------- |
| IaaS  | you            |
| PaaS  | shared         |
| SaaS  | provider       |

👉 This also applies to security and governance.

# 🏗️ IaaS – Infrastructure as a Service

## 🔐 Security

👉 You have major responsibility.

## Advantages

Full control over:

- OS
- network
- firewall
- ability to use your own security tools

👉 good for special requirements

## 📋 Governance

👉 very flexible, but also a lot of work

### Advantages

- your own policies are possible
- full control over the architecture
- individually customizable

### ⚠️ Disadvantage (important)

- high effort
- many possible sources of error

# ⚙️ PaaS – Platform as a Service

## 🔐 Security

👉 Shared responsibility

## Advantages

- The OS is patched by the provider
- Integrated security (for example TLS, identity)
- Smaller attack surface

👉 You focus on the code.

## 📋 Governance

### Advantages

- easy integration with Azure Policy
- standardized environment
- less chaos than IaaS

### ⚠️ Disadvantage

- less control than IaaS

# 🧩 SaaS – Software as a Service

## 🔐 Security

👉 The provider does almost everything.

## Advantages

- automatic updates
- security fully managed
- minimal effort for you

## 📋 Governance

### Advantages

- easy user and access management
- compliance is often already integrated
- quick usage without setup

### ⚠️ Disadvantage

- little influence
- limited customizability

### 🧠 Comparison

| Model | Security                                 | Governance                     |
| ------| ---------------------------------------- | ------------------------------ |
| IaaS  | maximum flexibility, but you are responsible | full control, high effort   |
| PaaS  | secure + less effort                     | standardized + integrated      |
| SaaS  | maximum simplicity                       | strongly predefined            |

👉 The higher the service level, the less you need to secure and govern yourself.

---

# Management of the Cloud

## Management of the cloud refers to managing your cloud resources. In the cloud, you can:

- Automatically scale resource deployment based on need.
- Deploy resources based on a preconfigured template, removing the need for manual configuration.
- Monitor the health of resources and automatically replace failing resources.
- Receive automatic alerts based on configured metrics, so you're aware of performance in real time.

---

## ☁️ Management in the Cloud

Cloud management refers to how you create, configure, monitor, and maintain cloud resources.

There are four primary ways to manage cloud environments:

- Web Portal (GUI)
- Command Line Interface (CLI)
- PowerShell
- APIs

## 🌐 1. Web Portal (GUI)

Example: Microsoft Azure Portal

Characteristics:

- Graphical user interface (browser-based)
- Beginner-friendly and intuitive
- No programming required

### Advantages

- Easy to learn and explore
- Visual feedback
- Good for quick configuration

### Disadvantages

- Not suitable for automation
- Hard to repeat tasks consistently
- Slower for large-scale operations

#### 👉 Typical use case

- initial setup
- exploration
- troubleshooting

---

## 💻 2. Command Line Interface (CLI)

CLI = general concept of text-based interaction

### Examples

- Azure CLI
- Bash (Linux shell)
- CMD (Windows)

### Characteristics

- Managed through terminal commands
- Scriptable and automatable
- Cross-platform

### Example (Azure CLI)

```bash
az group create --name myRG --location westeurope
```

### Advantages

- Fast and efficient
- Ideal for automation and CI/CD
- Repeatable processes

### Disadvantages

- Steeper learning curve
- Less visual feedback

#### 👉 Typical use case

Automation, deployments, scripting

---

## ⚡ 3. PowerShell

PowerShell is a shell and scripting language developed by Microsoft.

### Characteristics

- Object-based (.NET objects instead of plain text)
- Strong integration with the Microsoft ecosystem
- Uses a Verb-Noun command structure

### Example

```powershell
New-AzResourceGroup -Name myRG -Location westeurope
```

### Advantages

- Powerful automation capabilities
- Works with structured objects
- Well-suited for Microsoft environments

### Disadvantages

- Less common outside the Microsoft ecosystem
- Can be more complex than CLI

### 👉 Typical use case

- administration
- advanced automation
- Microsoft-centric environments

---

## 🔌 4. APIs

Cloud providers expose REST APIs for resource management.

### Characteristics

- Direct programmatic access
- HTTP-based (REST)

Example (simplified):

```http
POST https://management.azure.com/subscriptions/{id}/resourceGroups
```

### Advantages

- Maximum flexibility
- Foundation of all other tools (Portal, CLI, PowerShell)

### Disadvantages

- More complex to use directly
- Requires handling authentication and requests

### 👉 Typical use case

- custom tools
- integrations
- SDK development

---

## ⚖️ Comparison: CLI vs PowerShell vs Bash

### 🧠 Core Concepts

| Concept    | Description                                |
| ---------- | ------------------------------------------ |
| CLI        | General term for command-line interaction  |
| Bash       | Traditional Unix/Linux shell (text-based)  |
| PowerShell | Object-oriented shell + scripting language |
| Azure CLI  | Tool for managing Azure resources          |

### 🔍 Key Differences

| Feature  | Bash              | PowerShell          | Azure CLI               |
| -------- | ----------------- | ------------------- | ----------------------- |
| Type     | Shell             | Shell + Language    | Tool                    |
| Platform | Linux/macOS       | Cross-platform      | Cross-platform          |
| Output   | Text              | Objects (.NET)      | JSON                    |
| Syntax   | Unix-style        | Verb-Noun           | `az <service> <action>` |
| Focus    | System operations | Microsoft ecosystem | Azure                   |

## 🔄 How They Work Together

### 👉 Important for exams

- Azure CLI runs inside Bash, PowerShell, or CMD
- PowerShell can execute Azure CLI commands

### Example

```bash
az vm list
```

### 👉 PowerShell simply invokes Azure CLI here.

---

## 🧪 Exam-Relevant Key Points

### ✅ Portal

Easy, but not automatable

### ✅ CLI

Fast, scriptable, ideal for DevOps

### ✅ PowerShell

Powerful, object-based, Microsoft-focused

### ✅ APIs

The underlying foundation of all management methods

---

## Underlying Foundation of All Management Methods

### 🚀 Summary

- There are multiple ways to manage cloud resources
- The choice depends on:
- level of automation
- complexity
- environment

### 👉 In practice, they are often combined

- Portal → learning and quick tasks
- CLI / PowerShell → automation
- APIs → integration and advanced scenarios

---

## Describe Sustainability Considerations in the Cloud

Cloud computing can support sustainability goals when teams actively optimize how resources are deployed and used.

### Why the cloud can improve efficiency

Cloud providers operate at large scale, which can improve resource utilization compared to many isolated on-premises environments. In Azure, you can also reduce waste by matching deployed resources to actual demand.

### Sustainability-aligned cloud practices

Examples of practices that support sustainability and cost efficiency include:

- scaling resources down when demand decreases
- turning off or deallocating resources that are not in use
- choosing efficient services and configurations to reduce overprovisioning
- using governance and monitoring to track usage trends and optimize deployments over time

For example, a development environment that runs only during business hours can be automatically shut down overnight and on weekends. This practice reduces unnecessary consumption while still meeting team needs.

At a fundamentals level, sustainability in the cloud is closely tied to good operational habits:

- right-size
- automate
- monitor
- continuously optimize
