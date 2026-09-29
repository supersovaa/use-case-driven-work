---
name: use-case-driven-work
description: Plan implementation by concrete use cases, comparing their remaining plan-level responsibilities against established and projected progress, mapping dependencies across the requested scope, and prioritizing lightweight milestones without imposing unnecessary order.
---

# Use-Case-Driven Work

Use this skill when creating or revising an implementation plan.

Use concrete user-facing use cases as the primary units for relating user-visible progress to implementation work.

## Map use cases and responsibilities

Map the full implementation scope requested by the user before choosing initial work.

For each use case, identify the plan-level implementation responsibilities or capabilities required by already-settled requirements and design.
Represent shared responsibilities once in the planning model.
Treat semantic sharing as planning information; implementation may realize shared responsibilities separately or together according to later implementation decisions.

Identify dependencies between use cases and between those responsibilities.
Identify which responsibilities are already established in the current state.

## Compare remaining work

For each use case, derive the responsibilities still required beyond the established or projected state.
Assess the incremental implementation effort and complexity of that remaining work.

Evaluate the full set of viable use cases.
Prefer lighter use cases as implementation milestones, especially when establishing their remaining responsibilities also reduces the work needed by other use cases.

## Project the full plan

Build the plan across the full requested scope rather than stopping at the first milestone.

From the established state, project the responsibilities each planned milestone would establish.
Recompute remaining work for affected unfulfilled use cases from that projected state and continue until the requested scope is represented.

Keep independent branches separate while projecting progress so projection does not create artificial ordering between them.

## Preserve partial order

Create required ordering only from dependencies.
Lightweight-first is a priority when a sequencing choice is needed, not an additional dependency.

Leave independent viable work unordered and expose it as parallelizable.

## Replan from progress

When revising the plan after implementation results or repository changes, recompute established responsibilities, remaining work, and dependencies across the full remaining scope.
Reevaluate lightweight milestones from that current state while preserving reusable progress.

This skill governs cross-use-case decomposition, dependency planning, projected progress, and milestone priority.
Detailed implementation-plan structure, design, implementation, delegation, and repository workflows belong to their respective skills.
