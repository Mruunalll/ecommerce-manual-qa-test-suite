# Requirements Traceability Matrix

## RTM

| Requirement ID | Requirement Description | Test Case IDs | Status |
|----------------|------------------------|---------------|--------|
| REQ-001 | User must be able to register with email and password | TC-001, TC-002, TC-003 | ✅ Pass |
| REQ-002 | User must be able to login and logout | TC-004, TC-005, TC-007 | ✅ Pass |
| REQ-003 | Password reset must work via email | TC-006 | ✅ Pass |
| REQ-004 | Product search must return relevant results | TC-008, TC-009 | ✅ Pass |
| REQ-005 | Products must be filterable by price and category | TC-010 | ❌ Fail (BUG-010) |
| REQ-006 | Products must be sortable | TC-011 | ✅ Pass |
| REQ-007 | Product variants must show correct price/stock | TC-014, TC-015 | ⚠️ Partial (BUG-006) |
| REQ-008 | Quantity input must validate min/max | TC-016, TC-017, TC-018 | ❌ Fail (BUG-003) |
| REQ-009 | Cart must update correctly | TC-019, TC-020 | ✅ Pass |
| REQ-010 | Coupons must apply and validate correctly | TC-021, TC-022, TC-023, TC-024, TC-025 | ❌ Fail (BUG-001, BUG-005) |
| REQ-011 | Checkout must complete for guest users | TC-026 | ✅ Pass |
| REQ-012 | All checkout fields must validate | TC-028, TC-029 | ✅ Pass |
| REQ-013 | Payment via Stripe must handle success and errors | TC-030, TC-031 | ✅ Pass |
| REQ-014 | Shipping cost must update on method change | TC-032 | ✅ Pass |
| REQ-015 | Order confirmation email must be sent | TC-026 (email check) | ❌ Fail (BUG-008 — PayPal) |
| REQ-016 | Registered users can view order history | TC-033 | ✅ Pass |
| REQ-017 | Pending orders can be cancelled | TC-034 | ✅ Pass |
| REQ-018 | Site must be usable on mobile | TC-035 | ❌ Fail (BUG-004) |

---
