# Scenario 9: Input Sanitization - Solution

```php
// UserController.php
$username = trim(strtolower($input['username']));

// LoginController.php
$username = trim(strtolower($input['username']));
```

**Answer: DRY VIOLATION** ❌

**Explanation:** This duplicates the knowledge of how usernames should be sanitized. If the sanitization rules change (e.g., removing special characters), multiple places need updating.

**Solution:** Create a sanitization function:
```php
function sanitizeUsername($input) {
    return trim(strtolower($input));
}
```

---
