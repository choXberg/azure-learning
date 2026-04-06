# Describe Azure ExpressRoute

[lern.microsoft](https://learn.microsoft.com/en-us/training/modules/describe-azure-networking-services/4-expressroute)

## Overview

Azure ExpressRoute allows you to extend your on-premises network into the Microsoft cloud using a private connection.

- Connection is called an ExpressRoute circuit
- Provided via a connectivity provider
- Does not use the public internet

Use case:
- Secure and high-performance connection between on-premises and Azure

---

## Key Characteristics

- Private connection (no public internet)
- Higher reliability
- Faster speeds
- Lower and consistent latency
- Increased security

---

## Connectivity

ExpressRoute enables connections between:

- On-premises datacenters
- Offices or branch locations
- Microsoft cloud services

Each location requires its own ExpressRoute circuit.

---

## Supported Connectivity Models

- Any-to-any (IP VPN network)
- Point-to-point Ethernet
- Virtual cross-connection (colocation facility)

Note:
Focus on when to use ExpressRoute rather than implementation details.

---

## Features and Benefits

### Connectivity to Microsoft Cloud Services

Direct access to:

- Microsoft 365 (Office 365)
- Microsoft Dynamics 365
- Azure Virtual Machines
- Azure services (e.g. Storage, Cosmos DB)

---

### Global Connectivity

#### ExpressRoute Global Reach

- Connect multiple on-premises sites via Microsoft backbone
- No public internet required

Example:
- Office in Asia ↔ Datacenter in Europe via Microsoft network

---

### Dynamic Routing

- Uses Border Gateway Protocol (BGP)
- Enables dynamic route exchange between:
  - On-premises network
  - Azure resources

---

### Built-in Redundancy

- Redundant connections at each peering location
- High availability by design
- Can configure multiple circuits for additional resilience

---

## When to Use ExpressRoute

Choose ExpressRoute when:

- You need private connectivity to Azure
- You require predictable latency
- You need high bandwidth and performance
- You have strict compliance requirements
- You want to avoid public internet for critical traffic

---

## Security Considerations

- Traffic does not traverse the public internet
- Reduces exposure to internet-based threats

Important:

Some services still use the public internet:

- DNS queries
- Certificate Revocation List (CRL) checks
- Azure CDN requests

---

# Azure Networking: VPN vs ExpressRoute

## Overview

| Feature                | VPN (Azure VPN Gateway)                  | ExpressRoute                          |
|-----------------------|-----------------------------------------|--------------------------------------|
| Connection Type       | Encrypted over public internet          | Private connection (no internet)     |
| Transport Medium      | Internet                                | Dedicated private link               |
| Security              | High (encryption)                       | Very high (private + no internet)    |
| Performance           | Variable (internet-dependent)           | High and consistent                  |
| Latency               | Higher and less predictable             | Low and predictable                  |
| Bandwidth             | Limited                                | High throughput                      |
| Reliability           | Depends on internet                     | High (SLA, redundancy)               |
| Cost                  | Lower                                  | Higher                               |

---

## Connectivity Types

### VPN

- Point-to-Site (P2S)
- Site-to-Site (S2S)
- VNet-to-VNet

### ExpressRoute

- Private connection via provider
- ExpressRoute circuit per location
- Global Reach (connect on-premises sites)

---

## Routing

| Feature        | VPN                              | ExpressRoute                     |
|----------------|----------------------------------|---------------------------------|
| Routing Type   | Static or dynamic (BGP optional) | Dynamic (BGP required)          |
| Flexibility    | Medium                           | High                            |

---

## Use Cases

### Use VPN when:

- Quick and low-cost setup is needed
- Small to medium workloads
- Development or testing environments
- Backup/failover connection (e.g. for ExpressRoute)

---

### Use ExpressRoute when:

- Mission-critical workloads
- Strict compliance requirements
- Need predictable latency
- High data transfer volumes
- Avoiding public internet is required

---

## High Availability

### VPN

- Active/Standby (default)
- Active/Active possible
- Can be used as ExpressRoute failover

### ExpressRoute

- Built-in redundancy
- Multiple circuits possible
- SLA-backed connectivity

---

## Key Differences (Exam Focus)

- VPN uses the public internet, ExpressRoute does not
- ExpressRoute provides more predictable performance
- VPN is cheaper and easier to set up
- ExpressRoute is used for enterprise-grade scenarios
- ExpressRoute uses BGP by default
- VPN can be used as a fallback for ExpressRoute

---

## Quick Summary

- VPN = secure tunnel over the internet
- ExpressRoute = private dedicated connection
- VPN = flexible and cost-effective
- ExpressRoute = high performance and reliability

---

## Exam Tips

- ExpressRoute = private connection (no internet)
- Circuit = connection between on-premises and Azure
- Uses BGP for dynamic routing
- More reliable and faster than VPN
- Global Reach connects on-premises sites via Microsoft backbone
- Still requires internet for some auxiliary services (DNS, CRL, CDN)
---
- [Previous: Describe Azure Virtual Private Networks (VPN)](20_azure_virtual_private.md)
- [Next: Describe Azure DNS](40_azure_dns.md)
- [Home](../../../README.md)

