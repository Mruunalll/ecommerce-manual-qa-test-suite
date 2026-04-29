# 🛒 E-Commerce Manual QA Portfolio
### WooCommerce Web + Mobile Testing — End-to-End Manual QA

[![Test Cases](https://img.shields.io/badge/Test%20Cases-35-blue)]()
[![Bugs Found](https://img.shields.io/badge/Bugs%20Found-12-red)]()
[![Pass Rate](https://img.shields.io/badge/Pass%20Rate-65.7%25-yellow)]()
[![Platform](https://img.shields.io/badge/Platform-Web%20%2B%20Mobile-green)]()

## 📌 Project Summary
Executed a full manual QA cycle on a WooCommerce e-commerce storefront, covering authentication, product catalog, product detail pages, cart, checkout, order management, and responsive behaviour across web and mobile platforms. Identified 12 defects, including Critical issues with financial and UX impact.

## 🎯 What Was Tested
| Module | Test Cases | Bugs Found |
|--------|-----------:|-----------:|
| Authentication | 7 | 2 |
| Product Catalog | 5 | 1 |
| Product Detail Page | 6 | 2 |
| Shopping Cart | 7 | 3 |
| Checkout | 7 | 3 |
| Order Management | 2 | 0 |
| Mobile / Responsive | 1 | 1 |

## 🧪 Testing Types Applied
- Functional Testing
- Boundary Value Analysis
- Negative Testing
- Exploratory Testing using SBTM charters
- Usability Testing
- Compatibility Testing across Chrome, Firefox, Safari, and Edge
- Mobile Testing on iOS Safari and Android Chrome

## 🔴 Critical Defects Identified
| ID | Title | Severity |
|----|-------|----------|
| BUG-001 | Coupon stacking allows order total to go negative | Critical |
| BUG-002 | Out-of-stock product added to cart via direct URL manipulation | Critical |
| BUG-004 | Place Order CTA button hidden behind keyboard on iOS Safari checkout | Critical |

## 📁 Repository Structure
- `/docs` — Test plan and QA checklist
- `/test-cases` — Manual test cases grouped by module
- `/bug-reports` — Individual defect reports plus master bug log
- `/exploratory-testing` — Session-based exploratory charters
- `/rtm` — Requirements Traceability Matrix
- `/test-reports` — Final execution summary
- `/assets/screenshots` — Defect evidence index

## 🛠 Tools Used
| Tool | Purpose |
|------|---------|
| Chrome DevTools | DOM inspection, network monitoring, responsive checks |
| BrowserStack | Real-device mobile validation |
| Jira | Defect tracking workflow |
| Loom | Screen recording for defect evidence |
| Excel | Test case management and execution tracking |

## 👤 Author
**Mrunal** | Manual QA Engineer | [GitHub](https://github.com/Mruunalll)
