---
name: use-case-driven-work
description: Plan implementation by concrete use cases, mapping dependencies over the requested scope, sequencing each work item when its prerequisites are satisfied, and exposing independent work that can overlap.
---

# Use-Case-Driven Work

Use this skill when creating or revising an implementation plan.

Use concrete user-facing use cases as the primary units for relating user-visible progress to implementation work.

## Map the requested scope

Map the full implementation scope requested by the user before choosing the first work item.
Identify the relevant use cases, the work required for each, and dependencies between work items across use cases.

Keep the full requested scope visible so sequencing reflects dependencies throughout the planned work.

## Sequence by dependencies

Derive ordering from prerequisites.
Schedule each work item as soon as its prerequisites are satisfied, whichever use case it belongs to.
Let work from different use cases interleave according to those dependencies.

Show independent ready work as overlapping when the execution environment permits.

## Replan the remaining scope

When revising the plan after implementation results or repository changes, recompute the remaining execution order across the requested scope from the current dependency state.
Update newly ready work across all remaining use cases.

This skill governs cross-use-case dependency planning and sequencing.
Detailed implementation-plan structure, design, implementation, delegation, and repository workflows belong to their respective skills.
