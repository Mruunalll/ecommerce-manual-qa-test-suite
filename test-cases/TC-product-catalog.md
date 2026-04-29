# TC product catalog

| TC ID | Module | Title | Preconditions | Test Steps | Expected Result | Priority | Severity |
|-------|--------|-------|---------------|------------|-----------------|----------|----------|
| TC-008 | Product Catalog | Search for existing product | Products exist in catalog | 1. Type product name in search bar 2. Press Enter | Relevant products displayed; search term highlighted or shown | High | Major |
| TC-009 | Product Catalog | Search with no matching results | None | 1. Search for "xyznotexist123" | "No products were found" message shown; no broken layout | Medium | Minor |
| TC-010 | Product Catalog | Filter by price range | Products with varying prices exist | 1. Go to shop 2. Set price slider min=$10 max=$50 3. Apply | Only products within $10–$50 displayed; count updates | High | Major |
| TC-011 | Product Catalog | Sort by Price: Low to High | Multiple products with different prices | 1. Go to shop 2. Select "Sort by price: low to high" | Products ordered ascending by price; no gaps or duplicates | High | Major |
| TC-012 | Product Catalog | Pagination — navigate to page 2 | >12 products in catalog | 1. Go to shop page 1 2. Click "2" in pagination | Page 2 loads; different products shown; URL updates (?paged=2) | Medium | Minor |
| TC-013 | PDP | Add in-stock product to cart | Product is in stock | 1. Go to product page 2. Click "Add to Cart" | "Added to cart" notice appears; cart icon count increments | High | Critical |
| TC-014 | PDP | Select product variant — size | Configurable product with sizes | 1. Go to product page 2. Select Size: "L" 3. Note price change | Correct price and stock for size "L" shown; Add to Cart enabled | High | Major |
| TC-015 | PDP | Attempt to add OOS product | Product variant is out of stock | 1. Go to product page 2. Select OOS variant | "Out of Stock" label shown; Add to Cart button disabled | High | Critical |
| TC-016 | PDP | Quantity field — enter 0 | In-stock product | 1. On PDP set quantity to 0 2. Click Add to Cart | Validation error: "Please enter a quantity greater than 0" | High | Major |
| TC-017 | PDP | Quantity field — enter negative number | In-stock product | 1. Set quantity to -5 2. Click Add to Cart | Input rejected; error shown or value resets to 1 | High | Major |
| TC-018 | PDP | Quantity field — exceed stock | Product stock = 3 | 1. Set quantity to 99 2. Add to Cart | Error: "You cannot add that quantity. Only 3 in stock." | Medium | Major |
