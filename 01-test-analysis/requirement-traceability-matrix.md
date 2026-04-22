# Requirement traceability matrix

---

## Overview

In this artifact, I define the **Requirement Traceability Matrix (RTM)** to ensure complete traceability between **Requirements**, **Test Conditions**, and **Test Cases**.

I use this matrix to check that all elements from the Test Basis are covered and related correctly.

---

## Objective

- I ensure traceability between Requirement → Test Condition → Test Case
- I check that there are no orphan elements
- I guarantee complete coverage of the system
- I keep consistency with the Test Analysis and Test Design artifacts

---

## RTM

| REQ ID | TC ID | Test Case ID | Description                                       |
| ------ | ----- | ------------ | ------------------------------------------------- |
| REQ-01 | TC-01 | TC-01-TC-01  | Validate registration with valid mandatory fields |
| REQ-01 | TC-02 | TC-02-TC-01  | Validate error when mandatory fields are empty    |
| REQ-01 | TC-03 | TC-03-TC-01  | Validate error with invalid input format          |
| REQ-01 | TC-04 | TC-04-TC-01  | Validate error with duplicate data                |
| REQ-01 | TC-05 | TC-05-TC-01  | Validate boundary conditions for input fields     |
| REQ-02 | TC-06 | TC-06-TC-01  | Validate login with valid credentials             |
| REQ-02 | TC-07 | TC-07-TC-01  | Validate login with invalid credentials           |
| REQ-02 | TC-08 | TC-08-TC-01  | Validate login with empty fields                  |
| REQ-02 | TC-09 | TC-09-TC-01  | Validate session behavior                         |
| REQ-03 | TC-10 | TC-10-TC-01  | Validate product list display                     |
| REQ-03 | TC-11 | TC-11-TC-01  | Validate sorting functionality                    |
| REQ-03 | TC-12 | TC-12-TC-01  | Validate filtering functionality                  |
| REQ-03 | TC-13 | TC-13-TC-01  | Validate behavior when no results are found       |
| REQ-03 | TC-14 | TC-14-TC-01  | Validate pagination boundaries                    |
| REQ-04 | TC-15 | TC-15-TC-01  | Validate adding product to cart                   |
| REQ-04 | TC-16 | TC-16-TC-01  | Validate updating product quantity                |
| REQ-04 | TC-17 | TC-17-TC-01  | Validate removing product from cart               |
| REQ-04 | TC-18 | TC-18-TC-01  | Validate invalid quantity values                  |
| REQ-04 | TC-19 | TC-19-TC-01  | Validate quantity boundary conditions             |
| REQ-05 | TC-20 | TC-20-TC-01  | Validate successful checkout process              |
| REQ-05 | TC-21 | TC-21-TC-01  | Validate error when required data is missing      |
| REQ-05 | TC-22 | TC-22-TC-01  | Validate navigation between checkout steps        |
| REQ-05 | TC-23 | TC-23-TC-01  | Validate error with invalid data during checkout  |
| REQ-05 | TC-24 | TC-24-TC-01  | Validate checkout flow boundary conditions        |

---

## Navigation

I use the following related artifacts:

- Test Conditions → `../01-test-analysis/test-conditions.md`
- Test Cases → `./test-cases.md`

---

## Rules

- I ensure that every Requirement has at least one Test Condition
- I ensure that each Test Condition has at least one Test Case
- I avoid orphan elements
- I keep traceability following the model:

```text
Requirement → Test Condition → Test Case
```

---

## Notes

> [!NOTE]
> I use this matrix to check complete coverage and consistency between artifacts.

> [!IMPORTANT]
> I keep alignment with the Test Basis and do not create relations outside it.
