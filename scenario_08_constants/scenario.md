# Scenario 8: Constants

```java
// PaymentProcessor.java
public class PaymentProcessor {
    private static final int MAX_RETRY_ATTEMPTS = 3;
    // Uses for payment retries
}

// EmailService.java  
public class EmailService {
    private static final int MAX_RETRY_ATTEMPTS = 3;
    // Uses for email delivery retries
}
```
**Question:** Is this a DRY violation?

---
