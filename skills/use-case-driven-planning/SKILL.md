---
name: use-case-driven-planning
description: Plan concrete user-facing use cases by decomposing behavior into independently verifiable partial results and using shared diagonal progress planning for one or more use cases.
---

# Use-Case-Driven Planning

Use this skill when creating or revising implementation plans for concrete user-facing use cases.

Use a concrete user-facing use case as the completion target for relating implementation progress to observable behavior.
Use ordinary `plan-driven-planning` for settled design provenance, implementation-plan structure, dependencies, authoritative state, and concurrency constraints.
Apply `diagonal-progress-planning` to arrange and revise useful staged progress, whether one or several use cases are being planned. Its cross-use-case coordination applies when multiple use cases are relevant.

## Plan the use-case boundary

Begin with settled requirements, established implementation results, and the current repository planning state.
For each requested use case, identify the behavior that establishes its completion and the responsibilities or capabilities needed to deliver it.

Decompose the use case into plans that each establish a meaningful partial result.
Split a planned result when it contains independently establishable and verifiable outcomes; keep outcomes together when their implementation or meaningful validation is inseparable.
Define only the directly required prerequisites within the currently considered use case using ordinary dependency semantics.
Keep future work unplanned where available information does not yet justify a concrete plan boundary.

Relate each use case to relevant already-established or planned results.
When a required responsibility is already established on the relevant base branch, reference the current requirements/design canon and verified repository behavior. Keep the producing plan as historical context when useful.
When implementation of a prerequisite result is still pending, reference its authoritative producing plan as the one pending owner and record a direct dependency using ordinary planning rules. When a completed producing plan's result awaits integration into the relevant base branch, track that integration requirement using ordinary planning rules.
A current plan may appear under multiple use-case views while retaining one authoritative plan state.
Use `diagonal-progress-planning` to resolve newly discovered shared-result relationships and cross-use-case prerequisites.

## Preserve useful behavioral progress

Express each partial result in terms of what becomes establishable and verifiable for the use case.
Assign its completion obligations to the plan that can first establish them; keep behavior requiring further use cases with the later responsible plan.
Use `diagonal-progress-planning` to project the useful partial results of a single use case or interleave eligible results across multiple use cases. It owns priority comparisons among viable alternatives.
When a changed result affects the staged progression within a use case or across several use cases, use that skill to revise the affected projection and ordinary plan-driven rules for authoritative plan changes.

## Hand off verification

Keep the required observable behavior and the plan that establishes it identifiable so `use-case-driven-review` can select the affected behavior for test-evidence review.
Required test definitions and sufficient executable evidence belong to the respective test-evidence skills.
Implementation execution and code review follow their usual workflows; diagonal progress does not require synchronized waves.

This skill owns use-case completion targets, use-case-local decomposition, and behavioral progress attribution.
`diagonal-progress-planning` owns staged progress within or across use cases, cross-use-case dependencies when needed, incremental projection, and affected-progress revision.
