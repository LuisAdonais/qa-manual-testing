# Test conditions

---

## Test conditions

| TC ID   | Description                                       | Type      | Source REQ |
|---------|---------------------------------------------------|-----------|------------|
| TC-01   | Validate registration with valid mandatory fields  | Positive  | REQ-01     |
| TC-02   | Validate error when mandatory fields are empty     | Negative  | REQ-01     |
| TC-03   | Validate error with invalid input format           | Negative  | REQ-01     |
| TC-04   | Validate error with duplicate data                 | Negative  | REQ-01     |
| TC-05   | Validate boundary conditions for input fields      | Boundary  | REQ-01     |
| TC-06   | Validate login with valid credentials              | Positive  | REQ-02     |
| TC-07   | Validate login with invalid credentials            | Negative  | REQ-02     |
| TC-08   | Validate login with empty fields                   | Negative  | REQ-02     |
| TC-09   | Validate session behavior                          | Positive  | REQ-02     |
| TC-10   | Validate product list display                      | Positive  | REQ-03     |
| TC-11   | Validate sorting functionality                     | Positive  | REQ-03     |
| TC-12   | Validate filtering functionality                   | Positive  | REQ-03     |
| TC-13   | Validate behavior when no results are found        | Negative  | REQ-03     |
| TC-14   | Validate pagination boundaries                     | Boundary  | REQ-03     |
| TC-15   | Validate adding product to cart                    | Positive  | REQ-04     |
| TC-16   | Validate updating product quantity                 | Positive  | REQ-04     |
| TC-17   | Validate removing product from cart                | Positive  | REQ-04     |
| TC-18   | Validate invalid quantity values                   | Negative  | REQ-04     |
| TC-19   | Validate quantity boundary conditions              | Boundary  | REQ-04     |
| TC-20   | Validate successful checkout process               | Positive  | REQ-05     |
| TC-21   | Validate error when required data is missing       | Negative  | REQ-05     |
| TC-22   | Validate navigation between checkout steps         | Positive  | REQ-05     |
| TC-23   | Validate error with invalid data during checkout   | Negative  | REQ-05     |
| TC-24   | Validate checkout flow boundary conditions         | Boundary  | REQ-05     |

---

## Rules

- Be clear and testable
- Be derived from a requirement
- Cover:
  - Positive scenarios
  - Negative scenarios
  - Boundary conditions

---

## Notes

- Test conditions are derived only from the test basis