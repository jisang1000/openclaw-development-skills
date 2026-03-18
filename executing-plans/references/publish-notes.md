# Publish Notes

## Suggested publish summary

Controlled step-by-step execution of an existing plan with progress and blocker tracking.

## Suggested changelog

Initial OpenClaw-adapted release.

## Example publish command

```bash
clawhub publish ./skills/executing-plans \
  --slug executing-plans \
  --name "Executing Plans" \
  --version 0.1.0 \
  --changelog "Initial OpenClaw-adapted release."
```

## Final review checklist

- description is concise and triggerable
- body is practical, not theoretical only
- examples match real OpenClaw usage
- no unsupported platform-specific assumptions
