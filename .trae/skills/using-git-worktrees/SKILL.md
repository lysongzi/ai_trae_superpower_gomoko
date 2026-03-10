---
name: "using-git-worktrees"
description: "Create isolated worktree on new branch; baseline tests clean. Invoke after plan approval to start implementation safely."
---

# Using Git Worktrees

Create an isolated workspace on a fresh branch, run project setup, and verify a clean test baseline before any changes to ensure safe, parallel development.

## Triggers
- Plan approved and ready to implement.

## Guidance
- Create new branch with git worktree.
- Install dependencies and run tests; ensure all green.
- Keep main workspace clean and switch via worktrees.

## Output
- Isolated branch workspace with verified baseline.

## Reference
- https://github.com/obra/superpowers
