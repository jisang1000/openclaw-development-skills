---
name: executing-plans
description: Execute a written plan in a controlled way after scope, order, and verification points are clear. Use when a task already has a plan and now needs disciplined step-by-step execution without losing track of progress or blockers.
---

# Executing Plans

Once a plan is good enough, execute it deliberately instead of improvising each step.

## Core Rule

Do not keep re-planning forever. When the plan is clear enough, start executing and update only when reality changes.

## Workflow

1. Restate the goal and current plan.
2. Start with the first high-confidence step.
3. After each step, record one of:
   - complete
   - blocked
   - changed assumption
4. If blocked, decide:
   - debug now
   - narrow scope
   - parallelize an independent subtask
5. Keep verification attached to the relevant step.
6. Finish with a final verification and review pass.

## Progress Tracking

Track execution in simple language:
- done
- in progress
- blocked
- skipped with reason

## Good Execution Behavior

- preserve the original goal
- expose changed assumptions quickly
- avoid jumping ahead without finishing verification
- keep the user updated when the task is long-running

## Practical Examples

### Example: tool setup
1. inspect installation
2. install missing dependency
3. run smoke test
4. handle auth/config if needed
5. verify final command works

### Example: migration
1. inspect current state
2. update files in safe order
3. run checks after each stage
4. review diffs and final state

## Common Traps

- losing track of which step failed
- changing the plan silently
- declaring completion with unfinished verification
- mixing execution with unrelated new tasks
