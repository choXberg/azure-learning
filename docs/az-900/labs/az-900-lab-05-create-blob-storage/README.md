# AZ-900 Lab 05 – Create Blob Storage

## 🎯 Goal
Create an Azure Storage Account and work with Blob Storage (containers and blobs).

---

## 🧱 Key Concepts

### Storage Account
A storage account is the top-level resource that provides access to Azure Storage services:
- Blob Storage (objects/files)
- File Shares
- Tables (NoSQL)
- Queues (messaging)

> Without a storage account, no storage services can be used.

---

### Blob Storage
Blob Storage is used to store **unstructured data**, such as:
- Images
- Videos
- Documents
- Backup files

Structure:
Storage Account
└── Container
└── Blob (file)

---

### Container
- Logical grouping of blobs (similar to a folder)
- Used to organize data داخل a storage account

---

### Blob
- Individual file (e.g., image, JSON, SQLite database)
- Accessible via HTTP/HTTPS

---

## 🔐 Access Levels

When creating a container:

- **Private (default)**  
  → No anonymous access  
  → Access via Azure AD, access keys, or SAS tokens  

- **Public access**  
  → Anyone on the internet can access blobs  

> ⚠️ Important for exam: Public access allows anonymous access.

---

## 💾 Redundancy Options

Selected in this lab:
- **LRS (Locally Redundant Storage)**  
  → Data is replicated 3 times within a single datacenter  

Other options (for awareness):
- GRS → Geo-redundant (different region)
- ZRS → Zone-redundant (availability zones)

---

## ⚙️ What was done in this Lab

1. Created a **Storage Account**
2. Created a **Blob Container**
3. Uploaded a **Blob (image file)**
4. Explored:
   - Blob actions (view, download, delete)
   - Monitoring (Insights)
   - Troubleshooting options

---

## 📊 Monitoring

Available under **Monitoring**:
- Insights (performance, availability, failures)
- Metrics
- Logs

> Azure Monitor integrates with storage accounts.

---

## 🧠 Exam-Relevant Takeaways

- Storage Account is required for all storage services
- Blob Storage = unstructured data
- Container = logical grouping
- Blob = file/object
- Access levels (private vs public) are important
- LRS = 3 copies in one datacenter

---

## 🔥 Real-World Use Case (POIneer)

Blob Storage can be used to:
- Store generated `.sqlite` files
- Host map data or tiles
- Provide downloads for mobile clients

Example flow:
Renderer → generates SQLite DB
→ Upload to Blob Storage
→ Mobile app downloads latest version

---

## 🧪 Practice Questions

**1. What is required to store blobs in Azure?**  
A) Container  
B) Storage Account  
C) Virtual Machine  
→ **Answer: B**

---

**2. What is a blob?**  
A) Virtual machine  
B) File/object  
C) Database  
→ **Answer: B**

---

**3. What does LRS provide?**  
A) Global replication  
B) 3 copies in one datacenter  
C) No redundancy  
→ **Answer: B**

---

**4. What does public access allow?**  
A) Only admins can access  
B) Anonymous internet access  
C) Only API access  
→ **Answer: B**

---

## 🧘 Summary

This lab introduced Azure Blob Storage:
- Creating storage accounts
- Managing containers and blobs
- Understanding access control and redundancy

Blob Storage is a core Azure service and highly relevant for real-world applications.