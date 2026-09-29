---
name: use-case-driven-work
description: Plan implementation by concrete use cases, comparing their remaining plan-level implementation responsibilities against established progress, mapping dependencies across the requested scope, and prioritizing lightweight milestones without imposing unnecessary order.
---

# Use-Case-Driven Work

Use this skill when creating or revising an implementation plan.

Use concrete user-facing use cases as the primary units for relating user-visible progress to implementation work.

## Map use cases and responsibilities

Map the full implementation scope requested by the user before choosing initial work.

For each use case, identify the plan-level implementation responsibilities or capabilities required by already-settled requirements and design.
Represent responsibilities shared by multiple use cases once rather than assigning or duplicating them arbitrarily.

Identify dependencies between use cases and between those responsibilities.
Identify which responsibilities are already established in the current state.

## Compare remaining work

For each use case, derive the responsibilities still required beyond the established state.
Assess the incremental implementation effort and complexity of that remaining work.

Evaluate the full set of viable use cases.
Prefer lighter use cases as implementation milestones, especially when establishing their remaining responsibilities also reduces the work needed by other use cases.

## Preserve partial order

Create required ordering only from dependencies.
Lightweight-first is a priority when a sequencing choice is needed, not an additional dependency.

Leave independent viable work unordered and expose it as parallelizable.

## Replan from progress

When revising the plan after implementation results or repository changes, recompute established responsibilities, remaining work, and dependencies across the full remaining scope.
Reevaluate lightweight milestones from that current state while preserving reusable progress.

This skill governs cross-use-case decomposition, dependency planning, and milestone priority.
Detailed implementation-plan structure, design, implementation, delegation, and repository workflows belong to their respective skills.
