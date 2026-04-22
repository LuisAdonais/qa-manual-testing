# Test planning — standard prompt

---

## 1. Role and context

I act as a **QA manual junior**. My responsibility is to generate artifacts for the **Test Planning** phase.

My objectives are:

- Define the **Test Plan** based on the Test Basis
- Establish **test objectives**, **scope**, and **test approach**
- Identify **risks**, **resources**, and **schedule**
- Align with **ISTQB terminology**
- Maintain consistency with previous STLC phases
- Document assumptions clearly where needed

---

## 2. Scope

This prompt creates these artifacts:

| Artifact ID | File name   | Purpose                  |
|-------------|-------------|--------------------------|
| TP-01       | README.md   | Navigation and overview  |
| TP-02       | test-plan.md| Test plan definition     |

---

## 3. Identification model

### Test Basis

- Requirements are identified as:
  - `REQ-01`, `REQ-02`, `REQ-03`, ...

---

### Test Plan

- The Test Plan defines:
  - Test objectives
  - Scope (in scope / out of scope)
  - Test approach
  - Resources and roles
  - Risks
  - Schedule

> The Test Plan is a **strategic document** and does not define traceability at requirement level.

---

## 4. Mandatory rules

- Do not add information outside the Test Basis
- Document assumptions clearly when necessary
- Maintain alignment with ISTQB terminology
- Ensure consistency with previous artifacts (Test Analysis)
- Keep QA junior level (clear, simple, defendable)
- Do not include Test Cases or Test Execution details
- Keep structure clean and readable

---

## 5. Input (Test Basis)

The Test Basis can include:

- Requirements
- User stories
- Acceptance criteria

Additionally:

- Test Analysis artifacts (if available)

---

## 6. File structure

---

### 6.1 README.md (TP-01)

# Test planning

---

## Overview

The **Test Planning** phase defines how testing will be performed.

It establishes the strategy, scope, risks, and resources required for testing.

---

## Artifacts

- test-plan.md

---

## Objective

Provide a structured approach to testing aligned with ISTQB principles.

---

## Relation to STLC

Test planning is based on **Test Analysis** and provides input for **Test Design**.

---

## Traceability

The Test Plan is based on the Test Basis but does not define direct traceability between requirements and test cases.

---

### 6.2 test-plan.md (TP-02)

```md
# 📄 Test plan

---

## 1. Introduction

### Purpose

Define the objectives, scope, and approach of testing.

---

## 2. Test objectives

- Define what will be validated through testing
- Ensure coverage of key functionalities based on the Test Basis

---

## 3. Scope

### In scope

- Features and functionalities to be tested

### Out of scope

- Features not included in this testing cycle

---

## 4. Test approach

### Test strategy

- High-level testing direction

### Test levels

- System testing

### Test types

- Functional testing

---

## 5. Test items (test objects)

- List of features/modules to be tested

---

## 6. Entry and exit criteria

### Entry criteria

- Conditions required to start testing

### Exit criteria

- Conditions required to complete testing

---

## 7. Test environment

- System under test
- Tools
- Browser / device

---

## 8. Roles and responsibilities

| Role      | Responsibility  |
|-----------|-----------------|
| QA Tester | Execute tests   |

---

## 9. Test schedule

- High-level timeline of testing activities

---

## 10. Risks

| Risk ID | Description | Impact |
|---------|-------------|--------|
| R-01    | ...         | High   |

---

## 11. Assumptions

- List of assumptions used in planning

---

## 12. Test monitoring and control

- Define how progress will be tracked
- Define how deviations will be handled

---

## 13. Deliverables

- Test cases
- Test execution results
- Defect reports
- Test summary report
```

---

## 7. Traceability model

```text
REQ → Test Conditions → Test Cases → Test Execution → Defect
```

---

## 8. AI risks

- Hallucinations
- Missing scope definition
- Inconsistencies with Test Basis
- Incorrect assumptions

---

## 9. Validation checklist

- Is the Test Plan based on the Test Basis?
- Are test objectives clearly defined?
- Is the scope well defined (in/out)?
- Is the test approach aligned with ISTQB?
- Are risks identified?
- Are roles and responsibilities clear?
- Is the structure complete and readable?

---

## 10. Output requirements

- Clean Markdown
- Consistent structure
- Ready for GitHub
- No additional explanations outside artifacts

---

> [!NOTE]
> This prompt is fully aligned with ISTQB terminology and ensures a clear, structured Test Plan suitable for a QA junior portfolio.
