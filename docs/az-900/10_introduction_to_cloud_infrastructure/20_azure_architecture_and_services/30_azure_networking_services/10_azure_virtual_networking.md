# Describe Azure Virtual Networking

## Overview

Azure Virtual Networking enables secure communication between:

- Azure resources (VMs, Web Apps, Databases)
- Internet users
- On-premises environments

Think of it as an extension of your on-premises network into Azure.

---

## Key Capabilities

- Isolation and segmentation  
- Internet communication  
- Communication between Azure resources  
- Communication with on-premises resources  
- Traffic routing  
- Traffic filtering  
- Virtual network connectivity  

---

## Public vs Private Endpoints

### Public Endpoint
- Has a public IP address
- Accessible from anywhere on the internet

### Private Endpoint
- Exists inside a Virtual Network (VNet)
- Uses a private IP address
- Not directly accessible from the internet

---

## Isolation and Segmentation

- Create multiple isolated VNets
- Define a private IP address range
- Split into subnets

Benefits:
- Logical separation
- Improved security
- Better organization

### DNS Options

- Built-in Azure DNS
- Custom internal or external DNS servers

---

## Internet Communication

Enable inbound internet access via:

- Public IP address
- Public Load Balancer

---

## Communication Between Azure Resources

### Virtual Network Integration

Connect services like:

- Virtual Machines (VMs)
- Azure Kubernetes Service (AKS)
- App Service Environment

### Service Endpoints

Connect to services like:

- Azure SQL Database
- Azure Storage Accounts

Benefits:
- Improved security
- Optimized routing

---

## Communication with On-Premises

### Point-to-Site (P2S)

- Individual client connects to Azure VNet
- Uses encrypted VPN connection

### Site-to-Site (S2S)

- On-premises network connects to Azure VNet
- Gateway-to-gateway VPN
- Appears like a single network

### ExpressRoute

- Private dedicated connection
- Does not use the public internet
- Higher security and bandwidth

---

## Route Network Traffic

### Default Routing

Azure automatically routes traffic between:

- Subnets
- Virtual networks
- On-premises networks
- Internet

### Custom Routing

#### Route Tables
- Define how traffic is directed

#### User Defined Routes (UDR)
- Control routing between subnets and VNets

#### Border Gateway Protocol (BGP)
- Dynamic route exchange with:
  - VPN Gateway
  - ExpressRoute

---

## Filter Network Traffic

### Network Security Groups (NSG)

- Define inbound and outbound rules
- Allow or deny traffic based on:
  - IP address
  - Port
  - Protocol

### Network Virtual Appliances (NVA)

- Specialized virtual machines
- Perform network functions like:
  - Firewall
  - WAN optimization

---

## Connect Virtual Networks

### VNet Peering

- Connect two VNets directly
- Traffic stays on the Microsoft backbone network
- Does not traverse the public internet

Benefits:

- Low latency
- High security
- Cross-region connectivity

---

## Exam Tips

- VNet is the core networking building block in Azure
- Subnet is used for segmentation within a VNet
- NSG is used for traffic filtering
- UDR is used for custom routing
- VNet Peering connects VNets privately
- Service Endpoints vs Private Endpoints:
  - Service Endpoint: secure service access over VNet
  - Private Endpoint: private IP inside VNet
- ExpressRoute provides private connectivity without using the internet
---
- [Next: Describe Azure Virtual Private Networks (VPN)](20_azure_virtual_private.md)
- [Home](../../../README.md)

