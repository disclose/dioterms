# Changelog

All notable changes to this repository are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) semantics for its content structure.

## [Unreleased]

### Added
- `practices/` — operational playbooks for running VDPs/BBPs (program-launch, triage, coordinated-disclosure, safe-harbor-implementation, researcher-relations). Seeded with placeholder stubs awaiting community contribution.
- `maturity/` — DIOstatus maturity model as per-level content (`_index.md` + `level-0.md` through `level-5.md`). Migrated from `content/docs/diostatus.md` in disclose/website.
- `CHANGELOG.md` — this file.
- `CODEOWNERS` — scoped review routing for terms vs practices vs maturity.

### Changed
- README reframes the repository as the three-pillar disclose.io framework (terms + practices + maturity) rather than terms-only.

### Notes
- Existing `core-terms-*.md`, `core-terms/`, `regional/`, `simple-safeharbor/`, and `archive/` remain at their current locations. A follow-up PR will restructure them under `terms/` with `git mv` to preserve blame.

## [Pre-2.0]

See git history for changes prior to the introduction of this changelog (2021–2026).
