# ADR 7: Backend Pattern – Clean/Onion Architecture

**Date:** 2025-10-19 
**Updated** 2025-12-2
**Status:** Accepted  

**Context:**  
CMS services must remain maintainable and adaptable across evolving business rules. Framework dependencies must not pollute core logic.

**Decision:**  
Adopt **Clean Architecture with Layered Architectrue
- Domain Layer (entities, use cases)
- Repository Layer (data access)
- Service Layer (business logic)
- Controller Layer (REST interface)

**Consequences:**  
 Highly testable and maintainable structure  
 Clear separation of concerns  
 Slight overhead in abstraction layers  

**Alternatives:**  
- 3-tier architecture → tight coupling.  
- Hexagonal architecture → more complex for this scale.

**References:**  
- Fowler, M. (2019). *Patterns of Enterprise Application Architecture.*  
