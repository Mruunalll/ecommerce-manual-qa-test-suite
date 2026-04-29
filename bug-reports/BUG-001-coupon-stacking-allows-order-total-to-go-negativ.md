## BUG-001 — Coupon stacking allows order total to go negative

**Title:** Coupon stacking allows order total to go negative  
**Environment:** Chrome 124, WooCommerce 8.3, Staging  
**Severity:** Critical | **Priority:** High  

**Steps to Reproduce:**
1. Add product ($20) to cart
2. Apply coupon "FLAT25OFF" (flat $25 discount)
3. Apply coupon "EXTRA10OFF" (additional $10 off)

**Expected Result:** Second coupon blocked, OR total floors at $0  
**Actual Result:** Order total shows **–$15.00**; order can be placed with negative charge

---
