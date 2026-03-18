---
name: finishing-a-development-branch
description: Finish development work cleanly after implementation by verifying results, checking branch state, and deciding whether to merge, open a PR, keep for later, or discard. Use when a branch or isolated task looks complete and needs a disciplined wrap-up.
---

# Finishing a Development Branch

Finish work deliberately instead of abandoning a branch in an ambiguous state.

## Core Rule

Completion is not just "code exists". A branch is only ready to finish when its outcome, verification, and next disposition are clear.

## End-of-Branch Checklist

1. Re-state the intended outcome.
2. Verify the final behavior.
3. Review for missing files, dependency drift, and doc drift.
4. Check git status and changed files.
5. Decide one of four outcomes:
   - merge now
   - open PR
   - keep for later
   - discard

## What to Verify Before Finish

- tests or smoke checks relevant to the task
- no critical blocker remains hidden
- no accidental unrelated files are included
- the branch description still matches what was actually done

## Practical Examples

### Example: setup branch
- confirm the tool really works
- confirm docs/config match the working state
- then decide whether to merge or keep pending credentials

### Example: bug-fix branch
- reproduce the old failure
- confirm the failure is gone
- check no unrelated side effects were introduced

## Reporting Style

Summarize with:
- what the branch achieved
- how it was verified
- what remains risky or incomplete
- recommended disposition (merge / PR / keep / discard)

## Common Traps

- calling a branch done without verifying behavior
- forgetting to inspect accidental file changes
- keeping a branch around with no clear next step
- merging work that is only partially verified
