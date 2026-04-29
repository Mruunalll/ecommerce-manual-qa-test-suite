## BUG-008 — Order confirmation email not sent when PayPal sandbox used

**Title:** Order confirmation email not sent when PayPal sandbox used  
**Environment:** Chrome 124, PayPal Sandbox account  
**Severity:** Major | **Priority:** High  

**Steps to Reproduce:**
1. Complete checkout using PayPal sandbox
2. Payment shows success on PayPal
3. Check registered email

**Expected Result:** Order confirmation email received within 2 minutes  
**Actual Result:** No email received; order appears in admin as "Processing" but customer never notified

---
