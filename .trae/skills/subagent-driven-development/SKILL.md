---
name: "subagent-driven-development"
description: "Dispatch tasks to fresh subagents with two-stage review. Invoke when executing plan tasks for autonomous progress."
---

# Subagent-Driven Development

Execute plan tasks with fresh subagents. Each task undergoes two-stage review: spec compliance first, then code quality. Continue iteratively until done.

## Triggers
- Implementation phase with a prepared task list.

## Guidance
- Launch a new subagent per task; avoid shared state.
- Review for plan adherence, then quality and tests.
- Proceed to next task or fix issues before moving on.

## Output
- Completed tasks with verified reviews.

## Reference
- https://github.com/obra/superpowers
