# Scenario 7: Data Transformation - Solution

```javascript
// API Layer
function formatUserForAPI(user) {
    return {
        id: user.id,
        fullName: user.firstName + ' ' + user.lastName,
        email: user.email.toLowerCase()
    };
}

// Email Service
function formatUserForEmail(user) {
    return {
        id: user.id,
        fullName: user.firstName + ' ' + user.lastName,
        email: user.email.toLowerCase()
    };
}
```

**Answer: DRY VIOLATION**

**Explanation:** This duplicates the knowledge of how to format a user's full name and normalize email addresses. If the business changes how names are formatted, you'd need to update multiple places.

**Solution:** Create a shared User formatter:
```javascript
function formatUser(user) {
    return {
        id: user.id,
        fullName: user.firstName + ' ' + user.lastName,
        email: user.email.toLowerCase()
    };
}
```

---
