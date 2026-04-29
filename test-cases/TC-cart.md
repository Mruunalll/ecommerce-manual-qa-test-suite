# TC cart

| TC ID | Module | Title | Preconditions | Test Steps | Expected Result | Priority | Severity |
|-------|--------|-------|---------------|------------|-----------------|----------|----------|
| TC-019 | Cart | Update quantity in cart | Product in cart | 1. Go to cart 2. Change quantity from 1 to 3 3. Click Update | Subtotal updates to 3× unit price; totals recalculate | High | Critical |
| TC-020 | Cart | Remove item from cart | Product in cart | 1. Go to cart 2. Click ✕ on product row | Item removed; if last item, empty cart message shown | High | Major |
| TC-021 | Cart | Apply valid 10% off coupon | Valid coupon "SAVE10" exists | 1. Go to cart 2. Enter "SAVE10" 3. Click Apply | 10% deducted from subtotal; coupon shown in totals section | High | Critical |
| TC-022 | Cart | Apply expired coupon | Coupon "EXPIRED20" past end date | 1. Enter "EXPIRED20" 2. Click Apply | Error: "This coupon has expired" | High | Major |
| TC-023 | Cart | Apply invalid coupon code | None | 1. Enter "FAKECODE" 2. Click Apply | Error: "Coupon "FAKECODE" does not exist" | Medium | Minor |
| TC-024 | Cart | Apply coupon below minimum order | Coupon requires $100 min; cart = $40 | 1. Apply coupon 2. Cart total is $40 | Error: "The minimum spend for this coupon is $100" | Medium | Major |
| TC-025 | Cart | Apply two valid coupons | Two valid coupons exist | 1. Apply "SAVE10" 2. Apply "FREESHIP" | If stacking not allowed: error; if allowed: both applied; price must not go negative | High | Critical |
