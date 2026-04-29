## BUG-006 — Variant price not updated in cart when colour changed on PDP

**Title:** Variant price not updated in cart when colour changed on PDP  
**Environment:** Chrome 124, Edge 124  
**Severity:** Major | **Priority:** High  

**Steps to Reproduce:**
1. Add product (Red variant, $25) to cart
2. Return to PDP
3. Change variant to Blue ($30)
4. Click "Add to Cart"
5. Check cart

**Expected Result:** Cart shows Blue at $30; red item either updated or new line added  
**Actual Result:** Cart shows both Red ($25) and Blue ($30) as separate lines even though Blue was meant to replace Red

---
