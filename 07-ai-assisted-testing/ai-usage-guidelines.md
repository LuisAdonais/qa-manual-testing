# Ai usage guidelines

---

## Purpose

In this file, I define how I use AI to support my testing process.

I set clear rules to create and use testware in a controlled way.

---

## Ai tools used

I use AI as support in my testing process.

Tools:

- ChatGPT: to generate and review testware
- Cursor: to review and format the content

---

## How I use ai

I use AI following a controlled workflow:

1. I define the test basis (requirements, user stories, acceptance criteria)
2. I use ChatGPT with my system prompt
3. I work in separate chats to avoid mixing context
4. I generate content per file (test conditions, test cases)
5. I validate the result using a validation prompt
6. I review and format the content using Cursor
7. I perform final manual validation before using the testware

I do not use AI output directly without review.

---

## When I use ai

I use AI in these activities:

- Create test conditions from the test basis
- Create test cases based on test conditions
- Improve clarity in test conditions and test cases
- Suggest test scenarios based on the test basis
- Create initial structure for files and documentation

---

## When I do not use ai

I do not use AI in these cases:

- When there is no test basis defined to create testware
- When the requirements are not clear
- When the system logic is not specified
- When there is sensitive information

---

## Rules for using ai

To use AI I follow these rules:

- I always validate the testware against the test basis
- I do not assume the AI result is correct
- I do not use output without review
- I adjust the prompt if the result is not clear
- I do not add information that is not in the test basis

---

## Relation to the testing process

I use AI as support in:

- Test analysis: create test conditions
- Test design: create test cases

I do not use AI directly in test execution without previous validation.

---

## Traceability context

The use of AI respects traceability:

Requirement → test condition → test case → test execution → defect

---

## Limitations

The use of AI has limitations:

- It can create incorrect information
- It can miss important scenarios
- It can create steps that are not executable

That is why I always do manual validation.

---

## Summary

In this file:

- I define how I use AI in testing
- I set clear rules for using AI
- I validate all testware before use
- I keep alignment with the testing process