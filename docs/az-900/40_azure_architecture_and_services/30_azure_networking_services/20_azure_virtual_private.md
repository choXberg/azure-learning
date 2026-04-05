# Describe Azure Virtual Private Networks (VPN)

## Overview

A Virtual Private Network (VPN) uses an encrypted tunnel within another network.

- Typically connects private networks over the public internet
- Ensures secure communication over untrusted networks
- Protects data from eavesdropping and attacks

Use case:
- Securely connect on-premises environments with Azure

---

## VPN Gateway

A VPN Gateway is a type of Virtual Network Gateway deployed in a dedicated subnet.

It enables:

- Site-to-Site (S2S) connections
- Point-to-Site (P2S) connections
- Network-to-Network (VNet-to-VNet) connections

Key facts:

- Data is always encrypted in transit
- Only one VPN gateway per VNet
- One gateway can connect to multiple locations

---

## VPN Connection Types

### Point-to-Site (P2S)

- Individual device connects to Azure VNet
- Uses encrypted VPN tunnel
- Client-initiated connection

### Site-to-Site (S2S)

- On-premises network connects to Azure VNet
- Gateway-to-gateway connection
- Appears as one unified network

### VNet-to-VNet

- Connects two Azure virtual networks
- Useful for multi-region architectures

---

## VPN Gateway Types

When creating a VPN gateway, choose:

### Policy-Based VPN

- Uses static IP address rules
- Evaluates each packet against defined IP ranges
- Less flexible

### Route-Based VPN (Recommended)

- Uses routing tables to direct traffic
- Supports dynamic routing (e.g. BGP)
- More flexible and scalable

Use route-based VPN for:

- VNet-to-VNet connections
- Point-to-Site connections
- Multi-site connections
- ExpressRoute coexistence
- High availability scenarios

Authentication method:
- Uses a pre-shared key (PSK)

---

## High Availability Options

### Active/Standby (Default)

- Two instances (primary + standby)
- Automatic failover
- Short downtime during failover:
  - Seconds (planned)
  - Up to ~90 seconds (unplanned)

---

### Active/Active

- Both instances are active
- Each has its own public IP
- Multiple tunnels to on-premises

Benefits:

- Higher availability
- Better performance
- Requires BGP

---

### ExpressRoute Failover

- VPN used as backup for ExpressRoute
- Ensures connectivity if ExpressRoute fails
- Uses internet as fallback path

---

### Zone-Redundant Gateway

- Deploy across Availability Zones
- Protects against zone-level failures

Benefits:

- Higher resiliency
- Better scalability
- Improved availability

Requirements:

- Supported region
- Specific gateway SKU
- Standard public IP (not Basic)

---

## Exam Tips

- VPN = encrypted tunnel over public internet
- VPN Gateway = enables secure connectivity in Azure
- Only one VPN gateway per VNet
- Route-based VPN is preferred in most scenarios
- P2S = individual client connection
- S2S = network-to-network connection
- Active/Active = higher availability with multiple tunnels
- ExpressRoute + VPN = hybrid high-availability setup
- Zone-redundant gateways protect against availability zone failures