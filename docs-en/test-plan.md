# Test Plan — Mommento

## 1. Objective

The purpose of this test plan is to define the testing approach for **Mommento**, a productivity web application that combines a **Pomodoro Timer** and a **To-Do List**.

This document aims to ensure that the main features of the application work correctly, that core business rules are respected, and that defects are identified, documented, and communicated effectively.

---

## 2. Project Overview

**Mommento** is a web application that allows users to:

- use only the Pomodoro timer
- use only the task list
- use both features together

When a task is active, focus time is tracked for that task. If no task is active, the application records the time as general daily focus time.

The application also includes task statistics, Pomodoro statistics, theme customization, fullscreen mode, and cycle indicators.

---

## 3. Scope

### In Scope

The following features will be tested:

- Pomodoro timer
- Start / Pause button
- Reset timer button
- Manual switch between focus and break
- 5-minute break behavior
- 15-minute long break after 4 Pomodoro cycles
- Visual cycle indicators
- Pomodoro timer alarm notification
- Task creation
- Task editing
- Task deletion
- Task reordering
- Marking a task as active
- Pending and completed task counters
- Daily focus time tracking
- Task statistics
- Pomodoro statistics
- Theme color change
- Fullscreen mode
- Dynamic interface behavior related to active or inactive tasks

### Out of Scope

The following items are not included in this test plan unless explicitly added later:

- mobile device testing
- Windows operating system testing
- automated testing
- API testing
- performance testing
- security testing
- accessibility testing
- cross-browser compatibility beyond the selected browser used during execution

---

## 4. Test Items

The main test items are:

- Pomodoro module
- To-Do List module
- Statistics module
- Theme settings
- Fullscreen functionality
- Dynamic UI behavior

---

## 5. Test Strategy

Testing will be performed manually based on the functional behavior of the application.

The following testing types will be used:

- Smoke Testing
- Functional Testing
- Regression Testing

The following black-box testing techniques may be applied when designing test cases:

- Equivalence Partitioning
- Boundary Value Analysis
- Decision Table Testing
- State Transition Testing
- Pairwise Testing
- Data-Driven Testing

---

## 6. Test Levels

The focus of this portfolio project is on:

- System Testing
- End-to-End functional validation of core user flows

---

## 7. Entry Criteria

Testing can begin when:

- the application is accessible through the official URL
- the main interface loads successfully
- the core features are available for interaction
- there are no blocking issues preventing basic navigation

---

## 8. Exit Criteria

Testing can be considered complete when:

- all planned smoke test cases have been executed
- all planned functional test cases have been executed
- critical and high-severity defects have been reported
- test evidence has been collected
- test results have been documented and reviewed

---

## 9. Test Environment

Testing environment:

- **Operating System:** macOS
- **Browsers:** Safari, Google Chrome
- **Device Type:** Desktop / Laptop
- **Application Type:** Web Application
- **Environment:** Production (publicly available version)
- **URL:** https://www.mommento.com.br

> Note: Testing will be performed only on Mac systems for this portfolio version.

---

## 10. Test Deliverables

The expected deliverables for this project are:

- Test Plan
- Test Cases
- Test Execution Results
- Bug Reports
- Test Evidence (screenshots and/or recordings)

---

## 11. Risks

Potential risks include:

- production changes during the testing period
- limited environment coverage due to testing only on macOS
- absence of automated regression coverage
- possible data inconsistency in statistics after multiple timer cycles
- UI issues related to dynamic task display and layout behavior

---

## 12. Assumptions

This test plan assumes that:

- the website remains available during the test period
- the tested version reflects the current public version of the application
- all tested features are stable enough for manual validation
- no login is required to use the main core features, unless observed otherwise during execution

---

## 13. Roles and Responsibilities

### Tester
- Design test cases
- Execute manual tests
- Record results
- Report defects
- Collect evidence

For this portfolio project, all activities are performed by the same tester.

---

## 14. Approval

This document is part of a personal QA portfolio project and does not require formal stakeholder approval.
