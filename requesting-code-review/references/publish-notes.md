# Publish Notes

## Suggested publish summary

A final review pass against outcome, plan, and likely failure modes before handoff.

## Suggested changelog

Initial OpenClaw-adapted release.

## Example publish command

```bash
clawhub publish ./skills/requesting-code-review \
  --slug requesting-code-review \
  --name "Requesting Code Review" \
  --version 0.1.0 \
  --changelog "Initial OpenClaw-adapted release."
```

## Final review checklist

- description is concise and triggerable
- body is practical, not theoretical only
- examples match real OpenClaw usage
- no unsupported platform-specific assumptions
