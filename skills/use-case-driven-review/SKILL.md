---
name: use-case-driven-review
description: Review implementation progress by verifying behavioral test coverage for newly established, affected, and combined concrete user-facing use cases at the earliest step where their required behavior is established.
---

# Use-Case-Driven Review

Use this skill when reviewing implementation progress against concrete user-facing use cases.

Use concrete user-facing use cases as the units for relating implementation steps to behavior that must remain covered.

For each use case established by the current implementation step, verify that tests cover every behavior the use case is responsible for preserving.

For each previously established use case affected by the implementation step, preserve the behavioral intent of its tests.
Tests may evolve with the implementation while continuing to verify the behavior they previously protected.

For behavior that emerges from combining use cases, assign its test to the earliest implementation step where all participating use cases are established.
Review each implementation step against behavior whose required use cases are established by that step.
Carry later combined behavior with its assigned future step.

This skill governs use-case-level behavioral review coverage.
General code review, implementation-plan acceptance, implementation, planning, delegation, and repository workflows belong to their respective skills.
