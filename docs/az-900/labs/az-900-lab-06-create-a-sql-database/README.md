# AZ-900 Lab 06 – Create a SQL Database

## Overview
In this lab, an Azure SQL Database was created using a sample dataset (AdventureWorksLT), configured for access, and queried using the built-in Query Editor.

---

## Key Concepts

### 1. Azure SQL Database (PaaS)
- Fully managed relational database service
- No need to manage OS, patching, or infrastructure
- Built on SQL Server engine

👉 Exam Tip:
Azure SQL Database = **Platform as a Service (PaaS)**

---

### 2. Logical SQL Server
- A database must be hosted on a logical SQL server
- Server defines:
  - Admin login
  - Region
  - Firewall rules

👉 Important:
- Multiple databases can exist on one server

---

### 3. Authentication
- SQL authentication used:
  - Username: `sqluser`
  - Password: defined during setup

Alternative (not used here):
- Azure AD authentication

---

### 4. Networking & Firewall

Initial problem:
- Connection to database failed due to blocked client IP

Solution:
- Add client IP to server firewall

Steps:
1. Go to SQL Server
2. Open **Firewall settings**
3. Add client IP
4. Save changes

👉 Exam Tip:
- Azure SQL blocks access by default
- You must explicitly allow IP addresses

---

### 5. Public Endpoint Access
- Database exposed via public endpoint
- Access controlled via firewall rules

👉 Important:
- "Allow Azure services" = enables internal Azure communication

---

### 6. Sample Data (AdventureWorksLT)
- Preloaded dataset for testing
- Includes tables like:
  - `Product`
  - `ProductCategory`

---

### 7. Querying the Database

Example query:

    SELECT TOP 20 pc.Name as CategoryName, p.name as ProductName
    FROM SalesLT.ProductCategory pc
    JOIN SalesLT.Product p
    ON pc.productcategoryid = p.productcategoryid;

- Uses JOIN between two tables
- Executed via Azure Portal Query Editor

---

### 8. Query Editor (Portal)
- Browser-based SQL editor
- No external tools required (like SSMS)

---

### 9. Cost Awareness
- Azure SQL Database incurs cost while running
- Recommended:
  - Delete resource group after lab

---

## What I Learned

- How to create an Azure SQL Database
- Difference between SQL Server (logical) and database
- How firewall rules control access
- How to run queries directly in Azure Portal
- Basic understanding of Azure-managed databases

---

## Typical Exam Questions

**Q: What type of service is Azure SQL Database?**  
A: PaaS

**Q: Why can't you connect to a new Azure SQL Database?**  
A: Client IP is not allowed in firewall

**Q: What is required to host a SQL database in Azure?**  
A: A logical SQL server

**Q: Where are firewall rules configured?**  
A: On the SQL server (not the database)

**Q: What is AdventureWorksLT?**  
A: A sample database

---

## Notes for Real Projects (POIneer context 🚀)

- Azure SQL is great for:
  - Structured relational data
  - Complex queries
- But for POIneer:
  - SQLite (offline) still makes sense for mobile
  - Azure SQL could be useful for:
    - Admin backend
    - Analytics