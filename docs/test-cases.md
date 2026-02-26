# Test Cases – SauceDemo

## TC-LOG-001 – Valid login (standard_user)
**Preconditions:** User is on login page  
**Steps:**
1. Enter username: standard_user
2. Enter password: secret_sauce
3. Click Login
**Expected:** Inventory page is displayed

## TC-LOG-006 – Username with trailing spaces
**Preconditions:** User is on login page  
**Steps:**
1. Enter username: "standard_user  " (two trailing spaces)
2. Enter password: secret_sauce
3. Click Login
**Expected:** Username should be trimmed OR a clear validation message is shown

## TC-CHK-005 – Invalid ZIP code format
**Preconditions:** Logged in as standard_user, at least 1 item in cart  
**Steps:**
1. Open Cart → Checkout
2. Enter First Name: John
3. Enter Last Name: Doe
4. Enter ZIP: abc
5. Click Continue
**Expected:** Error shown: ZIP must be valid format (e.g., numeric)
