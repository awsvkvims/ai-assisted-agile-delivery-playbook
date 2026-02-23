# Developer Guide
AI Assisted Quality Driven Engineering

This guide helps developers use AI to strengthen built in quality, reduce cognitive load, and accelerate validated learning without compromising engineering rigor.

AI is a collaborator.
It is not the author of record.
You own the code.

---

## Core Principle

Write tests to clarify intent.
Write code to satisfy behavior.
Use AI to sharpen both.

If AI increases output but decreases understanding, stop.

---

## Where AI Helps The Most

AI assistance is most valuable at:

- Understanding unclear requirements
- Generating edge case scenarios
- Designing test cases
- Exploring alternative implementations
- Refactoring suggestions
- CI failure diagnosis
- Log pattern summarization

AI should reduce time to insight.

---

## 1. Before Writing Code

Before implementation:

- Clarify acceptance criteria.
- Identify edge cases.
- Identify failure conditions.
- Identify performance concerns.

AI Prompt Pattern:

"Given this user story and acceptance criteria, identify edge cases and potential failure modes."

Use AI to:
- Surface hidden assumptions
- Suggest boundary cases
- Identify missing error handling paths

Do not use AI to guess domain behavior.

---

## 2. Test First Thinking

In QDD, tests clarify behavior before implementation.

AI Prompt Pattern:

"Generate candidate test scenarios for this behavior, including negative and boundary cases."

Use AI to:
- Suggest additional scenarios
- Highlight incomplete test coverage
- Propose structured test names

Always review generated tests for correctness.

AI can propose.
You verify.

---

## 3. Code Scaffolding

AI can accelerate initial structure:

- Boilerplate
- Data mapping
- Simple adapters
- Repetitive patterns

AI Prompt Pattern:

"Provide a minimal implementation for this interface that satisfies these constraints."

Avoid:
- Blind copy paste
- Accepting insecure defaults
- Skipping understanding of generated logic

If you cannot explain the code, do not commit it.

---

## 4. Refactoring Support

AI can help detect:

- Duplication
- Long methods
- Naming inconsistencies
- Structural simplifications

AI Prompt Pattern:

"Suggest refactoring improvements for readability and maintainability while preserving behavior."

Verify that:
- No behavior changes unintentionally
- Tests still pass
- Complexity actually decreases

---

## 5. CI Signal Interpretation

When CI fails:

- Test failures
- Lint errors
- Security scans
- Static analysis warnings

AI Prompt Pattern:

"Here is the CI failure output. Summarize likely root causes and propose debugging steps."

AI can:
- Summarize large logs
- Suggest likely causes
- Recommend next investigation steps

You still perform the diagnosis.

---

## 6. Performance And Observability

Before release:

- Validate logging clarity.
- Validate metrics coverage.
- Validate error messages.

AI Prompt Pattern:

"Review this logging and metric design. Identify blind spots and unclear messages."

AI can:
- Suggest structured logging improvements
- Highlight missing telemetry
- Recommend clearer error descriptions

---

## 7. During Retrospective

AI can help analyze:

- Recurring defect patterns
- PR cycle time
- Review bottlenecks
- Failure clustering

AI Prompt Pattern:

"Given these defect summaries and cycle time data, identify patterns and potential systemic causes."

AI helps pattern recognition.
The team decides systemic changes.

---

## Anti Patterns

Do not:

- Replace reasoning with prompt iteration.
- Accept AI generated code without review.
- Skip writing tests because AI wrote code.
- Ignore security implications.
- Increase abstraction without necessity.

If cognitive load increases, reassess usage.

---

## Signals Of Effective AI Usage

- Tests become more comprehensive.
- PR cycle time decreases.
- Fewer rework cycles occur.
- CI failures are resolved faster.
- Code readability improves.
- Defect escape rate decreases.

AI should improve feedback quality and speed.
It should not increase noise.

