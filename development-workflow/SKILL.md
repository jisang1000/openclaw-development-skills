---
name: development-workflow
description: Use a structured development workflow for non-trivial coding, debugging, setup, and automation tasks. Use when work should follow a disciplined sequence—plan, implement, debug, verify, and review—instead of ad-hoc changes.
---

# Development Workflow

This skill combines planning, debugging, verification, review, and test-first thinking into one practical flow.

## Use This Sequence

### 1. Plan first
Load `writing-plans` when the task is multi-step, risky, or long-running.
Ask:
- what is the goal?
- what are the constraints?
- what are the success checks?

### 2. Prefer test-first when possible
Load `test-driven-development` when behavior can be proven with a failing test or reproducible check.

### 3. Debug systematically when blocked
Load `systematic-debugging` when the path is unclear or behavior is inconsistent.
Separate tool failure, config failure, auth failure, target-site blocking, and environment issues.

### 4. Verify before saying done
Load `verification-before-completion` before any completion report.
Check actual outcomes, not just command success.

### 5. Review before handoff
Load `requesting-code-review` for a final quality pass.
Check for missing dependencies, doc drift, hidden blockers, and partial completion.

## Recommended Default Flow

1. Write a short plan
2. Identify the smallest proof of success
3. Implement or debug
4. Verify actual behavior
5. Review and report remaining risk
6. If branch isolation helps, use `using-git-worktrees`
7. When done, close cleanly with `finishing-a-development-branch`

## Example Uses

- installing and fixing a toolchain
- browser automation setup
- script repair
- feature implementation
- bug fixing with regressions
- migration work
- parallel audits or research via `dispatching-parallel-agents`
- stepwise implementation via `executing-plans`

## Reporting Template

Use this summary style:
- Goal
- What changed
- How it was verified
- Risks / blockers
- Recommended next step

## Practical Examples

## 한국어 실전 사용 예시

### 예시 1: 스킬 설치가 안 될 때
1. `writing-plans`로 설치/검사/수정 순서를 짠다.
2. `systematic-debugging`으로 설치 문제인지, 의존성 문제인지, 인증 문제인지 분리한다.
3. `verification-before-completion`으로 실제 명령이 되는지 확인한다.
4. `requesting-code-review`로 문서 경로나 빠진 의존성이 없는지 점검한다.

### 예시 2: 브라우저 자동화가 특정 사이트에서 막힐 때
1. 작은 재현 경로부터 확인한다.
2. 툴 고장인지, 사이트 anti-bot인지 분리한다.
3. 로그인 세션 재사용 같은 우회 가능성을 본다.
4. 성공 여부를 실제 페이지 상태로 검증한다.

### 예시 3: 긴 코딩 작업
1. `writing-plans`로 단계 쪼개기
2. `test-driven-development`로 재현 가능한 실패부터 만들기
3. `executing-plans`로 순차 실행
4. 필요하면 `dispatching-parallel-agents`로 독립 작업 분리
5. 마지막에 `finishing-a-development-branch`로 정리
