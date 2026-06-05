# Changelog

All notable changes to this plugin are documented here. The format is based on
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project
adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.4.0] - 2026-06-05

### Added
- 2 P2 templates, completing the per-step set at 14: `trend-layering` (Step 9,
  optional — the three-circle + product-link go/no-go checklist) and
  `master-messaging` (Step 10 — the canonical baseline that stops copy drift).
- Both registered in the skill's `## Templates` registry and offered by the
  planner agent at Steps 9 and 10.

## [0.3.0] - 2026-06-05

### Added
- 4 P1 templates filling the 10-step gaps that have no dedicated command:
  `positioning-team-roster` (Step 2), `vocabulary-and-baggage` (Step 3),
  `target-segment-profile` (Step 7), and `positioning-canvas` (the Five-plus-one
  consolidation that replaces the FOR/IS-A statement). Brings the set to 12.
- A `## Templates` registry in the skill (`SKILL.md`) listing all 12 templates.

### Changed
- The planner agent now offers the matching blank template at Steps 2, 3, 7, and
  the Step 10 capture.
- `/map-value-themes` offers `target-segment-profile.md` at its Step 7 hand-off.

### Fixed
- `SKILL.md` frontmatter `description` is now a single valid quoted scalar (the
  prior multi-line block scalar interfered with skill discovery).

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
