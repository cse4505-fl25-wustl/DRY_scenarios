# Scenario 4: Business Logic - Solution

```java
// OrderController.java
public boolean canProcessOrder(Order order) {
    return order.getTotal() > 0 && order.getItems().size() > 0 
           && order.getCustomer().isActive();
}

// OrderService.java
public void validateOrder(Order order) {
    if (order.getTotal() <= 0 || order.getItems().size() == 0 
        || !order.getCustomer().isActive()) {
        throw new ValidationException("Invalid order");
    }
}
```

**Answer: DRY VIOLATION** ❌

**Explanation:** This duplicates the business rules for what constitutes a valid order. Changes to order validation rules require updates in multiple places.

**Solution:** Extract to a shared validation method:
```java
public class OrderValidator {
    public static boolean isValidOrder(Order order) {
        return order.getTotal() > 0 && order.getItems().size() > 0 
               && order.getCustomer().isActive();
    }
}
```

---
