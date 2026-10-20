# Test Plan: E-commerce Web Application

| Field | Detail |
|---|---|
| Project | Ecommerce Web Application |
| Version | 1.0 |
| Prepared by | Sanika Bodhale |
| Date | 2026-10-12|

## 1. Introduction
manually testing the Login, Product and Checkout features of the e-commerce application.

## 2. Objectives
- Verify the application meets functional requirements.
- Identify defects before release.
- Confirm a smooth, secure purchase journey from login to order confirmation.

## 3. Scope
### In Scope
- User registration and login / logout / forgot password
- Product listing, search, filter, sort, product detail page
- Cart management
- Checkout: address, shipping, payment, order confirmation
- Cross-browser and responsive checks

### Out of Scope
- Performance / load testing
- Automated testing
- Third-party payment gateway internals
- Admin panel

## 4. Test Strategy
| Type | Approach |
|---|---|
| Functional | Execute written test cases for each module |
| Negative | Invalid inputs, empty fields, unauthorized access |
| Boundary | Min/max quantity, field length limits |
| UI/Usability | Layout, alignment, messages, navigation |
| Compatibility | Chrome, Firefox, Edge, Safari; mobile and desktop |
| Regression | Run Regression Checklist after each fix/build |
| Exploratory | Time-boxed sessions to find unscripted issues |

## 5. Test Environment
| Item | Detail |
|---|---|
| URL | https://staging.example.com |
| Browsers | Chrome (latest), Firefox (latest), Edge (latest), Safari |
| Devices | Windows 11, macOS, Android, iOS |
| Test Accounts | Provided by team (valid user, locked user, new user) |
| Test Payment | Gateway sandbox cards |

## 6. Entry Criteria
- Requirements are available and signed off.
- Build deployed to the test environment and smoke test passed.
- Test data and accounts are ready.

## 7. Exit Criteria
- 100% of planned test cases executed.
- No open Critical or High severity defects.
- At least 95% of test cases passed.
- Test summary report shared.

## 8. Defect Management
- Defects are logged using `Bug-Reports/Bug_Report_Template.md`.
- Lifecycle: New → Assigned → In Progress → Fixed → Retest → Closed / Reopened.

| Severity | Meaning |
|---|---|
| Critical | System crash, payment or data loss, no workaround |
| High | Major feature broken, workaround difficult |
| Medium | Feature partly broken, workaround exists |
| Low | Cosmetic or minor issue |

## 9. Deliverables
- Test Plan
- Test Cases (Login, Product, Checkout)
- Bug Reports
- Regression Checklist
- Test Summary Report

## 10. Schedule
| Activity | Duration |
|---|---|
| Test planning | 2 days |
| Test case design | 4 days |
| Test execution (cycle 1) | 5 days |
| Defect retest and regression | 3 days |
| Reporting | 1 day |

## 11. Risks and Mitigation
| Risk | Mitigation |
|---|---|
| Unstable test environment | Daily smoke test; raise with DevOps early |
| Requirement changes | Track changes, update test cases promptly |
| Payment sandbox downtime | Use backup test cards; reschedule payment tests |
| Tight deadlines | Prioritise High priority test cases first |

## 12. Roles
| Role | Responsibility |
|---|---|
| QA Tester | Design and execute tests, log defects |
| Developer | Fix defects |
| Product Owner | Clarify requirements, accept release |
