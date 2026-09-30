---
name: use-case-driven-work
description: Plan and review implementation by concrete use cases, splitting each use case into staged work, arranging overlapping step streams across viable use cases, mapping dependencies across the requested scope, comparing remaining plan-level work against established and projected results, reviewing established use cases through behavioral test coverage, and favoring lighter milestones when evidence supports a difference.
---

# Use-Case-Driven Work

Use this skill when creating or revising an implementation plan or reviewing implementation progress.

Use concrete user-facing use cases as the primary units for relating user-visible progress to implementation work.

Keep plan-level dependencies and the results established by planned work explicit enough to support incremental revision.

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

## Arrange diagonal progress

Split each use case into multiple implementation steps that each establish a concrete result.
Treat each use case as a stream of those steps.

For each stream, identify the earliest point where established or preceding planned results make its first useful step viable.
Streams with the same earliest viable point may start together.
Place each stream at that point and carry its remaining steps through subsequent milestones.

Combine the streams so their steps overlap across the plan, producing diagonal progression across use cases.

## Project the full plan

Build the plan across the full requested scope.

From the established state, project the results each planned milestone would establish.
Recompute affected remaining work from that projected state and continue until the requested scope is represented.

Keep independent branches separate while projecting progress.

## Revise incrementally

When revising an existing plan, reuse established plan relationships and update the affected portion.
Propagate changes through dependent planned work until its dependencies are satisfied again.

## Review by use-case behavior

For each use case established by the current implementation step, verify that tests cover every behavior the use case is responsible for preserving.

For each previously established use case affected by the implementation step, preserve the behavioral intent of its tests.
Tests may evolve with the implementation while continuing to verify the behavior they previously protected.

For behavior that emerges from combining use cases, assign its test to the earliest implementation step where all participating use cases are established.
Review each implementation step against behavior whose required use cases are established by that step.
Carry later combined behavior with its assigned future step.

## Preserve partial order

Dependencies define required ordering.
Lightweight-first guides priority among viable alternatives.

Leave independent viable work unordered and expose it as parallelizable.

## Replan from progress

When new implementation results or newly established dependencies affect the remaining plan, update the affected planning state and propagate their effects through dependent remaining work.

This skill governs cross-use-case decomposition, dependency planning, incremental plan revision, projected progress, milestone priority, and use-case-level review coverage.
Detailed implementation-plan structure, design, implementation, delegation, and repository workflows belong to their respective skills.
