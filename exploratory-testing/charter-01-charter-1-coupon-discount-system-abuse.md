# Charter 1: Coupon & Discount System Abuse
**Mission:** Explore coupon application edge cases to find pricing vulnerabilities  
**Area:** Cart → Coupon Module  
**Duration:** 60 minutes  
**Tester:** Senior QA  

**Session Notes:**
- Tested sequential coupon application — second blocked ✅
- Tested simultaneous URL manipulation with two coupon params — both applied ❌ (BUG-001)
- Applied coupon then reduced cart below minimum — coupon stayed applied ❌ 
- Removed coupon product from cart — discount remained in totals ❌ (orphaned discount)
- Tested Unicode coupon code "SAVE10 " (trailing space) — still applied ⚠️ (security concern)

**Edge Cases Found:**
- Orphaned coupon discount when qualifying product removed
- Trailing/leading spaces in coupon code ignored (good: lenient; bad: potential bypass)
- Flat discount coupon + 100% off coupon → negative total

---
