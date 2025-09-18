# Scenario 6: UI Components - Solution

```jsx
// LoginForm.jsx
<button className="btn-primary" onClick={handleLogin}>
    Login
</button>

// RegisterForm.jsx
<button className="btn-primary" onClick={handleRegister}>
    Register  
</button>
```

**Answer: ACCEPTABLE DUPLICATION**

**Explanation:** This is proper reuse of a design system component. The `btn-primary` class represents shared styling knowledge (good!), but each button serves a different purpose with different handlers.

**Note:** If the button styling was hardcoded in each place instead of using a shared class, that would be a DRY violation.

---
