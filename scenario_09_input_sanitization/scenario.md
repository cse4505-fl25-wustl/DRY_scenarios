# Scenario 9: Input Sanitization

```php
// UserController.php
$username = trim(strtolower($input['username']));

// LoginController.php
$username = trim(strtolower($input['username']));
```
**Question:** Is this a DRY violation?

---
