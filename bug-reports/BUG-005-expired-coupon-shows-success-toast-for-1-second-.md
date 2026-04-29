## BUG-005 — Expired coupon shows success toast for 1 second before showing error

**Title:** Expired coupon shows success toast for 1 second before showing error  
**Environment:** Chrome 124, macOS Sonoma  
**Severity:** Minor | **Priority:** Medium  

**Steps to Reproduce:**
1. Enter expired coupon code
2. Click Apply
3. Observe UI flash

**Expected Result:** Error shown immediately; no success state  
**Actual Result:** Green success toast flashes for ~800ms before being replaced by red error — confusing UX

---
