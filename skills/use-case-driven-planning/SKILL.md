---
name: use-case-driven-planning
description: Plan implementation from concrete user-facing use cases by growing planning state incrementally, deriving direct dependencies, reusing shared results, arranging viable staged progress, and revising only affected planned work.
---

# Use-Case-Driven Planning

Use this skill when creating or revising an implementation plan from concrete user-facing use cases.

Use concrete user-facing use cases as the primary units for relating user-visible progress to implementation work.

Grow the planning state incrementally from the use cases currently being planned.
A new plan starts from the implementation results and settled requirements already known.
An existing plan starts from its established planning state.

## Grow planning state from use cases

For each use case being planned, identify the responsibilities or capabilities needed to establish its required behavior.
Relate it to implementation results already established or already planned when those results affect the work.

Add dependencies when they determine ordering, reuse, blocking, or the result established by a planned step.
Derive them from the prerequisite results required for each planned result to be established and validated in repository behavior.
When a use case combines results that can be established independently, keep their producing steps independent and place the dependency on the first planned result that requires the combination.
Treat implementation scope and dependency separately: a prerequisite result may stay outside the dependent step's scope.
Represent only direct dependency edges to the prerequisite results a step requires directly; earlier prerequisites remain reachable through those results' own dependencies.
Use isolated test setup as evidence about a result's independent validity rather than as the definition of repository dependencies.
Extend the planning state as later use cases reveal additional relevant relationships.

Before adding work for a new use case, inspect existing implementation paths that already establish the same responsibility.

When required behavior overlaps behavior already established or required by another planned use case, decompose the affected work enough to expose the shared responsibility or capability.
Represent the shared behavior with one established or planned result and make each affected use case depend on that result.
Apply this reuse where settled requirements, design, repository state, or plan boundaries establish that the same behavior satisfies each use case.

Continue until the requested use cases are represented by enough planning structure to guide their implementation.

## Compare remaining work

When choosing what to plan or advance next, compare the viable use cases currently under consideration by deriving the additional responsibilities required beyond established or already planned results.
Assess their incremental implementation effort and complexity from the available planning information.

Prefer lighter viable use cases when the available information supports a difference.
Keep tied or uncertain candidates at the same priority.

## Arrange incremental progress

Split a use case into implementation steps that each establish a concrete result as that use case is added to the plan.

When established or preceding planned results make another use case viable, add its first useful step at that point.
Carry remaining steps forward as their dependencies become satisfied.

Interleave viable use-case steps when this produces earlier user-visible progress.

## Project incrementally

Project the results needed to place the work currently being planned.
After adding a planned milestone, treat its projected result as part of the planning state and reassess work affected by that result.

Extend projection as needed until the requested use cases are represented.
Keep independent branches separate while projecting progress.

## Revise incrementally

When revising an existing plan, start from its established planning state and update the changed portion.
Treat new implementation results and newly established dependencies as changes to that state.
Follow dependent planned work when a changed result affects its requirements or ordering, and continue until the affected planning state is consistent again.

Preserve established planning state outside the affected work.

## Preserve partial order

Dependencies define required ordering.
Lightweight-first guides priority among viable alternatives.

Leave independent viable work unordered and expose it as parallelizable.

This skill governs incremental cross-use-case decomposition, dependency planning, plan revision, projected progress, and milestone priority.
Detailed implementation-plan structure, design, implementation, delegation, review, and repository workflows belong to their respective skills.
