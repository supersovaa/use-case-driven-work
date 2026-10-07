# Use-Case-Driven Work

A lightweight pair of skills for planning and reviewing implementation work around concrete user-facing use cases.

## Core idea

Concrete user-facing use cases are the shared unit for relating implementation progress to planned responsibilities and behavioral test coverage.
Planning grows only the structure needed for the use cases being considered, while review verifies behavior when the required use cases become established.

## Skills

`use-case-driven-planning` owns incremental cross-use-case decomposition, direct dependency planning, plan revision, projected progress, and milestone priority.

`use-case-driven-review` owns use-case-level selection and timing of behavioral test-evidence review for newly established, affected, and combined use cases.

## Repository dependency

This repository depends on [`requirement-driven-testing`](https://github.com/supersovaa/requirement-driven-testing) for executable test-evidence responsibilities.

Within use-case-driven review, the selected behavior scopes the settled required test definitions to review. Missing required test definitions return to `test-evidence-planning`, while `test-evidence-review` owns the criteria for judging whether those settled definitions have sufficient executable evidence.
Test-evidence preservation and remediation remain with the corresponding skills in that dependency rather than being redefined here.

## Adjacent responsibilities

Detailed implementation-plan structure belongs to the planning workflow that defines that structure.
Implementation execution, general code review, delegation, and repository operations belong to their respective skills.

Executable behavior and detailed operational rules remain in each skill's `SKILL.md`.
