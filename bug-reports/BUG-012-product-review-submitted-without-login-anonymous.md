## BUG-012 — Product review submitted without login (anonymous review goes live)

**Title:** Product review submitted without login (anonymous review goes live)  
**Environment:** Chrome 124 (logged out)  
**Severity:** Major | **Priority:** High  

**Steps to Reproduce:**
1. Log out
2. Go to product page
3. Scroll to reviews
4. Submit review directly (no login prompt)

**Expected Result:** Guest blocked from submitting review (or review held for moderation)  
**Actual Result:** Review appears immediately without moderation (WooCommerce setting not enforced)

---
