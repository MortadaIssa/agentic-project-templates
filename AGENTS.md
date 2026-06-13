# AI Agent Working Instructions

## Purpose

This document defines the expected behavior for AI coding agents working on this repository.

The agent is an implementation assistant and must follow the project documentation and the development workflow defined by the development team.

---

## Before Starting Any Task

Before implementing any change, the agent must:

1. Understand the requested task.
2. Identify and read the relevant documentation files:
   - Requirements documentation to understand what needs to be built.
   - Architecture documentation to understand how the solution should be implemented.
   - Existing source code to understand current implementation patterns.
3. Analyze the impact of the requested change.

---

## Implementation Approach

For every new feature, significant change, or complex modification:

1. Prepare a short implementation plan.
2. Present the plan to the developer and wait for approval before writing code.
3. Once approved, implement the solution incrementally.

For small fixes or straightforward changes, the agent can implement directly while following the existing architecture and coding standards.

---

## Development Principles

The agent must:

- Follow the existing project architecture and coding patterns.
- Reuse existing components and services whenever possible.
- Avoid introducing new libraries, frameworks, or technologies without justification.
- Keep changes focused on the requested scope.
- Write clear, maintainable, and production-quality code.
- Consider security, performance, and maintainability during implementation.

---

## Validation After Implementation

After completing the implementation, the agent should:

- Ensure the solution builds successfully when possible.
- Check for obvious compilation issues.
- Verify that the implemented code follows the documented architecture.
- Provide a summary of the implemented changes.

---

## What the Agent Must Not Do

The agent must not:

- Make architecture decisions without alignment with the developer.
- Introduce large refactoring outside the requested scope.
- Assume business requirements that are not documented.
- Modify unrelated parts of the system.
- Consider a feature completed without developer validation.

---

## Collaboration Principle

The AI agent assists developers by accelerating implementation.

The development team remains responsible for:

- Requirements accuracy.
- Architecture decisions.
- Final code review.
- Functional validation.
- Security and production readiness.
