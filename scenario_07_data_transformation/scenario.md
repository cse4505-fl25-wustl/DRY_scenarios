# Scenario 7: Data Transformation

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
**Question:** Is this a DRY violation?

---
