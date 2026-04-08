# AZ-900 – Lab 01: Create a Virtual Machine (IaaS)

## Core Concept
- Azure Virtual Machines are part of **Infrastructure as a Service (IaaS)**
- You are responsible for:
  - Operating system
  - Installed software
  - Security updates

---

## Key Components

### 1. Subscription
- Required to create resources
- Defines billing and access scope

### 2. Resource Group
- Logical container for resources
- Used for lifecycle management (create/delete together)

### 3. Region
- Defines physical location of the resource
- Impacts latency, availability, and cost

---

## Virtual Machine Configuration

### Image
- Defines the OS (e.g., Windows Server 2019, Ubuntu)
- Preconfigured templates provided by Azure

### Size
- Defines CPU, RAM, and cost
- Example: `Standard_D2s_v3`

### Authentication
- Username + password (or SSH key for Linux)

---

## Networking

### Public IP
- Required for external access

### Network Security Group (NSG)
- Controls inbound and outbound traffic

### Common Ports
- RDP (3389) → Remote Desktop (Windows)
- SSH (22) → Remote access (Linux)
- HTTP (80) → Web traffic

---

## Access

### Remote Desktop (RDP)
- Used to connect to Windows VMs
- Requires port 3389 to be open

---

## Example Workload

- Installed IIS (Web Server) on VM
- VM acts as a web server

---

## Key Learnings

- VM = IaaS → full control, but also full responsibility
- Azure handles infrastructure, you manage the OS
- NSG acts as a firewall for VM access
- Public IP + open port required for external access

---

## Exam Tips

- VM = IaaS (not PaaS!)
- NSG controls network traffic
- Resource Group = logical grouping
- Region affects availability and performance

## Quiz – Lab 01: Virtual Machines (IaaS)

### Question 1
What cloud service model do Azure Virtual Machines belong to?

- A) SaaS  
- B) PaaS  
- C) IaaS  
- D) FaaS  

<details>
<summary>Answer</summary>

C) IaaS

</details>

---

### Question 2
What is required to create resources in Azure?

- A) Resource Group  
- B) Subscription  
- C) Region  
- D) Availability Zone  

<details>
<summary>Answer</summary>

B) Subscription

</details>

---

### Question 3
What is the purpose of a Resource Group?

- A) Define VM size  
- B) Store user credentials  
- C) Organize and manage resources  
- D) Control network traffic  

<details>
<summary>Answer</summary>

C) Organize and manage resources

</details>

---

### Question 4
Which component controls inbound and outbound traffic for a VM?

- A) Virtual Network  
- B) Resource Group  
- C) Network Security Group (NSG)  
- D) Subscription  

<details>
<summary>Answer</summary>

C) Network Security Group (NSG)

</details>

---

### Question 5
Which port is used for Remote Desktop Protocol (RDP)?

- A) 22  
- B) 80  
- C) 443  
- D) 3389  

<details>
<summary>Answer</summary>

D) 3389

</details>

---

### Question 6
Which port is typically used for HTTP traffic?

- A) 22  
- B) 80  
- C) 443  
- D) 3389  

<details>
<summary>Answer</summary>

B) 80

</details>

---

### Question 7
What does the "Region" setting influence?

- A) VM password  
- B) Physical location, latency, and cost  
- C) Operating system  
- D) Network ports  

<details>
<summary>Answer</summary>

B) Physical location, latency, and cost

</details>

---

### Question 8
What do you manage yourself when using IaaS?

- A) Physical datacenter  
- B) Operating system and applications  
- C) Azure platform updates  
- D) Azure networking backbone  

<details>
<summary>Answer</summary>

B) Operating system and applications

</details>

---

### Question 9
What is required to connect to a Windows VM remotely?

- A) HTTP  
- B) SSH  
- C) RDP  
- D) FTP  

<details>
<summary>Answer</summary>

C) RDP

</details>

---

### Question 10
What is needed to access a VM from the internet?

- A) Private IP only  
- B) Public IP and open port  
- C) Resource Group  
- D) Availability Set  

<details>
<summary>Answer</summary>

B) Public IP and open port

</details>