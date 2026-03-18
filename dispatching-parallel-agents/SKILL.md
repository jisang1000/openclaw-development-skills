---
name: dispatching-parallel-agents
description: Use parallel sub-agents when a task can be safely split into independent tracks. Use when research, comparison, auditing, or implementation subtasks can run concurrently without conflicting edits or shared mutable state.
---

# Dispatching Parallel Agents

Use parallel agents to increase speed without creating coordination chaos.

## Core Rule

Only parallelize work that is meaningfully separable.
Do not split tightly coupled work just to look fast.

## Good Fit

Use for:
- comparing multiple options
- auditing many independent items
- researching several sources in parallel
- splitting implementation into isolated files or domains
- one agent gathering facts while another validates or reviews

## Bad Fit

Avoid parallelization when:
- tasks edit the same files heavily
- steps depend on each other's intermediate output
- the overhead of coordination is higher than the work itself
- the task is small enough to finish directly

## Workflow

1. Define the main goal.
2. Split into independent subtasks.
3. Make each subtask explicit and self-contained.
4. Spawn parallel agents only for those subtasks.
5. Wait for all results.
6. Reconcile conflicts and synthesize one final answer.

## Task Design Rule

Each sub-agent task should include:
- exact scope
- what not to touch
- expected output format
- what counts as success

## Practical Examples

### Example: skill audit
- Agent A: inspect installed skills
- Agent B: test runtime dependencies
- Agent C: summarize broken vs working

### Example: comparison task
- Agent A: option 1 research
- Agent B: option 2 research
- Agent C: price/feature comparison

## Common Traps

- parallelizing tasks that need the same files
- vague sub-agent instructions
- forgetting to synthesize results
- reporting before all child results arrive
