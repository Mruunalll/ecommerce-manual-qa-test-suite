# TC order management

| TC ID | Module | Title | Preconditions | Test Steps | Expected Result | Priority | Severity |
|-------|--------|-------|---------------|------------|-----------------|----------|----------|
| TC-033 | Orders | View order history | Registered user with past orders | 1. Login 2. Go to My Account → Orders | All past orders listed with order ID, date, status, total | Medium | Minor |
| TC-034 | Orders | Cancel pending order | Order in "Pending" status | 1. Go to order detail 2. Click Cancel | Order status changes to "Cancelled"; confirmation shown | Medium | Major |
