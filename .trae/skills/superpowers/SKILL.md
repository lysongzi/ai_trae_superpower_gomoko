---
name: "superpowers"
description: "Agentic workflow with planning, TDD, code review, and branch finishing. Invoke when starting features, debugging, or organizing development."
---

# Superpowers

Superpowers provides an opinionated engineering workflow that coordinates brainstorming/design, planning, isolated worktrees, subagent execution, strict TDD, and code review before merging.

## Triggers
- Start of a feature, refactor, or bug fix.
- Need a formal plan or design validation.
- Require strict TDD enforcement before any code is written.
- Want automated code review and branch finishing workflow.

## Workflow Stages
- Brainstorming: refine problem, explore alternatives, capture design spec.
- Writing Plans: break work into atomic tasks with file paths and verification.
- Using Git Worktrees: create isolated branch workspace, ensure clean test baseline.
- Subagent-Driven Development: dispatch tasks with two-stage review.
- Test-Driven Development: RED-GREEN-REFACTOR; delete code written before tests.
- Requesting Code Review: pre-merge checks, severity-based issues.
- Finishing a Development Branch: verify tests; merge/PR/cleanup guidance.

## Usage
- Invoke this skill when you want structured engineering flow with automatic stage handoffs.
- Combine with specific sub-skills (brainstorming, writing-plans, test-driven-development, etc.) for stage-specific guidance.

## References
- https://github.com/obra/superpowers
