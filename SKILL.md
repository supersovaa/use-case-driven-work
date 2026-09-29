---
name: use-case-driven-work
description: Plan implementation by concrete use cases, splitting each use case into staged work, staggering progress across viable use cases, mapping dependencies across the requested scope, comparing remaining plan-level work against established and projected results, and favoring lighter milestones when evidence supports a difference.
---

# Use-Case-Driven Work

Use this skill when creating or revising an implementation plan.

Use concrete user-facing use cases as the primary units for relating user-visible progress to implementation work.

## Map the requested scope

Map the full requested implementation scope before choosing initial work.

For each use case, identify the plan-level responsibilities or capabilities required by settled requirements and design.
Identify dependencies between use cases and between those responsibilities.
Identify implementation results already established in the current state.

Apply cross-use-case reuse only where settled requirements, design, repository state, or plan boundaries establish that the same result satisfies each use case.

## Compare remaining work

For each use case, derive the additional responsibilities required beyond established or projected results.
Assess their incremental implementation effort and complexity from the available planning information.

Prefer lighter viable use cases when the available information supports a difference.
Keep tied or uncertain candidates at the same priority.

## Stagger use-case progress

Split each use case into multiple implementation steps that each establish a concrete result.

For each use case, identify the earliest point where established or preceding planned results make its first useful step viable.
Stagger the steps so later use cases enter at those points while earlier use cases continue through their remaining steps.

Prefer this diagonal progression over layer-wide batching or completing each use case in sequence.

## Project the full plan

Build the plan across the full requested scope.

From the established state, project the results each planned milestone would establish.
Recompute affected remaining work from that projected state and continue until the requested scope is represented.

Keep independent branches separate while projecting progress.

## Preserve partial order

Dependencies define required ordering.
Lightweight-first guides priority among viable alternatives.

Leave independent viable work unordered and expose it as parallelizable.

## Replan from progress

After implementation results or repository changes, repeat the mapping, comparison, and projection from the current state across the remaining scope.

This skill governs cross-use-case decomposition, dependency planning, projected progress, and milestone priority.
Detailed implementation-plan structure, design, implementation, delegation, and repository workflows belong to their respective skills.
