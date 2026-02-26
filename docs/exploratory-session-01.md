# Exploratory Testing Session 01

Application: https://www.saucedemo.com  
Tester: [Your Name]  
Date: [Today’s Date]  
Browser: Chrome  
Environment: Web  

---

## Objective
Initial exploratory testing of core user flows:
- Login
- Product listing
- Cart behavior
- Checkout process

---

## Areas Explored

### 1. Login Functionality
- Valid login (standard_user)
- Invalid password
- Empty fields
- Username with trailing spaces

Observation:
Username field accepts trailing spaces without clear validation behavior.

---

### 2. Checkout Form Validation
- Missing first name
- Missing last name
- Missing ZIP code
- Non-numeric ZIP input

Observation:
ZIP code format validation appears insufficient.

---

### 3. Cart and Pricing
- Add multiple items
- Remove items
- Verify subtotal recalculation

Observation:
Price calculation needs controlled verification.

---

### 4. Special Test Users
Tested:
- problem_user
- performance_glitch_user

Observed:
UI inconsistencies and incorrect product images (likely intentional for testing).
