# Scenario 1: Database Queries

```sql
-- User Service
SELECT id, name, email FROM users WHERE active = 1;

-- Report Service  
SELECT id, name, email FROM users WHERE active = 1;
```
**Question:** Is this a DRY violation?

---
