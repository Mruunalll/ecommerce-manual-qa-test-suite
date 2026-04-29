# High-Level Test Scenarios

## Scenarios

### Module: User Authentication
- S01: Register new user with valid data
- S02: Register with already-used email
- S03: Login with valid credentials
- S04: Login with invalid password (3 attempts → lockout)
- S05: Password reset via email link
- S06: Social login (Google) — if enabled
- S07: Logout clears session

### Module: Product Catalog
- S08: Search returns relevant products
- S09: Search with no results shows appropriate message
- S10: Filter by category, price range, rating
- S11: Sort by price (low-high, high-low), popularity, newness
- S12: Pagination works; URL updates correctly
- S13: Product count badge updates with filters

### Module: Product Detail Page
- S14: All product images load; gallery carousel works
- S15: Variant selection (size, colour) updates price/stock
- S16: OOS variant disables Add to Cart
- S17: Quantity selector respects min=1 and max=stock
- S18: Review submission (logged in vs. guest)
- S19: Breadcrumb navigation correct

### Module: Shopping Cart
- S20: Add single product to cart
- S21: Add multiple products; totals update correctly
- S22: Update quantity in cart; subtotal recalculates
- S23: Remove item from cart
- S24: Apply valid coupon code
- S25: Apply expired/invalid coupon
- S26: Apply two coupons simultaneously
- S27: Cart persists across browser sessions (registered user)
- S28: Empty cart shows correct empty state

### Module: Checkout
- S29: Guest checkout with valid data
- S30: Registered user checkout (saved address autofills)
- S31: Shipping method selection and cost update
- S32: Payment via Stripe (success, decline, insufficient funds)
- S33: Payment via PayPal sandbox
- S34: Order confirmation email received
- S35: Form validation on all required fields
- S36: Address with special characters (accented names)

### Module: Order Management
- S37: View order history (registered user)
- S38: View single order detail
- S39: Cancel pending order
- S40: Download digital product (if applicable)

### Module: Mobile / Responsive
- S41: Navigation menu (hamburger) works on mobile
- S42: Product grid reflows to single column
- S43: Checkout form usable on small screen
- S44: Touch targets meet 44×44px minimum

---
