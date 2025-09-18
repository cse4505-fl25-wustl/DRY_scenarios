# Scenario 5: Utility Functions - Solution

```python
# math_utils.py
def calculate_tax(amount, rate):
    return amount * rate

# financial_calculations.py
def compute_sales_tax(price, tax_rate):
    return price * tax_rate
```

**Answer: ACCEPTABLE DUPLICATION** ✅

**Explanation:** While the implementation is identical, these represent different concepts - general tax calculation vs. specific sales tax computation. They might evolve differently (e.g., sales tax might need rounding, exemptions, etc.).

**Alternative View:** Some might argue this is a violation and suggest a shared `multiply` function, but the semantic difference makes separate functions reasonable.

---
