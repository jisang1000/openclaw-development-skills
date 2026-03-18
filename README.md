# OpenClaw Development Skills

A practical set of OpenClaw-adapted development skills for planning, debugging, verification, review, execution, and branch hygiene.

These skills are designed to improve how an agent works rather than replace OpenClaw's built-in tools. The goal is simple: better plans, cleaner debugging, stronger verification, safer execution, and clearer final reporting.

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

## Recommended Adoption Order

1. `verification-before-completion`
2. `systematic-debugging`
3. `writing-plans`
4. `requesting-code-review`
5. `test-driven-development`
6. `development-workflow`
7. Supporting workflow skills

## Best For

- tool and runtime setup
- automation repair
- browser/script debugging
- structured implementation work
- safer multi-step development tasks
- more reliable completion reporting

## Design Principle

These skills are intentionally lightweight, behavior-oriented, and OpenClaw-friendly.
They focus on decision quality and execution discipline, not platform-specific magic.

## First Publish Recommendation

Publish `verification-before-completion` first.
It has the clearest value proposition, is broadly useful, and represents the set well.
