# Test Plan: Swag Labs (saucedemo.com)

| Field | Value |
|---|---|
| Project | Swag Labs demo shop |
| Prepared by | Jenith Bhatta |
| Version | 1.0 |
| Date | DATE |

## 1. Objective
Verify that the main user journey (login, browse, cart, checkout, logout) works correctly and that errors are handled sensibly.

## 2. Scope
**In scope:** login and logout, product listing and sorting, product details, shopping cart, checkout (3 steps), side menu.
**Out of scope:** performance and load testing, security testing, mobile apps, payment integration (none exists in the demo).

## 3. Test approach
- Manual functional testing from written test cases
- Negative testing with invalid and missing inputs
- Exploratory testing with the special users (`problem_user`, `performance_glitch_user`)
- Defects logged using the template in `bug-reports.md`

## 4. Test environment
- Chrome (latest), Windows 11
- Internet connection
- URL: https://www.saucedemo.com

## 5. Entry criteria
- Site is reachable
- Test accounts are available
- Test cases are reviewed

## 6. Exit criteria
- All planned test cases executed
- All critical and high defects reported
- Results recorded in `test-cases.md`

## 7. Severity levels
| Level | Meaning |
|---|---|
| Critical | Main flow blocked, no workaround |
| High | Major feature broken, workaround exists |
| Medium | Feature partly wrong |
| Low | Cosmetic issue |

## 8. Risks
- The site is a shared demo and may change without notice
- Special users are designed to behave incorrectly, so their results need separate review
