# ADR 5: Database – MySQL RDBMS

**Date:** 2025-11-09  
**Status:** Accepted  

**Context:**  
CMS data includes structured complaint records, requiring ACID transactions and relational integrity.

**Decision:**  
Use **MySQL** as the relational database integrated via **Spring Data JPA**.

**Consequences:**  
✅ Mature, reliable, and open source  
✅ Supports indexing and backups for large datasets  
⚠️ Sharding and horizontal scaling require additional setup  

**Alternatives:**  
- PostgreSQL → equally viable but less integrated with existing expertise.  
- MongoDB → weaker consistency model.

**References:**  
- Oracle (2024). *MySQL 8.0 Reference Manual.*  
