## BUG-002 — Out-of-stock product added to cart via direct URL parameter manipulation

**Title:** Out-of-stock product added to cart via direct URL parameter manipulation  
**Environment:** Chrome 124, WooCommerce 8.3, Staging  
**Severity:** Critical | **Priority:** High  

**Steps to Reproduce:**
1. Find OOS product (e.g., ID 47)
2. Visit `/?add-to-cart=47` directly in browser
3. Check cart

**Expected Result:** OOS product not added; error displayed  
**Actual Result:** Product added to cart successfully; checkout proceeds

---
