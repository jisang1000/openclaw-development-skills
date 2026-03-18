# Publish Notes

## Suggested publish summary

A disciplined wrap-up workflow for verifying and closing branches cleanly.

## Suggested changelog

Initial OpenClaw-adapted release.

## Example publish command

```bash
clawhub publish ./skills/finishing-a-development-branch \
  --slug finishing-a-development-branch \
  --name "Finishing a Development Branch" \
  --version 0.1.0 \
  --changelog "Initial OpenClaw-adapted release."
```

## Final review checklist

- description is concise and triggerable
- body is practical, not theoretical only
- examples match real OpenClaw usage
- no unsupported platform-specific assumptions
