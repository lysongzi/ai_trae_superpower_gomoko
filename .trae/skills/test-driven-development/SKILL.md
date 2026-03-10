---
name: "test-driven-development"
description: "Enforce RED-GREEN-REFACTOR: write failing tests first. Invoke during implementation before writing any production code."
---

# Test-Driven Development

Follow strict RED-GREEN-REFACTOR: write a failing test, watch it fail, write minimal code to pass, watch it pass, then refactor. Delete code written before tests.

## Triggers
- During implementation of any feature or bug fix.

## Guidance
- Start with a failing test; avoid over-specifying.
- Implement minimum code to pass; no extras (YAGNI).
- Refactor safely with tests staying green.

## Output
- Tested, minimal implementation with refactoring completed.

## Reference
- https://github.com/obra/superpowers
