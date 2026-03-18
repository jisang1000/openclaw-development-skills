---
name: requesting-code-review
description: Review work against the requested outcome, plan, and likely failure modes before declaring it finished. Use after implementation, setup, automation changes, or any non-trivial modification that needs a quality pass.
---

# Requesting Code Review

Run a quality pass before final delivery.

## Core Rule

Before handing off work, check both:
- spec compliance
- code/config/workflow quality

## Review Pass

### 1. Outcome Check
- Did we solve what the user actually asked?
- Is anything only partially complete?
- Was the correct target edited or configured?

### 2. Plan Check
- Did execution follow the intended plan?
- If the plan changed, was that surfaced clearly?

### 3. Failure Modes
Look for:
- missing dependencies
- wrong paths
- auth/credential gaps
- brittle selectors or assumptions
- docs that no longer match runtime reality
- site-specific blocks mistaken for tool failure

### 4. Verification Quality
- Was behavior tested?
- Was only syntax tested?
- What remains unverified?

## Output Format

Use this structure:
- What looks good
- Risks / gaps
- What should be fixed before calling it done

## Good Example
- "설치는 됐지만 문서가 예전 경로를 가리켜서 실사용 시 혼란이 생김. 문서 수정 후 dry-run 재검증 필요."

## Review Standard

If a critical issue remains, do not present the work as fully complete.
Instead say what is done, what is blocked, and what the next fix should be.

## Practical Examples

### Example: Path mismatch
- Good review catch: docs point to an old path even though the script itself works

### Example: Partial setup
- Good review catch: CLI installed but account/login not configured

### Example: Browser task
- Good review catch: automation tool is healthy, but target site is blocking bots; do not call the whole setup broken
