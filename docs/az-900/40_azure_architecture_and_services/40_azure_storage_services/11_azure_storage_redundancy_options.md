# Azure Storage Redundancy Options

## Overview

Redundancy defines how Azure replicates your data to ensure:

- Durability
- Availability
- Fault tolerance

---

## Redundancy Types

### LRS (Locally Redundant Storage)

- Data is replicated within a single datacenter
- Typically 3 copies

Pros:
- Lowest cost

Cons:
- No protection against datacenter failure

Use case:
- Non-critical data

---

### ZRS (Zone-Redundant Storage)

- Data replicated across multiple Availability Zones in the same region

Pros:
- Protection against datacenter failure
- High availability

Cons:
- Slightly higher cost than LRS

Use case:
- High availability within a region

---

### GRS (Geo-Redundant Storage)

- Data replicated to a secondary region (paired region)
- Asynchronous replication

Pros:
- Protection against regional failure

Cons:
- Secondary region not readable

Use case:
- Disaster recovery scenarios

---

### RA-GRS (Read-Access Geo-Redundant Storage)

- Same as GRS, but:
- Read access to secondary region

Pros:
- Read from secondary region
- Better availability for read operations

---

### GZRS (Geo-Zone-Redundant Storage)

- Combines ZRS + GRS
- Replicated across zones AND to another region

Pros:
- Very high durability and availability

Use case:
- Mission-critical applications

---

### RA-GZRS (Read-Access Geo-Zone-Redundant Storage)

- Same as GZRS + read access to secondary region

Pros:
- Maximum availability and resilience

---

## Comparison Overview

| Type     | Region Protection | Zone Protection | Read Access Secondary | Cost        |
|----------|------------------|------------------|------------------------|-------------|
| LRS      | ❌               | ❌               | ❌                     | Low         |
| ZRS      | ❌               | ✅               | ❌                     | Medium      |
| GRS      | ✅               | ❌               | ❌                     | Medium      |
| RA-GRS   | ✅               | ❌               | ✅                     | Medium+     |
| GZRS     | ✅               | ✅               | ❌                     | High        |
| RA-GZRS  | ✅               | ✅               | ✅                     | Highest     |

---

## Exam Tips

- LRS = cheapest, lowest protection
- ZRS = protects against datacenter failure
- GRS = protects against regional failure
- RA-GRS = read access to secondary region
- GZRS = zones + geo replication
- RA-GZRS = highest availability option