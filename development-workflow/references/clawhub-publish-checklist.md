# ClawHub Publish Checklist

Use this checklist before publishing these OpenClaw-adapted development skills.

## Scope

Skills currently prepared:
- verification-before-completion
- systematic-debugging
- writing-plans
- requesting-code-review
- test-driven-development
- development-workflow
- using-git-worktrees
- finishing-a-development-branch
- dispatching-parallel-agents
- executing-plans

## Pre-publish checks

### 1. Metadata quality
- name is clear and stable
- description explains both what the skill does and when to use it
- no platform-specific claims that are not true in OpenClaw

### 2. Body quality
- imperative instructions
- no duplicated sections
- examples are realistic
- references are linked only when needed

### 3. OpenClaw fit
- no Claude-only slash-command assumptions
- no unsupported plugin workflow language
- references to OpenClaw concepts are accurate

### 4. Safety
- no destructive default behavior
- no hidden external actions
- no credential assumptions in generic skills

### 5. Packaging shape
Each skill folder should be self-contained:
- SKILL.md required
- optional references/ only if useful
- avoid unnecessary extra docs

## Suggested publish order

1. verification-before-completion
2. systematic-debugging
3. writing-plans
4. requesting-code-review
5. test-driven-development
6. development-workflow

Publish supporting skills next:
7. using-git-worktrees
8. finishing-a-development-branch
9. dispatching-parallel-agents
10. executing-plans

## Suggested changelog theme

"Adapted proven development workflow skills for OpenClaw. Focus on planning, debugging, verification, review, controlled execution, and branch hygiene."

## Final manual review

Before publish, read each SKILL.md once from top to bottom and ask:
- Would another OpenClaw agent know when to trigger this?
- Is this concise enough?
- Does this help behavior, not just describe theory?
