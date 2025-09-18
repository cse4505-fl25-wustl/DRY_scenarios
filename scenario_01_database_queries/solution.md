# Scenario 1: Database Queries - Solution

```sql
-- User Service
SELECT id, name, email FROM users WHERE active = 1;

-- Report Service  
SELECT id, name, email FROM users WHERE active = 1;
```

**Answer: DRY VIOLATION**

**Explanation:** This duplicates the knowledge of how to retrieve active users. If the business rule for "active user" changes (e.g., adding a date check), you'd need to update multiple places. 

**Solution:** Create a shared view, stored procedure, or repository method:
```sql
CREATE VIEW active_users AS 
SELECT id, name, email FROM users WHERE active = 1;
```

---
