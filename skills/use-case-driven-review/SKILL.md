---
name: use-case-driven-review
description: Use when reviewing implementation progress in terms of concrete user-facing use cases.
---

# Use-Case-Driven Review

At each implementation step, select evidence for the use cases it establishes or affects. Include combined behavior at the earliest step where its participating use cases are established.

## Select the behavior for this step

For each use case established by the current implementation step, include every behavior the use case is responsible for preserving in the current test-evidence review.

For each previously established use case affected by the implementation step, include its established behavior in the current test-evidence review.

For behavior that emerges from combining use cases, assign its test-evidence review to the earliest implementation step where all participating use cases are established.
Review each implementation step against behavior whose required use cases are established by that step.
Carry later combined behavior with its assigned future step.

## Review the selected evidence

Use the resulting behavior set to select the settled required test definitions that fall within the surrounding review scope.
Apply `test-evidence-review` to those definitions.
When the selected behavior lacks settled required test definitions, return that scope to `test-evidence-planning` rather than deriving test cases during review.

This skill owns use-case-level selection and timing of behavioral test-evidence review.
Required test-case definition belongs to `test-evidence-planning`.
Test-evidence sufficiency belongs to `test-evidence-review`.
Test-evidence preservation and remediation belong to the corresponding skills in the repository's `requirement-driven-testing` dependency.
General code review, implementation-plan acceptance, implementation, planning, delegation, and repository workflows belong to their respective skills.
