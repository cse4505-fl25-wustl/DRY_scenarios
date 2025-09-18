# Scenario 10: Logging

```java
// OrderService.java
logger.info("Processing order: " + orderId + " at " + new Date());

// PaymentService.java
logger.info("Processing payment: " + paymentId + " at " + new Date());
```
**Question:** Is this a DRY violation?

---
