---
name: use-case-driven-work
description: Plan implementation by concrete use cases, decomposing them into implementation elements, mapping dependencies across the requested scope, and preferring lightweight use cases that establish reusable progress early.
---

# Use-Case-Driven Work

Use this skill when creating or revising an implementation plan.

Use concrete user-facing use cases as the primary units for relating user-visible progress to implementation work.

## Map use cases and elements

Map the full implementation scope requested by the user before choosing the first work item.
Decompose each use case into the implementation elements it needs, including elements shared by multiple use cases.

Identify dependencies between use cases and between implementation elements.
Also identify overlap and containment between the element sets required by different use cases.

## Prefer lightweight use cases

Among viable use cases, prefer one that can be established with fewer or simpler new implementation elements.

When one use case needs a subset of the elements required by another, prefer establishing the smaller use case first when dependencies allow.
Reuse the established elements when extending the implementation to broader use cases.

Keep only ordering required by dependencies or this lightweight-first preference.
Leave independent work unordered and expose it as parallelizable.

## Replan the remaining scope

When revising the plan after implementation results or repository changes, recompute the remaining use cases, elements, and dependencies from the current state.
Prefer the lightest newly viable use cases while preserving reusable progress.

This skill governs cross-use-case decomposition, dependency planning, and sequencing.
Detailed implementation-plan structure, design, implementation, delegation, and repository workflows belong to their respective skills.
