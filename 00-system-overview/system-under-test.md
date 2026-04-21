# System under test (SUT)

---

## System overview

- **System name:** Demo Web Shop (Tricentis)
- **Application type:** Web application
- **Access type:** Public (some features require login)

### Description

Demo Web Shop is a web application for e-commerce testing practice.  
Users can browse products and simulate the purchase process.

### Business purpose

The system aims to:

- Allow users to browse products
- Allow users to register and log in
- Simulate a basic purchase flow

---

## Main functionalities

- User registration
- Login and logout
- Product browsing
- Shopping cart
- Checkout

---

## Users and roles

- **Guest user**
  - Can browse products

- **Registered user**
  - Can log in
  - Can add products to cart
  - Can perform checkout

---

## Test environment

- **URL:** https://demowebshop.tricentis.com/
- **Browser:** Firefox
- **Device:** Desktop

---

## Assumptions

- Payment is simulated

---

## Risks

- Issues in checkout flow may affect the purchase process
- Login or registration failures may block user actions

---

## Test basis

Testing is based on:

- Requirements
- User stories
- Acceptance criteria

---

## Relation to testing

This document defines the **system under test (test object)** and provides context for:

- Test analysis
- Test design
- Test planning

It is used together with the test basis to create:

- Test conditions
- Test cases

---

## Scope note

This document provides a general understanding of the system.  
Testing scope and approach are defined in the test plan.

---

## Traceability

```text
Requirement → Test condition → Test case
```
