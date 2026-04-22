
# Test data

---

## Overview

In this artifact, I define the **Test Data** needed to run the **Test Cases** from the **Test Conditions**.

I specify the data used to check positive, negative, and boundary scenarios, based on the Test Basis.

---

## Objective

- I define the data needed to run the Test Cases
- I cover positive, negative, and boundary scenarios
- I ensure traceability between Test Case → Test Data
- I keep alignment with the Test Plan and identified risks

---

## Test data

| TD ID | REQ ID | TC ID | Test Case ID | Input data example                                                                                       |
| ----- | ------ | ----- | ------------ | -------------------------------------------------------------------------------------------------------- |
| TD-01 | REQ-01 | TC-01 | TC-01-TC-01  | First Name: Juan / Last Name: Pérez / Email: [juan@test.com](mailto:juan@test.com) / Password: Test1234! |
| TD-02 | REQ-01 | TC-02 | TC-02-TC-01  | First Name: "" / Email: "" / Password: ""                                                                |
| TD-03 | REQ-01 | TC-03 | TC-03-TC-01  | Email: juan@@test                                                                                        |
| TD-04 | REQ-01 | TC-04 | TC-04-TC-01  | Email: [duplicado@test.com](mailto:duplicado@test.com) / Password: Test1234!                             |
| TD-05 | REQ-01 | TC-05 | TC-05-TC-01  | First Name (min): A                                                                                      |
| TD-06 | REQ-01 | TC-05 | TC-05-TC-01  | First Name (max): JuanCarlosMaximilianoTestingQA                                                         |
| TD-07 | REQ-02 | TC-06 | TC-06-TC-01  | Email: [duplicado@test.com](mailto:duplicado@test.com) / Password: Test1234!                             |
| TD-08 | REQ-02 | TC-07 | TC-07-TC-01  | Email: [duplicado@test.com](mailto:duplicado@test.com) / Password: wrong123                              |
| TD-09 | REQ-02 | TC-08 | TC-08-TC-01  | Email: "" / Password: ""                                                                                 |
| TD-10 | REQ-02 | TC-09 | TC-09-TC-01  | Email: [duplicado@test.com](mailto:duplicado@test.com) / Password: Test1234! (user logged in)            |
| TD-11 | REQ-03 | TC-10 | TC-10-TC-01  | Product: "Build your own computer"                                                                       |
| TD-12 | REQ-03 | TC-11 | TC-11-TC-01  | Sort option: Price (Low to High)                                                                         |
| TD-13 | REQ-03 | TC-12 | TC-12-TC-01  | Category: Computers                                                                                      |
| TD-14 | REQ-03 | TC-13 | TC-13-TC-01  | Search: "zzzz-invalid-product"                                                                           |
| TD-15 | REQ-03 | TC-14 | TC-14-TC-01  | Page: 1                                                                                                  |
| TD-16 | REQ-03 | TC-14 | TC-14-TC-01  | Page: last                                                                                               |
| TD-17 | REQ-04 | TC-15 | TC-15-TC-01  | Product: "Build your own computer" / Quantity: 1                                                         |
| TD-18 | REQ-04 | TC-16 | TC-16-TC-01  | Quantity: 2                                                                                              |
| TD-19 | REQ-04 | TC-16 | TC-16-TC-01  | Quantity: 5                                                                                              |
| TD-20 | REQ-04 | TC-17 | TC-17-TC-01  | Product: "Build your own computer" (present in cart)                                                     |
| TD-21 | REQ-04 | TC-18 | TC-18-TC-01  | Quantity: -1                                                                                             |
| TD-22 | REQ-04 | TC-18 | TC-18-TC-01  | Quantity: "abc"                                                                                          |
| TD-23 | REQ-04 | TC-19 | TC-19-TC-01  | Quantity: 0                                                                                              |
| TD-24 | REQ-04 | TC-19 | TC-19-TC-01  | Quantity: 1000                                                                                           |
| TD-25 | REQ-05 | TC-20 | TC-20-TC-01  | Address: Test Street 123 / City: TestCity / Country: Argentina                                           |
| TD-26 | REQ-05 | TC-21 | TC-21-TC-01  | Address: "" / City: ""                                                                                   |
| TD-27 | REQ-05 | TC-22 | TC-22-TC-01  | Checkout step: Billing                                                                                   |
| TD-28 | REQ-05 | TC-22 | TC-22-TC-01  | Checkout step: Shipping                                                                                  |
| TD-29 | REQ-05 | TC-22 | TC-22-TC-01  | Checkout step: Payment                                                                                   |
| TD-30 | REQ-05 | TC-23 | TC-23-TC-01  | ZIP: invalid / Phone: invalid                                                                            |
| TD-31 | REQ-05 | TC-24 | TC-24-TC-01  | Address length: 1 character                                                                              |
| TD-32 | REQ-05 | TC-24 | TC-24-TC-01  | Address length: 255 characters                                                                           |

---

## Rules

- I get the Test Data from the **Test Basis**
- I make sure every data supports at least one **Test Case**
- I cover:
  - Valid inputs
  - Invalid inputs
  - Boundary values
- I reuse data when needed

---

## Traceability

```text
Requirement → Test Condition → Test Case → Test Data
```

---

## Notes

> [!NOTE]
> I define the Test Data based on the observable behavior of the system.

> [!IMPORTANT]
> I do not make assumptions beyond the Test Basis.
