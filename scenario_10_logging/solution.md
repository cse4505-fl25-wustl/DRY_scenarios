# Scenario 10: Logging - Solution

```java
// OrderService.java
logger.info("Processing order: " + orderId + " at " + new Date());

// PaymentService.java
logger.info("Processing payment: " + paymentId + " at " + new Date());
```

**Answer: ACCEPTABLE DUPLICATION**

**Explanation:** These are different log messages for different business events. While the format is similar, they're logging distinct information for different purposes.

**Note:** If there was a standard logging format requirement, you might extract a formatting utility, but the core logging is appropriately different.

---
