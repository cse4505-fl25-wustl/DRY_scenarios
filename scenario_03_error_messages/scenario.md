# Scenario 3: Error Messages

```javascript
// Frontend validation
if (!email.includes('@')) {
    showError("Please enter a valid email address");
}

// Backend API response
if (!email.includes('@')) {
    return { error: "Please enter a valid email address" };
}
```
**Question:** Is this a DRY violation?

---
