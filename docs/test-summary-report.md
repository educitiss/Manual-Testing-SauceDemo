# Test Summary Report – SauceDemo

## Project
Manual QA Testing – SauceDemo

Application: https://www.saucedemo.com  
Tester: [Your Name]  
Browser: Chrome  
OS: Windows  
Test Type: Manual Functional Testing  

---

## Scope of Testing

The following core features were tested:

- Login functionality
- Product inventory
- Cart operations
- Checkout process
- Input validation

Testing included both positive and negative scenarios.

---

## Test Execution Summary

| Metric | Count |
|------|------|
| Total Test Cases | 3 |
| Passed | 1 |
| Failed | 2 |
| Blocked | 0 |

---

## Defects Found

| Issue ID | Title | Severity | Priority |
|--------|------|--------|--------|
| #1 | Checkout allows non-numeric ZIP code | Medium | P2 |
| #2 | Login does not handle username with trailing spaces | Low | P3 |

---

## Observations

- Core functionality works as expected for valid user flows.
- Input validation needs improvement for ZIP code.
- Login input handling could be improved to trim whitespace.

---

## Recommendations

- Implement input validation for ZIP code format.
- Trim leading and trailing whitespace in login fields.
- Expand validation tests for other checkout fields.

---

## Conclusion

Testing identified issues related to input validation and edge case handling.  
The application generally functions correctly for standard user flows but would benefit from stronger input validation mechanisms.
