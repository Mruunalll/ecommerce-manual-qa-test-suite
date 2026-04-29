## BUG-003 — Cart quantity field accepts negative numbers without validation

**Title:** Cart quantity field accepts negative numbers without validation  
**Environment:** Firefox 125, Windows 11  
**Severity:** Major | **Priority:** High  

**Steps to Reproduce:**
1. Add product to cart
2. On cart page, change quantity to -5
3. Click "Update Cart"

**Expected Result:** Validation error; quantity resets to 1  
**Actual Result:** Cart updates to -5 quantity; subtotal shows negative value

---
