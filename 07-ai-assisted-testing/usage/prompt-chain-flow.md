# Prompt chain flow

---

## Purpose

This document describes how prompt chaining is used to generate and validate testware with AI support.

AI acts as a support, not a replacement for the tester.

The flow ensures all outputs align with the Test Basis and are validated before use.

---

## Relation to STLC

This file is not tied to a single STLC phase.

It supports multiple phases by assisting in generating, validating, and formatting testware.

---

## AI tools used

- ChatGPT – generate and review testware  
- Cursor – review and format content  

---

## Prompt flow

System prompt  
↓  
Context prompt  
↓  
Task prompt  
↓  
Evaluation prompt  
↓  
Format prompt  

---

## How it is used

1. Define the Test Basis:
   - Requirements  
   - User stories  
   - Acceptance criteria  

2. Use ChatGPT with the system prompt  

3. Work in separate chats to avoid context mixing  

4. Generate testware:
   - Test conditions  
   - Test cases  
   - Expected results  

5. Validate outputs:
   - Use the evaluation prompt  
   - Validate against the Test Basis  

6. Adjust prompts as needed  

7. Review and format content with Cursor  

8. Perform final manual validation:
   - Verify traceability  
   - Check consistency  
   - Ensure no assumptions were added  

---

## Use in testing

AI supports different STLC phases, based on the activity.

### Test analysis

- Create test conditions from the Test Basis  
- Identify test scenarios  

### Test planning

- Support creation of the test plan structure  
- Improve clarity of planning documentation  

### Test design

- Create test cases  
- Define expected results  
- Suggest test scenarios  

### Test execution

- AI does not execute tests  
- AI may assist in:
  - Reviewing test steps  
  - Clarifying expected results  

All outputs must be validated before use.

### Defect management

- Support writing defect descriptions  
- Improve clarity and structure  

Defects must be based on actual test execution.

### Test closure

- Support creation of test summary reports  
- Improve clarity of results  

---

## Relation to AI module

The flow is aligned with:

- `ai-usage-guidelines.md`  
- `ai-output-validation.md`  
- `prompts/system-prompt.md`  
- `prompts/evaluation-prompt.md`  
- `prompts/format-prompt.md`  

---

## Traceability

Requirement → Test condition → Test case → Test execution → Defect

---

## AI risks

- Hallucinations – output not based on the Test Basis  
- Reasoning errors – incorrect logic  
- Bias – incomplete scenarios  

These risks are reduced with validation and manual review.

---

## Benefits

- Reduces hallucinations  
- Improves quality of testware  
- Maintains traceability  
- Enables validation before test execution  

---

> [!NOTE]

> I always use the Test Basis as input.  
> AI output is not used without validation.  
> Prompts are adjusted if results are unclear.  
> A final manual validation is always performed.  
> AI supports, but does not replace, the tester.