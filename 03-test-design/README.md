# Test design

---

## Overview

In this phase, I transform the **Test Conditions** into **Test Cases** and **Test Data**.

I define how the system will be validated using structured and traceable test scenarios.

---

## Objective

- I transform Test Conditions into Test Cases
- I define the Test Data needed for execution
- I ensure traceability between Requirement → Test Condition → Test Case
- I keep alignment with ISTQB and STLC

---

## Artifacts

In this phase, I create:

- `test-cases.md`
- `test-data.md`
- `requirement-traceability-matrix.md`

---

## Input (test basis)

I base this phase on:

- Requirements → `../01-test-analysis/requirements-analysis.md`
- Test Conditions → `../01-test-analysis/test-conditions.md`
- Test Plan → `../02-test-planning/test-plan.md`

---

## Relation to STLC

I base this phase on:

- Test analysis
- Test planning

This phase gives input for:

- Test execution

---

## Traceability

I keep the following traceability model:

```text
Requirement → Test Condition → Test Case → Test Data
```

---

## Notes

> [!NOTE]
> I design the Test Cases and Test Data using only the Test Basis and the observable behavior of the system.

> [!IMPORTANT]
> I do not make assumptions beyond the Test Basis.
