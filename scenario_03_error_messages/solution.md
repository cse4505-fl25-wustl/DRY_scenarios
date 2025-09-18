# Scenario 3: Error Messages - Solution

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

**Answer: BORDERLINE - Depends on Context**

**Explanation:** This could be acceptable if the messages serve different purposes (UX vs API response). However, if they should always be identical, it's a violation.

**Better Approach:** Centralize error messages in a shared resource file or have the frontend use backend error messages.

---
