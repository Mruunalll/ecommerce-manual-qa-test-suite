# TC auth

| TC ID | Module | Title | Preconditions | Test Steps | Expected Result | Priority | Severity |
|-------|--------|-------|---------------|------------|-----------------|----------|----------|
| TC-001 | Auth | Register with valid new email | Site accessible; user not previously registered | 1. Go to /register 2. Enter valid name, unique email, strong password 3. Click Register | Account created; user redirected to My Account; welcome email received | High | Critical |
| TC-002 | Auth | Register with duplicate email | Existing account with same email | 1. Go to /register 2. Enter existing email 3. Click Register | Error: "An account is already registered with your email address" | High | Major |
| TC-003 | Auth | Register with weak password | None | 1. Enter valid email 2. Enter password "123" 3. Click Register | Password strength indicator shows "Weak"; form blocks submission | Medium | Major |
| TC-004 | Auth | Login with valid credentials | Account exists | 1. Go to /my-account 2. Enter correct email + password 3. Click Login | User authenticated; redirected to My Account dashboard | High | Critical |
| TC-005 | Auth | Login with wrong password | Account exists | 1. Enter correct email 2. Enter wrong password 3. Click Login | Error: "The password you entered is incorrect" | High | Major |
| TC-006 | Auth | Password reset flow | Account exists; email accessible | 1. Click "Forgot Password" 2. Enter registered email 3. Check email 4. Click reset link 5. Enter new password | Password updated; user can login with new password | High | Critical |
| TC-007 | Auth | Session persists after browser reopen | User logged in | 1. Login 2. Close browser 3. Reopen and go to site | User remains logged in (if remember me checked) | Medium | Minor |
