# Azure Network Security Groups (NSG)

## What is a Network Security Group?

An Azure Network Security Group (NSG) is used to filter network traffic to and from Azure resources.

It acts as a basic firewall for controlling inbound and outbound traffic at the network level.

---

## Key Concepts

- Controls traffic using **security rules**
- Can be associated with:
  - Subnets
  - Network interfaces (NICs)
- Works at **Layer 4 (TCP/UDP)**

---

## Security Rules

Each NSG contains rules that define:

- Source (IP, subnet, or service)
- Destination
- Port (e.g., 80, 443)
- Protocol (TCP/UDP)
- Action:
  - Allow
  - Deny
- Priority (lower number = higher priority)

---

## Example

Allow HTTP traffic:

- Source: Any
- Destination: Web server
- Port: 80
- Action: Allow

---

## Default Rules

Azure automatically provides default rules, such as:

- Allow traffic within the same VNet
- Deny all inbound traffic from the internet (by default)

---

## When to use NSG

- Control access to VMs
- Restrict traffic between subnets
- Secure application tiers (e.g., web → database)

---

## Exam Tips

- NSGs filter traffic at **network level**
- They are **stateful** (responses are automatically allowed)
- Can be applied to **subnets or NICs**

---

## Summary

NSGs are a fundamental security feature in Azure used to control network traffic using allow/deny rules.