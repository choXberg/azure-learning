## Azure Physical Infrastructure

### Core Idea

* Microsoft Azure organizes its infrastructure globally to provide:

  * high availability
  * scalability
  * resiliency

---

## 🌍 Infrastructure Hierarchy

👉 From large → small:

1. **Geography**

   * Large area (e.g. Europe, US, Asia)
   * Contains multiple regions

2. **Region**

   * Geographic area with one or more datacenters
   * Connected with **low-latency network**
   * You choose a region when deploying resources

3. **Availability Zone**

   * Physically separate locations within a region
   * Each zone has:

     * independent power
     * cooling
     * networking
   * Acts as an **isolation boundary**

4. **Datacenter**

   * Physical building with servers, racks, networking

👉 Key idea:

* Geography → Region → Zone → Datacenter

---

## Availability Zones

* Minimum **3 zones** in supported regions
* Connected via high-speed private network

👉 Benefit:

* If one zone fails → others still work

👉 Use case:

* Distribute resources across zones for high availability

---

## Azure Service Categories for Availability Zones

### 1. Zonal Services

* Resource is tied to a **specific zone**

👉 Examples:

* Virtual Machines
* Managed Disks
* Public IPs

👉 Key idea:

* You choose the zone

---

### 2. Zone-Redundant Services

* Azure automatically replicates across zones

👉 Examples:

* Zone-redundant storage
* Azure SQL Database

👉 Key idea:

* Built-in high availability (no manual setup)

---

### 3. Non-Regional Services

* Not tied to a specific region or zone
* Globally resilient

👉 Examples:

* Microsoft Entra ID
* Azure DNS

👉 Key idea:

* Always available across geographies

---

## Region Pairs

* Each region is paired with another region
* At least **300 miles apart**

👉 Benefits:

* disaster recovery
* automatic failover (in some cases)
* updates rolled out one region at a time

👉 Key idea:

* Protect against **regional outages**

---

## Sovereign Regions

* Isolated Azure environments for:

  * governments
  * compliance requirements

👉 Examples:

* Azure Government (US)
* Azure China

## 🧠 Mentales Modell (sehr wichtig!)
Geography (z. B. Europe)
    ↓
Region (z. B. West Europe)
    ↓
Availability Zone (z. B. Zone 1, 2, 3)
    ↓
Datacenter (physische Gebäude)

---

## 🎯 Ultra-Kompakte Prüfungs-Merksätze
- Availability Zone = isolated datacenter
- Zonal = du bist verantwortlich
- Zone-redundant = Azure kümmert sich
- Region Pair = Backup auf Region-Ebene

## Wichtig
- Hierarchie (Geo → Region → Zone → DC)
- 3 Zonen nebeneinander
- Zonal vs Redundant vs Global

---

## 🧠 Quick Memory Guide

* Geography → Region → Zone → Datacenter
* Zones → protect against datacenter failure
* Region pairs → protect against regional failure

---

## 🎯 Exam Triggers

👉 "Physically separate datacenters within a region"
→ Availability Zones

👉 "What to use for high availability within a region?"
→ Availability Zones

👉 "Replicate across zones automatically"
→ Zone-redundant service

👉 "Disaster recovery across regions"
→ Region Pairs

👉 "Global services not tied to region"
→ Non-regional services
