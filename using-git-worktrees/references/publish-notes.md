# Publish Notes

## Suggested publish summary

Safe branch isolation for parallel or risky development work.

## Suggested changelog

Initial OpenClaw-adapted release.

## Example publish command

```bash
clawhub publish ./skills/using-git-worktrees \
  --slug using-git-worktrees \
  --name "Using Git Worktrees" \
  --version 0.1.0 \
  --changelog "Initial OpenClaw-adapted release."
```

## Final review checklist

- description is concise and triggerable
- body is practical, not theoretical only
- examples match real OpenClaw usage
- no unsupported platform-specific assumptions
