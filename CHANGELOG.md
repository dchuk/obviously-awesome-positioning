# Changelog

All notable changes to this plugin are documented here. The format is based on
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project
adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.2.0] - 2026-06-05

### Added
- 8 fillable artifact templates in `skills/obviously-awesome/templates/`, one
  per command output: `best-fit-customers`, `competitive-alternatives`,
  `unique-attributes`, `value-themes`, `market-frame`, `sales-story`,
  `positioning-diagnosis`, `positioning-review-log`. Each reuses its command's
  exact output structure and encodes the book's hard constraints.

### Changed
- All 7 commands now offer their backing template at the output step and link it
  in their Related-files footer.

## [0.1.0] - 2026-06-05

### Added
- Initial release.
- Auto-activating `obviously-awesome-positioning` skill with 12 reference files.
- 7 commands: `diagnose-positioning`, `identify-best-fit-customers`,
  `list-competitive-alternatives`, `map-value-themes`, `select-market-frame`,
  `build-sales-story`, `review-positioning-health`.
- 2 agents: `obviously-awesome-positioning-planner`,
  `obviously-awesome-positioning-reviewer`.
