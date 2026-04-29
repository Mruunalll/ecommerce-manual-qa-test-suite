# TC checkout

| TC ID | Module | Title | Preconditions | Test Steps | Expected Result | Priority | Severity |
|-------|--------|-------|---------------|------------|-----------------|----------|----------|
| TC-026 | Checkout | Guest checkout — complete order | Cart has item; no login | 1. Go to checkout 2. Fill all fields as guest 3. Pay via Stripe test card | Order placed; confirmation page shown; confirmation email sent | High | Critical |
| TC-027 | Checkout | Registered user — autofill address | User has saved address | 1. Login 2. Add to cart 3. Go to checkout | Saved billing/shipping address pre-filled | Medium | Minor |
| TC-028 | Checkout | Required field validation | Checkout page | 1. Leave "First Name" blank 2. Click Place Order | Inline error: "Billing First name is a required field" | High | Major |
| TC-029 | Checkout | Invalid email format in checkout | Checkout page | 1. Enter "notanemail" in email field 2. Place Order | Validation error on email field | High | Major |
| TC-030 | Checkout | Payment — Stripe card declined | Checkout with items | 1. Use Stripe test card 4000 0000 0000 0002 | Error: "Your card was declined"; order NOT created | High | Critical |
| TC-031 | Checkout | Payment — Stripe insufficient funds | Checkout with items | 1. Use card 4000 0000 0000 9995 | Error: "Insufficient funds"; order NOT created | High | Major |
| TC-032 | Checkout | Shipping method change updates total | Two shipping methods available | 1. Select "Standard Shipping" 2. Note total 3. Switch to "Express Shipping" | Total updates to reflect correct shipping cost | High | Major |
