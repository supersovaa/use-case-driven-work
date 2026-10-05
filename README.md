# use-case-driven-work

A lightweight two-skill workflow for planning and reviewing implementation around concrete user-facing use cases.

## Skills

- `use-case-driven-planning`: build and revise implementation planning state from concrete user-facing use cases.
- `use-case-driven-review`: select the use-case behavior whose test evidence must be reviewed as implementation progress changes.

## Repository dependency

This repository depends on [`requirement-driven-testing`](https://github.com/supersovaa/requirement-driven-testing) for rules governing requirement- and design-backed executable test evidence.

`use-case-driven-work` owns which use-case behavior enters planning or review scope and when combined behavior becomes applicable.
`requirement-driven-testing` owns whether executable tests provide sufficient evidence and how established test evidence is preserved or restored.

Keep those test-evidence rules in the dependency rather than duplicating them in this repository.
