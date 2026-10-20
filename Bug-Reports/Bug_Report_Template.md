# Bug Report

| Field | Detail |
|---|---|
| **Bug ID** | BUG-001 |
| **Title** | Short, clear summary of the issue |
| **Module** | Login / Product / Cart / Checkout |
| **Reported By** | Your Name |
| **Date Reported** | YYYY-MM-DD |
| **Build / Version** | v1.0.0 |
| **Environment** | Staging · Windows 11 · Chrome 120 |
| **Severity** | Critical / High / Medium / Low |
| **Priority** | P1 / P2 / P3 / P4 |
| **Status** | New / Assigned / In Progress / Fixed / Retest / Closed / Reopened |
| **Assigned To** | Developer name |
| **Related Test Case** | e.g. CHK-007 |

## Description
Brief explanation of what went wrong.

## Preconditions
- User is logged in
- Cart contains 1 item

## Steps to Reproduce
1. Go to ...
2. Click on ...
3. Enter ...
4. Observe ...

## Expected Result
What should happen.

## Actual Result
What actually happened.

## Reproducibility
Always / Sometimes / Rarely (e.g. 3 out of 3 attempts)

## Attachments
- Screenshot: `screenshots/bug-001.png`
- Video: `videos/bug-001.mp4`
- Console / network logs

## Additional Notes
Workaround, browser differences, related bugs.

---

## Severity vs Priority Guide

| Severity | Description | Example |
|---|---|---|
| Critical | Blocks core functionality, no workaround | Payment charged but order not created |
| High | Major feature fails | Cannot add items to cart |
| Medium | Partial failure, workaround exists | Filter fails but search works |
| Low | Cosmetic | Misaligned button, typo |

| Priority | Meaning |
|---|---|
| P1 | Fix immediately |
| P2 | Fix in current release |
| P3 | Fix in next release |
| P4 | Fix when time permits |

---

## Sample Filled Bug

| Field | Detail |
|---|---|
| Bug ID | BUG-001 |
| Title | Order total not updated after removing item from cart |
| Module | Cart |
| Severity | High |
| Priority | P2 |
| Steps | 1. Add 2 products. 2. Open cart. 3. Remove one product. |
| Expected | Total reflects only the remaining product |
| Actual | Total still shows the price of both products until page refresh |
