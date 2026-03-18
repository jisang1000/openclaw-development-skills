---
name: using-git-worktrees
description: Use git worktrees to isolate parallel development tasks safely. Use when multiple branches need to be worked on side by side, when risky changes should be isolated from the main workspace, or when separate implementation/debugging tracks should not interfere with each other.
---

# Using Git Worktrees

Use git worktrees when one working directory is not enough.

## Core Rule

Do not pile unrelated or risky changes into the same working tree when isolation would reduce mistakes.

## When to Use

Use for:
- parallel feature work
- risky refactors
- comparing two implementation approaches
- debugging while keeping the main branch clean
- sub-agent or separate-task execution that should not touch the same files in one tree

## Workflow

1. Confirm the current branch is in a good state.
2. Choose a clear branch name for the new work.
3. Create a separate worktree for that branch.
4. Run any project setup needed in the new worktree.
5. Do the isolated work there.
6. Verify changes before merging or discarding.

## Good Practices

- keep each worktree purpose-specific
- use explicit branch names
- avoid mixing unrelated tasks in the same worktree
- clean up unused worktrees after the work is resolved

## Practical Examples

### Example: risky experiment
- Keep main workspace stable
- Create a worktree for the experiment branch
- Test there without polluting the main branch

### Example: parallel debugging
- One worktree for current implementation
- One worktree for root-cause debugging or alternative fix

## Common Traps

- creating a second branch but still editing the original worktree
- forgetting setup/dependencies in the new worktree
- leaving stale worktrees around after the task is complete
