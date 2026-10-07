---
name: use-case-driven-review
description: Review implementation progress by selecting the behavioral test-evidence scope for newly established, affected, and combined concrete user-facing use cases and applying focused evidence review at the earliest step where their required behavior is established.
---

# Use-Case-Driven Review

Use this skill when reviewing implementation progress against concrete user-facing use cases.

Use concrete user-facing use cases as the units for relating implementation steps to behavior that must remain covered.

For each use case established by the current implementation step, include every behavior the use case is responsible for preserving in the current test-evidence review.

For each previously established use case affected by the implementation step, include its established behavior in the current test-evidence review.

For behavior that emerges from combining use cases, assign its test-evidence review to the earliest implementation step where all participating use cases are established.
Review each implementation step against behavior whose required use cases are established by that step.
Carry later combined behavior with its assigned future step.

Use the resulting behavior set to select the settled required test definitions that fall within the surrounding review scope.
Apply `test-evidence-review` to those definitions.
When the selected behavior lacks settled required test definitions, return that scope to `test-evidence-planning` rather than deriving test cases during review.

This skill owns use-case-level selection and timing of behavioral test-evidence review.
Required test-case definition belongs to `test-evidence-planning`.
Test-evidence sufficiency belongs to `test-evidence-review`.
Test-evidence preservation and remediation belong to the corresponding skills in the repository's `requirement-driven-testing` dependency.
General code review, implementation-plan acceptance, implementation, planning, delegation, and repository workflows belong to their respective skills.
