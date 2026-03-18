# Publish Notes

## Suggested publish summary

Test-first behavior validation for bug fixes, features, and risky code changes.

## Suggested changelog

Initial OpenClaw-adapted release.

## Example publish command

```bash
clawhub publish ./skills/test-driven-development \
  --slug test-driven-development \
  --name "Test-Driven Development" \
  --version 0.1.0 \
  --changelog "Initial OpenClaw-adapted release."
```

## Final review checklist

- description is concise and triggerable
- body is practical, not theoretical only
- examples match real OpenClaw usage
- no unsupported platform-specific assumptions
