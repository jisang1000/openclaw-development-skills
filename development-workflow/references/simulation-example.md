# Development Workflow Simulation Example

## Scenario

Task: "A browser automation skill is installed, but a shopping site blocks search results. Make it usable if possible."

## Step-by-step skill usage

### 1. writing-plans
Create a short plan:
1. Confirm whether the browser tool itself works
2. Reproduce the failing target flow
3. Separate tool failure vs site blocking
4. Try a safe alternate approach
5. Verify the final behavior

### 2. systematic-debugging
Split the problem:
- Does the browser open normal sites?
- Does only the target site fail?
- Is the failure auth-related, anti-bot, or selector-related?
- Does headless fail while headed mode works?

### 3. test-driven-development
If reproducible, define a minimal failing check:
- open target page
- confirm expected title or element is missing
- use that as the failing check before changing the setup

### 4. executing-plans
Execute in order:
- test a known-good page
- test target page
- try alternate mode (headed / session reuse / different engine)
- rerun the same checks after each change

### 5. verification-before-completion
Do not say "fixed" just because the browser launched.
Only say complete if the target behavior is confirmed:
- target page loads
- expected text/element exists
- user-facing task actually works

### 6. requesting-code-review
Before final delivery, ask:
- Did we fix the actual target problem?
- Are docs and runtime paths consistent?
- Is this a tool issue or a target-site blocking issue?
- What remains unverified?

### 7. dispatching-parallel-agents (optional)
If the task is large:
- Agent A: inspect skill/runtime setup
- Agent B: test alternate browser path
- Agent C: summarize blockers and compare outcomes

### 8. using-git-worktrees / finishing-a-development-branch (optional)
If code changes are significant:
- isolate risky fixes in a worktree
- verify outcomes
- then decide merge / keep / discard

## Final report style

- What was broken
- Confirmed cause
- What changed
- How it was verified
- What still remains blocked
