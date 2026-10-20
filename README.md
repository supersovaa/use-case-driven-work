# Use-Case-Driven Work

Use concrete user-facing use cases as completion targets for implementation planning and behavior-based review.

## Skills

- [use-case-driven-planning](skills/use-case-driven-planning/SKILL.md) — use when creating or revising implementation plans for user-facing use cases; define each use case's required behavior and independently verifiable partial results.
- [use-case-driven-review](skills/use-case-driven-review/SKILL.md) — use when reviewing implementation progress against established, affected, and combined use-case behavior.

## Planning workflow

Use [plan-driven-planning](https://github.com/supersovaa/plan-driven-implementation/blob/main/skills/plan-driven-planning/SKILL.md) for implementation-plan boundaries, direct-dependency semantics, persistent state, and general concurrency constraints.

Use [diagonal-progress-planning](https://github.com/supersovaa/diagonal-progress-planning/blob/main/SKILL.md) for cross-use-case result dependencies, coarse implementation order, lightweight-first priorities among grounded alternatives, incremental progress projections, and revision of the affected planning scope.
This follows the local-versus-cross planning separation used by [cell-complete-development](https://github.com/supersovaa/cell-complete-development), without requiring the Cell workflow's synchronized waves or Cell-specific test completion rules.
Unrelated use cases may advance while cross-use-case analysis is incomplete elsewhere.

## Verification and other responsibilities

This repository depends on [requirement-driven-testing](https://github.com/supersovaa/requirement-driven-testing).
Use-case review selects applicable settled required test definitions for newly established, affected, and combined use-case behavior.
Missing definitions return to `test-evidence-planning`; `test-evidence-review` judges executable evidence, and the preservation and remediation skills retain their respective responsibilities.

Detailed implementation execution, general code review, delegation, and repository operations remain with their respective skills.

## Installation

Install `skills/use-case-driven-planning/` and `skills/use-case-driven-review/` as separate skills under your agent's skill loader, retaining each directory's `SKILL.md`.
For use-case planning, also install `plan-driven-planning` and `diagonal-progress-planning`.
For behavioral evidence review, make the relevant `requirement-driven-testing` skills available.
