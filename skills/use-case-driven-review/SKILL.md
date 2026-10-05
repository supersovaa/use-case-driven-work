---
name: use-case-driven-review
description: Review implementation progress by selecting the behavioral test-evidence scope for newly established, affected, and combined concrete user-facing use cases at the earliest step where their required behavior is established.
---

# Use-Case-Driven Review

Use this skill when reviewing implementation progress against concrete user-facing use cases.

Use concrete user-facing use cases as the units for relating implementation steps to behavior that must remain covered.
Use `requirement-driven-testing` to judge the sufficiency and preservation of executable test evidence for that behavior.

For each use case established by the current implementation step, include every behavior the use case is responsible for preserving in the current test-evidence review.

For each previously established use case affected by the implementation step, include its established behavior in the current test-evidence review.

For behavior that emerges from combining use cases, assign its test-evidence review to the earliest implementation step where all participating use cases are established.
Review each implementation step against behavior whose required use cases are established by that step.
Carry later combined behavior with its assigned future step.

This skill governs use-case-level selection and timing of behavioral test-evidence review.
Test-evidence sufficiency and preservation belong to `requirement-driven-testing`.
General code review, implementation-plan acceptance, implementation, planning, delegation, and repository workflows belong to their respective skills.
