# ADR 6: Authentication and Authorization – OAuth2 + JWT + RBAC

**Date:** 2025-11-09  
**Status:** Accepted  

**Context:**  
CMS requires secure login for customers, agents, and admins with GDPR compliance. Stateless session handling is preferred for scalability.

**Decision:**  
Implement **OAuth2.0 Authorization Code Flow** with PKCE for public clients (React, Mobile). Use **JWT tokens** and enforce **RBAC (Role-Based Access Control)** with roles stored in a policy database.

**Consequences:**  
✅ Secure, scalable, and stateless authentication  
✅ Enables SSO and distributed access management  
⚠️ Token management and refresh complexity  

**Alternatives:**  
- Session-based auth → not scalable.  
- Basic Auth → insecure.  

**References:**  
- OWASP (2024). *API Security Top 10.*  
- RFC 6749 – *The OAuth 2.0 Framework.*  
