# Test Plan

## Project Overview

### Application Description
A full-featured e-commerce storefront built on WooCommerce. Sells physical and digital products. Supports multiple payment gateways (Stripe, PayPal, COD), coupon/discount system, guest and registered checkout, order tracking, and wishlist functionality.

### Scope

#### ✅ In-Scope
- User registration, login, logout, password reset
- Product listing, search, filtering, sorting, pagination
- Product detail page (variants, gallery, stock, reviews)
- Shopping cart (add, update, remove, coupon application)
- Checkout (guest + registered, address, shipping, payment)
- Order confirmation, order history, order cancellation
- Responsive/mobile layout (iOS + Android)
- Cross-browser compatibility (Chrome, Firefox, Safari, Edge)

#### ❌ Out-of-Scope
- WooCommerce admin panel / backend configuration
- Payment gateway processing (test mode only)
- Third-party plugins not bundled with core WooCommerce
- Performance/load testing
- Automated testing scripts

### Test Environment

| Category | Details |
|----------|---------|
| Browsers | Chrome 124, Firefox 125, Safari 17, Edge 124 |
| OS | Windows 11, macOS Sonoma, Ubuntu 22 |
| Mobile Devices | iPhone 14 (iOS 17, Safari), Samsung Galaxy S23 (Android 14, Chrome) |
| Screen Sizes | 1920×1080, 1366×768, 768×1024 (tablet), 390×844 (mobile) |
| Network | 4G (throttled via DevTools), WiFi |
| Test Data | Staging environment with seeded products, test accounts |
| Payment | Stripe test cards (4242...) + PayPal Sandbox |

---

## Test Strategy

### Testing Types

| Type | Description |
|------|-------------|
| **Functional** | Verify all features work as per requirements |
| **Regression** | Re-test fixed bugs + core flows after any build change |
| **Exploratory** | Unscripted sessions around cart, checkout, and coupon modules |
| **Usability** | Nielsen heuristics applied to checkout and product pages |
| **Compatibility** | Cross-browser + cross-device rendering and behaviour |
| **Boundary Value** | Quantity fields, price inputs, coupon min/max orders |
| **Negative Testing** | Invalid inputs, expired coupons, OOS products, SQL injection in search |

### Approach
1. Review requirements/user stories (or derive from live site behaviour)
2. Create test scenarios per module
3. Write detailed test cases (positive + negative + edge)
4. Execute in priority order: Critical flows first (checkout > cart > login)
5. Log defects in Jira with screenshots and steps
6. Exploratory sessions after scripted runs
7. Regression on bug fixes before sign-off

### Risk Areas & Mitigation

| Risk | Likelihood | Mitigation |
|------|-----------|------------|
| Coupon calculation errors | High | Boundary + combination testing |
| Payment gateway failures | High | Use Stripe test cards; verify all response states |
| Mobile checkout UX breaks | High | Test on real devices, not only DevTools |
| Cart state lost on session timeout | Medium | Test session expiry scenarios |
| OOS product still purchasable | Medium | Direct URL manipulation tests |
| Cross-browser CSS differences | Medium | Visual testing on all 4 browsers |

---
