# Test Cases

---

## Overview

In this artifact, I define the **Test Cases** derived from the **Test Conditions**.

I describe how I validate each scenario using clear steps, executable steps, and verifiable expected results, based on the Test Basis.

---

## Objective

- I transform Test Conditions into Test Cases
- I define executable test scenarios
- I ensure traceability between Test Condition → Test Case
- I keep alignment with the Test Plan and the identified risks

---

## Test Cases

| TC ID  | Test Case ID     | Description                                                        | Preconditions                     | Test Steps                                                                                                                                                                                                                    | Test Data            | Expected Result                                                           | Priority | Risk  |
|--------|------------------|--------------------------------------------------------------------|------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------|----------------------------------------------------------------------------|----------|-------|
| TC-01  | TC-01-TC-01      | Validate registration with valid mandatory fields                  | User on registration page          | 1. Enter valid first name<br>2. Enter valid last name<br>3. Enter valid email (e.g., [user@test.com](mailto:user@test.com))<br>4. Enter valid password<br>5. Confirm password<br>6. Submit form                             | Valid data           | User is registered correctly                                               | High     | R-01  |
| TC-02  | TC-02-TC-01      | Validate error when mandatory fields are empty                     | User on registration page          | 1. Leave mandatory fields empty<br>2. Submit form                                                                                                                                      | Empty data           | Message "First name is required." and "Email is required." is shown        | High     | R-01  |
| TC-03  | TC-03-TC-01      | Validate error with invalid email format                           | User on registration page          | 1. Enter invalid email (e.g., juan@@test)<br>2. Fill in other fields with valid data<br>3. Submit form                                                                              | Invalid email        | Message "Wrong email" is shown                                             | High     | R-01  |
| TC-04  | TC-04-TC-01      | Validate error with duplicate data                                | User on registration page          | 1. Enter already registered email<br>2. Complete form<br>3. Submit                                                                             | Existing email        | Duplicate registration error message is shown                              | High     | R-01  |
| TC-05  | TC-05-TC-01      | Validate boundary conditions in registration fields                | User on registration page          | 1. Enter minimum/maximum values<br>2. Submit form                                                                                              | Boundary data         | System validates the limits correctly                                      | Medium   | R-01  |
| TC-06  | TC-06-TC-01      | Validate login with valid credentials                             | User on login page                 | 1. Enter valid email<br>2. Enter valid password<br>3. Submit                                                                                   | Valid credentials     | User logs in correctly                                                     | High     | R-02  |
| TC-07  | TC-07-TC-01      | Validate login with invalid credentials                           | User on login page                 | 1. Enter incorrect credentials<br>2. Submit                                                                                                    | Invalid credentials   | "Login was unsuccessful. Please correct the errors and try again." is shown | High     | R-02  |
| TC-08  | TC-08-TC-01      | Validate login with empty fields                                  | User on login page                 | 1. Leave fields empty<br>2. Submit                                                                                                             | Empty data            | Error message is shown                                                     | High     | R-02  |
| TC-09  | TC-09-TC-01      | Validate session behavior                                         | Logged in user                     | 1. Navigate inside the system                                                                                                                   | Valid session          | The session stays active correctly                                         | Medium   | R-02  |
| TC-10  | TC-10-TC-01      | Validate product list display                                    | User on catalog                    | 1. Access catalog                                                                                                                              | N/A                   | Products are visible on screen                                             | Medium   | R-03  |
| TC-11  | TC-11-TC-01      | Validate product sorting                                         | User on catalog                    | 1. Apply sorting option                                                                                                                        | Sort option          | Products are sorted correctly                                              | Medium   | R-03  |
| TC-12  | TC-12-TC-01      | Validate product filtering                                       | User on catalog                    | 1. Apply filter                                                                                                                                 | Selected filter         | Products are filtered correctly                                            | Medium   | R-03  |
| TC-13  | TC-13-TC-01      | Validate behavior with no results                               | User on catalog                    | 1. Apply filter with no match                                                                                                                   | Invalid filter        | Message with no results is shown                                           | Medium   | R-03  |
| TC-14  | TC-14-TC-01      | Validate pagination                                             | User on catalog                    | 1. Navigate between pages                                                                                                                       | N/A                   | Pagination works correctly                                                 | Medium   | R-03  |
| TC-15  | TC-15-TC-01      | Validate adding product to cart                                 | Logged in user                      | 1. Select product<br>2. Add to cart                                                                                                             | Valid product         | Product added to cart                                                      | High     | R-04  |
| TC-16  | TC-16-TC-01      | Validate update of quantity                                    | User with cart                      | 1. Change quantity                                                                                                                              | Valid quantity         | Quantity updated correctly                                                 | High     | R-04  |
| TC-17  | TC-17-TC-01      | Validate remove product                                        | User with cart                      | 1. Remove product                                                                                                                               | N/A                   | Product is removed from cart                                               | High     | R-04  |
| TC-18  | TC-18-TC-01      | Validate invalid quantity                                      | User with cart                      | 1. Enter invalid quantity (e.g., -1)                                                                                                            | Invalid quantity        | Error message is shown                                                     | High     | R-04  |
| TC-19  | TC-19-TC-01      | Validate quantity limits                                       | User with cart                      | 1. Enter boundary values                                                                                                                        | Boundary data         | System validates correctly                                                 | Medium   | R-04  |
| TC-20  | TC-20-TC-01      | Validate successful checkout                                   | User with cart                      | 1. Start checkout<br>2. Complete steps<br>3. Confirm                                                                                            | Valid data           | Order completed correctly                                                  | High     | R-05  |
| TC-21  | TC-21-TC-01      | Validate error for missing data in checkout                    | User on checkout                    | 1. Skip required data<br>2. Continue                                                                                                            | Incomplete data        | System asks to complete data                                               | High     | R-05  |
| TC-22  | TC-22-TC-01      | Validate navigation in checkout                               | User on checkout                    | 1. Go forward and back between steps                                                                                                            | N/A                   | Correct navigation between steps                                           | Medium   | R-05  |
| TC-23  | TC-23-TC-01      | Validate invalid data in checkout                             | User on checkout                    | 1. Enter invalid data<br>2. Continue                                                                                                            | Invalid data           | Error message is shown                                                     | High     | R-05  |
| TC-24  | TC-24-TC-01      | Validate boundaries in checkout                               | User on checkout                    | 1. Use boundary values                                                                                                                          | Boundary data         | Correct validation                                                         | Medium   | R-05  |

---

## Rules

- I derive each Test Case from a **[Test Condition](../01-test-analysis/test-conditions.md)**
- I define one scenario per Test Case
- I write clear and executable steps
- I define verifiable expected results
- I assign priority based on risks of the Test Plan
- I include reference to **Risk ID**
- I avoid duplicated Test Cases
- I ensure the Test Cases are atomic and traceable

---

## Traceability

```text
Requirement → Test Condition → Test Case → Test Data
```

---

## Notes

> [!NOTE]
> I design the Test Cases based on the Test Basis and the observable system behavior.

> [!IMPORTANT]
> I do not make assumptions beyond the Test Basis.
