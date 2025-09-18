# Scenario 8: Constants - Solution

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

**Answer: ACCEPTABLE DUPLICATION**

**Explanation:** Even though the values are identical, they represent different business concepts. Payment retry logic might change independently of email retry logic based on different business requirements.

**Note:** If there's a company-wide policy that "all services should retry 3 times," then it becomes a DRY violation and should be centralized.

---
