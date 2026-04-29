## BUG-009 — "Continue Shopping" button on empty cart page returns 404

**Title:** "Continue Shopping" button on empty cart page returns 404  
**Environment:** Chrome 124, Firefox 125  
**Severity:** Major | **Priority:** Medium  

**Steps to Reproduce:**
1. Remove all items from cart
2. Click "Continue Shopping" button on empty cart page

**Expected Result:** Redirected to shop/products page  
**Actual Result:** 404 page — button links to `/shop/` but store slug is `/products/`

---
