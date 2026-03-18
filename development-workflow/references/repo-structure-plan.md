# Repo Structure Plan for OpenClaw Development Skills

## Goal

Package the OpenClaw-adapted development skills as one coherent set while still allowing each skill to be published independently.

## Suggested top-level structure

```text
openclaw-development-skills/
├── README.md
├── verification-before-completion/
│   ├── SKILL.md
│   └── references/
├── systematic-debugging/
│   ├── SKILL.md
│   └── references/
├── writing-plans/
│   └── SKILL.md
├── requesting-code-review/
│   └── SKILL.md
├── test-driven-development/
│   └── SKILL.md
├── development-workflow/
│   ├── SKILL.md
│   └── references/
├── using-git-worktrees/
│   └── SKILL.md
├── finishing-a-development-branch/
│   └── SKILL.md
├── dispatching-parallel-agents/
│   └── SKILL.md
└── executing-plans/
    └── SKILL.md
```

## Grouping logic

### Core quality loop
- verification-before-completion
- systematic-debugging
- writing-plans
- requesting-code-review
- test-driven-development
- development-workflow

### Supporting workflow skills
- using-git-worktrees
- finishing-a-development-branch
- dispatching-parallel-agents
- executing-plans

## Publish strategy

### Option A: publish individually
Best when testing demand and refining descriptions.

### Option B: maintain one GitHub repo, publish skills one by one
Best for version control and reuse.

## Suggested first publish order

1. verification-before-completion
2. systematic-debugging
3. writing-plans
4. requesting-code-review
5. test-driven-development
6. development-workflow
7. the supporting workflow skills after that

## README should explain

- what the set is for
- which skills are core vs supporting
- recommended adoption order
- how the skills compose into one workflow
