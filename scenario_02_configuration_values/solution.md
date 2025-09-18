# Scenario 2: Configuration Values - Solution

```java
// EmailService.java
private static final String SMTP_HOST = "smtp.company.com";

// NotificationService.java  
private static final String SMTP_HOST = "smtp.company.com";
```

**Answer: DRY VIOLATION** ❌

**Explanation:** This duplicates configuration knowledge. When the SMTP server changes, you'd need to update multiple classes.

**Solution:** Use a configuration file or constants class:
```java
public class Config {
    public static final String SMTP_HOST = "smtp.company.com";
}
```

---
