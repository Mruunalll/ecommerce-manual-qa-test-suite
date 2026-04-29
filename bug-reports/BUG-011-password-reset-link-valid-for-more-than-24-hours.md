## BUG-011 — Password reset link valid for more than 24 hours

**Title:** Password reset link valid for more than 24 hours  
**Environment:** All environments  
**Severity:** Major | **Priority:** High  

**Steps to Reproduce:**
1. Request password reset
2. Wait 25 hours
3. Click the link

**Expected Result:** Link expired; user prompted to request new reset  
**Actual Result:** Link still valid and functional after 48+ hours (security concern)

---
