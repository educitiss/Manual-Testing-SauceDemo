# Test Cases – SauceDemo

## TC-LOG-001 – Valid login (standard_user)

**Preconditions:**  
User is on login page

**Steps:**
1. Enter username: standard_user
2. Enter password: secret_sauce
3. Click Login

**Expected Result:**  
Inventory page is displayed.

**Actual Result:**  
Inventory page loaded successfully.

**Status:**  
Pass

## TC-LOG-002 – Login with invalid password

**Preconditions:**  
User is on login page

**Steps:**
1. Enter username: standard_user
2. Enter password: wrong_password
3. Click Login

**Expected Result:**  
Error message should be displayed indicating invalid credentials.

**Actual Result:**  
Error message displayed:  
"Epic sadface: Username and password do not match any user in this service"

**Status:**  
Pass

## TC-LOG-003 – Login with empty username

**Preconditions:**  
User is on login page

**Steps:**
1. Leave username field empty
2. Enter password: secret_sauce
3. Click Login

**Expected Result:**  
Error message should be displayed indicating that username is required.

**Actual Result:**  
Error message displayed:  
"Epic sadface: Username is required"

**Status:**  
Pass

## TC-LOG-004 – Login with empty password

**Preconditions:**  
User is on login page

**Steps:**
1. Enter username: standard_user
2. Leave password field empty
3. Click Login

**Expected Result:**  
Error message should be displayed indicating that password is required.

**Actual Result:**  
Error message displayed:  
"Epic sadface: Password is required"

**Status:**  
Pass

## TC-LOG-005 – Login with both fields empty

**Preconditions:**  
User is on login page

**Steps:**
1. Leave username field empty
2. Leave password field empty
3. Click Login

**Expected Result:**  
Error message should be displayed indicating that username is required.

**Actual Result:**  
Error message displayed:  
"Epic sadface: Username is required"

**Status:**  
Pass

## TC-LOG-006 – Username with trailing spaces

**Preconditions:**  
User is on login page

**Steps:**
1. Enter username: "standard_user  " (two trailing spaces)
2. Enter password: secret_sauce
3. Click Login

**Expected Result:**  
System should trim whitespace or display validation error.

**Actual Result:**  
Login fails when trailing spaces are present.

**Status:**  
Fail

**Linked Defect:**  
Issue #2 – Login does not handle username with trailing spaces correctly

## TC-INV-001 – Inventory page loads after login

**Preconditions:**  
User is on login page

**Steps:**
1. Enter username: standard_user
2. Enter password: secret_sauce
3. Click Login

**Expected Result:**  
User is redirected to inventory page and product list is displayed.

**Actual Result:**  
Inventory page loaded successfully and products were displayed.

**Status:**  
Pass

## TC-INV-002 – Add item to cart from inventory

**Preconditions:**  
User is logged in and on inventory page.

**Steps:**
1. Locate any product on the inventory page.
2. Click "Add to cart".

**Expected Result:**  
Item should be added to cart and cart badge should increase.

**Actual Result:**  
Item was added successfully and cart badge displayed "1".

**Status:**  
Pass

## TC-CHK-005 – Invalid ZIP code format

**Preconditions:**  
Logged in as standard_user, at least 1 item in cart

**Steps:**
1. Open Cart → Checkout
2. Enter First Name: John
3. Enter Last Name: Doe
4. Enter ZIP: abc
5. Click Continue

**Expected Result:**  
Error should be displayed indicating invalid ZIP format.

**Actual Result:**  
User was allowed to proceed to the next checkout step.

**Status:**  
Fail

**Linked Defect:**  
Issue #1 – Checkout allows non-numeric ZIP code

## TC-SORT-001 – Verify sorting by price (low to high)

**Preconditions:**  
User logged in as standard_user

**Steps:**
1. Open inventory page
2. Select "Price (low to high)" in sorting dropdown
3. Observe product prices
4. Refresh page
5. Observe product prices

**Expected Result:**  
Products sorted in ascending price order.

**Actual Result:**  
Products appear correctly sorted until refreshed.

**Status:**  
Fail
