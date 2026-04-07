# Azure Network Security: Firewall and DDoS Protection

## Azure Firewall

### What is Azure Firewall?

Azure Firewall is a managed, cloud-based network security service that protects Azure Virtual Networks.

It provides more advanced features than NSGs.

---

### Key Features

- Centralized network protection
- Stateful firewall
- Application-level filtering (Layer 7)
- Fully managed by Azure

---

### When to use Azure Firewall

- Central control of traffic across multiple networks
- Advanced filtering (URLs, domains)
- Enterprise security requirements

---

## Azure DDoS Protection

### What is DDoS Protection?

Azure DDoS Protection helps defend your applications against Distributed Denial of Service (DDoS) attacks.

These attacks try to overwhelm a service with traffic.

---

### Key Features

- Automatic detection and mitigation
- Protects public endpoints
- Integrated with Azure Virtual Network

---

### Types

- **Basic (default)**: Automatically enabled, basic protection
- **Standard**: Enhanced protection, metrics, alerts

---

## NSG vs Azure Firewall

| Feature | NSG | Azure Firewall |
|--------|-----|---------------|
| Level | Network (L4) | Network + Application (L7) |
| Scope | Subnet / NIC | Centralized |
| Complexity | Simple | Advanced |
| Management | Manual rules | Managed service |

---

## Exam Tips

- NSG = basic traffic filtering
- Azure Firewall = advanced, centralized security
- DDoS Protection = protects against traffic overload attacks

---

## Summary

Azure provides multiple layers of network security:
- NSGs for basic filtering
- Azure Firewall for advanced protection
- DDoS Protection for attack mitigation