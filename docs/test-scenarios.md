# Test Scenarios – SauceDemo

App: https://www.saucedemo.com  
Scope: Login, Inventory, Cart, Checkout, Logout

## Login
- TS-LOG-001 Login with valid credentials (standard_user)
- TS-LOG-002 Login with invalid password
- TS-LOG-003 Login with empty username
- TS-LOG-004 Login with empty password
- TS-LOG-005 Login with both fields empty
- TS-LOG-006 Username with trailing spaces

## Inventory
- TS-INV-001 Inventory page loads after login
- TS-INV-002 Add item to cart from inventory
- TS-INV-003 Remove item from inventory
- TS-INV-004 Sort products (Name A-Z, Z-A, Price low-high, high-low)

## Cart
- TS-CAR-001 Cart shows added items correctly
- TS-CAR-002 Remove item from cart
- TS-CAR-003 Continue shopping returns to inventory

## Checkout
- TS-CHK-001 Checkout with valid details
- TS-CHK-002 Checkout with missing first name
- TS-CHK-003 Checkout with missing last name
- TS-CHK-004 Checkout with missing zip
- TS-CHK-005 Checkout with invalid zip format

## Logout
- TS-OUT-001 Logout from menu
