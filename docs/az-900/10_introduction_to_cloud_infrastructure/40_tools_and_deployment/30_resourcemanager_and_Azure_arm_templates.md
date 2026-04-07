# Azure Resource Manager (ARM) & ARM Templates

## What is Azure Resource Manager?

**Azure Resource Manager (ARM)** is the deployment and management service for Azure. It provides a consistent management layer that allows you to create, update, and delete resources in your Azure account.

Every request made through Azure tools (Portal, CLI, PowerShell, APIs, SDKs) goes through ARM.

### Request Flow

1. A user sends a request (Portal, CLI, API, etc.)
2. ARM authenticates and authorizes the request
3. ARM forwards the request to the appropriate Azure service
4. The service executes the requested action

👉 This ensures **consistent behavior across all tools**, because everything uses the same underlying API.

---

## Benefits of Azure Resource Manager

With ARM, you can:

- Use **declarative templates** instead of manual scripts
- Manage resources as a **group (resource group)** instead of individually
- Ensure **consistent deployments** across environments
- Define **dependencies between resources**
- Use **Role-Based Access Control (RBAC)** for security
- Apply **tags** for organization and cost tracking

---

## Infrastructure as Code (IaC)

**Infrastructure as Code (IaC)** means managing infrastructure using code instead of manual configuration.

### Evolution of IaC in Azure:

- Start: Azure CLI / PowerShell
- Advanced: ARM Templates or Bicep
- Goal: **Repeatable, automated deployments**

👉 This aligns directly with DevOps principles.

---

## Azure Resource Manager Templates

ARM templates are **JSON files** that define the desired state of your Azure infrastructure.

### Key Characteristics

- Declarative: Define *what* should be deployed, not *how*
- Validated before deployment
- Resources are deployed:
  - In the correct order (based on dependencies)
  - In parallel when possible

### Example (simplified)

```json
{
  "$schema": "https://schema.management.azure.com/schemas/2019-04-01/deploymentTemplate.json#",
  "resources": [
    {
      "type": "Microsoft.Storage/storageAccounts",
      "apiVersion": "2021-04-01",
      "name": "mystorageaccount",
      "location": "westeurope",
      "sku": {
        "name": "Standard_LRS"
      },
      "kind": "StorageV2"
    }
  ]
}
```

## Benefits of ARM Templates
- Declarative syntax → focus on desired state
- Repeatability → same template = same result
- Orchestration → dependencies handled automatically
- Modularity → reusable/nested templates
- Extensibility → integrate PowerShell or Bash scripts if needed

---

## Bicep

Bicep is a modern, declarative language for deploying Azure resources via ARM.

👉 It is essentially a simplified abstraction over ARM templates (JSON).

### Benefits of Bicep
- Cleaner syntax → easier to read and write than JSON
- Up-to-date resource support → tracks Azure APIs automatically
- Idempotent deployments → safe to run multiple times
- Built-in orchestration → handled by ARM
- Modularity → supports reusable modules

### Example (Bicep vs JSON)
Bicep

```json
resource storage 'Microsoft.Storage/storageAccounts@2021-04-01' = {
  name: 'mystorageaccount'
  location: 'westeurope'
  sku: {
    name: 'Standard_LRS'
  }
  kind: 'StorageV2'
}
```
👉 Much cleaner than JSON.

---

## Key Takeaways
- ARM is the central management layer of Azure
- All Azure operations go through ARM
- ARM templates enable Infrastructure as Code using JSON
- Bicep simplifies ARM templates and improves readability
- IaC ensures:
    - consistency
    - repeatability
    - automation

## 🧠 Exam Tip
- ARM = control plane (management layer)
- Templates/Bicep = Infrastructure as Code tools
- Declarative = define what, not how