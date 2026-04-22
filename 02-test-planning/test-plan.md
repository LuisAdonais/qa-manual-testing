# 📄 Test plan

---

## 1. Introduction

### Purpose

In this document, I define the testing approach based on the **Test Basis** and the analysis done on the application.

My goal is to validate the main functionalities by observing the real behavior of the system.

---

## 2. Test objectives

During the analysis of the application, I identified that I must validate:

- User registration (`REQ-01`)
- Login (`REQ-02`)
- Product navigation (`REQ-03`)
- Cart management (`REQ-04`)
- Checkout process (`REQ-05`)

For each Requirement, I will cover the defined Test Conditions:

- `REQ-01` → `TC-01` → `TC-05`
- `REQ-02` → `TC-06` → `TC-09`
- `REQ-03` → `TC-10` → `TC-14`
- `REQ-04` → `TC-15` → `TC-19`
- `REQ-05` → `TC-20` → `TC-24`

I also want to cover:

- Positive scenarios
- Negative scenarios
- Boundary conditions

---

## 3. Scope

### In scope

| REQ ID   | TC coverage        |
|----------|-------------------|
| `REQ-01` | `TC-01` → `TC-05` |
| `REQ-02` | `TC-06` → `TC-09` |
| `REQ-03` | `TC-10` → `TC-14` |
| `REQ-04` | `TC-15` → `TC-19` |
| `REQ-05` | `TC-20` → `TC-24` |

---

### Out of scope

- Functionalities not defined in the Test Basis
- External integrations not specified

---

## 4. Test strategy

I will apply:

- Testing based on risks identified in the Requirement analysis
- Functional validation of the main flows

I focus on:

- Undefined validations
- Ambiguities in behavior
- Detected functional risks

---

## 5. Test approach

During the analysis of the page:

- I navigated the main flows
- I tested valid and invalid data
- I observed system behavior and error messages

I will execute:

- `TC-01` → `TC-24`

Combining:

- Structured testing (based on Test Conditions)
- Exploratory testing

---

## 6. Test items (test objects)

| ID      | Description           | REQ      |
|---------|-----------------------|----------|
| `TI-01` | Registration          | `REQ-01` |
| `TI-02` | Login                 | `REQ-02` |
| `TI-03` | Product catalog       | `REQ-03` |
| `TI-04` | Cart                  | `REQ-04` |
| `TI-05` | Checkout              | `REQ-05` |

---

## 7. Entry criteria

To start testing I need:

- Defined Test Basis (`REQ`, `TC`, `RTM`)
- Access to the application available
- Accessible environment

---

## 8. Exit criteria

I consider testing finished when:

- I execute 100% of the Test Conditions
- No critical Defects are left open
- I have documented all results

---

## 9. Test environment

| Element    | Value        |
|------------|-------------|
| Environment| Public web   |
| Browser    | Firefox     |
| Device     | Desktop     |

---

## 10. Roles and responsibilities

| Role      | Responsibility                   |
|-----------|----------------------------------|
| QA Tester | Design and execution of tests    |

---

## 11. Test schedule

| Phase           | Status   |
|-----------------|----------|
| Test planning   | Done     |
| Test design     | Pending  |
| Test execution  | Pending  |

---

## 12. Risks

During the analysis, I identified the following risks:

| Risk ID | Description                                      | Impact |
|---------|--------------------------------------------------|--------|
| `R-01`  | Undefined validations in registration (`REQ-01`) | High   |
| `R-02`  | Login behavior not clearly defined (`REQ-02`)    | High   |
| `R-03`  | Ambiguous filters and pagination (`REQ-03`)      | Medium |
| `R-04`  | Quantity rules not defined (`REQ-04`)            | High   |
| `R-05`  | Incomplete or unclear checkout flow (`REQ-05`)   | High   |

---

## 13. Assumptions

During the analysis, I assumed:

- The system uses standard validations
- The payment is simulated
- The system is available publicly

---

## 14. Test monitoring and control

I will:

- Record the progress for each Test Condition execution
- Monitor Defects found

---

## 15. Deliverables

- Test plan
- Test cases
- Test execution report
- Defect reports
- Test summary report

---

## 16. System observations

During the analysis of the page I observed:

- In the registration form, when I leave required fields empty, the system shows error messages like:
  - "First name is required."
  - "Email is required."

- When I enter an invalid email format (example: `juan@@test`), the system shows the message:
  - "Wrong email"

- In login, when I enter incorrect credentials, the system shows:
  - "Login was unsuccessful. Please correct the errors and try again."

- In the product catalog, I can navigate between pages using visible pagination controls in the interface

- In the cart, I can add and remove products from the cart view

- During the checkout process, the system requires completing information in each step before moving to the next

---

> [!IMPORTANT]
> All testing is based on the Test Basis and on observable system behavior.

> [!NOTE]
> Traceability is maintained:
> `REQ` → `TC` → `Test Case` → `Test Execution` → `Defect`