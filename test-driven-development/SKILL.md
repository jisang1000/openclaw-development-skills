---
name: test-driven-development
description: Use test-first development when behavior should be proven, not assumed. Use when implementing features, fixing bugs, refactoring risky logic, or adding automation where a failing test or reproducible check should come first.
---

# Test-Driven Development

Use a red-green-refactor loop whenever behavior should be proven, not assumed.

## Core Rule

Do not write the final fix first when a reproducible test can be created.
Start by expressing the expected behavior in a failing test or failing check.

## Workflow

1. Define the expected behavior.
2. Write the smallest failing test/check.
3. Confirm it fails for the right reason.
4. Implement the smallest change that makes it pass.
5. Re-run the test/check.
6. Refactor only if the behavior stays green.

## What Counts as a Test

Depending on context, a "test" may be:
- a unit test
- an integration test
- a failing CLI smoke check
- a reproducible browser/script check
- a minimal regression script

## When to Use

Use for:
- bug fixes with reproducible symptoms
- logic-heavy code changes
- regressions likely to return
- scripts where output can be checked automatically
- code that affects user-visible behavior

## When Not to Force It

TDD may be lightweight or partial when:
- the task is pure documentation
- the environment cannot reproduce the target behavior
- the best available check is a smoke test rather than a formal test suite

## Practical Examples

### Example: Bug fix
- Reproduce the failing input
- Write a test that fails
- Fix only enough for the test to pass

### Example: Script repair
- Save a sample failing command
- Make the command fail predictably
- change the script
- rerun the same command until it passes

## Common Traps

- writing broad tests before clarifying the exact behavior
- fixing multiple things before confirming the failure
- skipping the initial failing check
- declaring success without rerunning the test
