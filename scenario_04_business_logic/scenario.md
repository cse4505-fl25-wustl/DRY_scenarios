# Scenario 4: Business Logic

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
**Question:** Is this a DRY violation?

---
