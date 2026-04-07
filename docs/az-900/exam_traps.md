# AZ-900 Exam Traps (High Probability Questions)

## ⚠️ Trap 1: Service Health vs Resource Health vs Azure Status

| Service         | Scope                     |
| --------------- | ------------------------- |
| Azure Status    | Global (all customers)    |
| Service Health  | Your services in a region |
| Resource Health | Specific resource         |

👉 Question pattern:
"You receive a notification about your VM health"
→ Answer: **Resource Health**

---

## ⚠️ Trap 2: NSG vs Azure Firewall

| Feature    | NSG        | Firewall    |
| ---------- | ---------- | ----------- |
| Level      | L4         | L7          |
| Scope      | Subnet/NIC | Centralized |
| Complexity | Simple     | Advanced    |

👉 Exam answer rule:

* Simple filtering → NSG
* Advanced / centralized → Firewall

---

## ⚠️ Trap 3: Availability Zone vs Region

| Term   | Meaning                    |
| ------ | -------------------------- |
| Region | Multiple datacenters       |
| Zone   | Single isolated datacenter |

👉 High availability inside region → **Zones**

---

## ⚠️ Trap 4: IaaS vs PaaS vs SaaS

| Model | Responsibility           |
| ----- | ------------------------ |
| IaaS  | You manage most          |
| PaaS  | Azure manages platform   |
| SaaS  | Azure manages everything |

👉 Question pattern:
"Which requires least management?"
→ SaaS

---

## ⚠️ Trap 5: Pricing Calculator vs Cost Management

| Tool               | Purpose           |
| ------------------ | ----------------- |
| Pricing Calculator | Before deployment |
| Cost Management    | After deployment  |

---

## ⚠️ Trap 6: VPN vs ExpressRoute

| Feature    | VPN       | ExpressRoute |
| ---------- | --------- | ------------ |
| Connection | Internet  | Private      |
| Security   | Encrypted | Dedicated    |
| Cost       | Lower     | Higher       |

---

## ⚠️ Trap 7: Blob vs File Storage

| Storage | Use Case           |
| ------- | ------------------ |
| Blob    | Unstructured data  |
| File    | Shared file system |

---

## ⚠️ Trap 8: Scaling vs Elasticity

* Scaling = increase/decrease resources
* Elasticity = automatic scaling based on demand

---

## ⚠️ Trap 9: CapEx vs OpEx

* CapEx = upfront
* OpEx = pay-as-you-go (cloud!)

---

## ⚠️ Trap 10: Azure Policy vs Resource Locks

| Tool   | Purpose                  |
| ------ | ------------------------ |
| Policy | Enforce rules            |
| Locks  | Prevent deletion/changes |

---

## ⚠️ Trap 11: Monitor vs Advisor

| Tool    | Purpose             |
| ------- | ------------------- |
| Monitor | Data (metrics/logs) |
| Advisor | Recommendations     |

---

## 🧠 Final Tip

If two answers look similar:

👉 Ask yourself:

* **Monitoring or recommendation?**
* **Before or after deployment?**
* **Simple or advanced?**
* **Global or resource-specific?**
