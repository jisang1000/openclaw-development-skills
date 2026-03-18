# OpenClaw Development Skills

A practical set of OpenClaw-adapted development skills for planning, debugging, verification, review, execution, and branch hygiene.

These skills are designed to improve how an agent works rather than replace OpenClaw's built-in tools. The goal is simple: better plans, cleaner debugging, stronger verification, safer execution, and clearer final reporting.

## What This Repository Is For

This repository packages a focused development stack for OpenClaw agents.

Use it when you want an agent to:
- plan before coding
- debug by root cause instead of guessing
- verify real outcomes before saying work is done
- review likely failure modes before handoff
- execute multi-step implementation work more consistently

These skills are intentionally lightweight, behavior-oriented, and OpenClaw-friendly.
They focus on decision quality and execution discipline, not platform-specific magic.

## Core Skills

- `verification-before-completion` — Verify real outcomes before saying work is done
- `systematic-debugging` — Debug through a structured root-cause process
- `writing-plans` — Break long work into explicit, ordered steps
- `requesting-code-review` — Review outcome, plan, and likely failure modes before handoff
- `test-driven-development` — Use test-first thinking when behavior should be proven
- `development-workflow` — Combine planning, execution, debugging, verification, and review into one practical flow

## Supporting Skills

- `using-git-worktrees` — Isolate risky or parallel work safely
- `finishing-a-development-branch` — Close branch work cleanly with verification and disposition
- `dispatching-parallel-agents` — Use parallel sub-agents for independent subtasks
- `executing-plans` — Execute an existing plan step by step without losing track of progress

## Quick Start

1. Start with `verification-before-completion`.
2. Add `systematic-debugging` and `writing-plans` next.
3. Use `development-workflow` when you want one integrated flow.
4. Add supporting skills only when the project actually needs them.

### Minimal starter stack

- `verification-before-completion`
- `systematic-debugging`
- `writing-plans`
- `development-workflow`

## Recommended Adoption Order

1. `verification-before-completion`
2. `systematic-debugging`
3. `writing-plans`
4. `requesting-code-review`
5. `test-driven-development`
6. `development-workflow`
7. Supporting workflow skills

## Example Usage Flow

### Example: fix a broken automation

1. Use `writing-plans` to break the repair into explicit steps.
2. Use `systematic-debugging` to identify the real failure point.
3. Implement the fix.
4. Use `verification-before-completion` to prove the failure is actually resolved.
5. Use `requesting-code-review` if the change is risky or likely to regress.

### Example: implement a small feature safely

1. Use `development-workflow` as the main frame.
2. Pull in `test-driven-development` if the behavior should be proven.
3. Use `finishing-a-development-branch` when closing out the work.

## Repository Layout

- `development-workflow/`
- `dispatching-parallel-agents/`
- `executing-plans/`
- `finishing-a-development-branch/`
- `requesting-code-review/`
- `systematic-debugging/`
- `test-driven-development/`
- `using-git-worktrees/`
- `verification-before-completion/`
- `writing-plans/`

Each skill directory contains a `SKILL.md` and, where useful, a `references/` folder with supporting notes and examples.

## Best For

- tool and runtime setup
- automation repair
- browser/script debugging
- structured implementation work
- safer multi-step development tasks
- more reliable completion reporting

## First Publish Recommendation

Publish `verification-before-completion` first.
It has the clearest value proposition, is broadly useful, and represents the set well.
