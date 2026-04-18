# Changelog

All notable changes to this repository are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) semantics for its content structure.

## [Unreleased]

### Added
- `practices/` — operational playbooks for running VDPs/BBPs (program-launch, triage, coordinated-disclosure, safe-harbor-implementation, researcher-relations). Seeded with placeholder stubs awaiting community contribution.
- `maturity/` — diostatus maturity model as per-level content (`_index.md` + `level-0.md` through `level-5.md`). Migrated from `content/docs/diostatus.md` in disclose/website.
- `CHANGELOG.md` — this file.
- `CODEOWNERS` — scoped review routing for terms vs practices vs maturity.

### Changed
- README reframes the repository as the three-pillar disclose.io framework (terms + practices + maturity) rather than terms-only.
- `core-terms-vdp.md` / `core-terms-bbp.md` — "at least `{{disclosure_window}}` from the initial report" → "at least `{{disclosure_window}} days` from the initial report" (clarifies units; aligns with policymaker template).
- `core-terms-vdp.md` — "Please use `{{channel}}` to report security issues…" → "Please report security issues via `{{channel}}`…" (aligns with policymaker template).
- `simple-safeharbor/simple-safe-harbor.md` — prose rewritten for plainer language (aligns with policymaker template; legal substance unchanged).
- "DIOstatus" → "diostatus" casing normalised across README, metadata, CODEOWNERS, and maturity pages.
- `practices/*.md` stubs reduced to a one-line "Coming soon" plus an upstream PR link; community contribution fills them in.

### Notes
- Existing `core-terms-*.md`, `core-terms/`, `regional/`, `simple-safeharbor/`, and `archive/` remain at their current locations. A follow-up PR will restructure them under `terms/` with `git mv` to preserve blame.
- Policymaker (`disclose/policymaker`) is treated as the canonical source for term prose drift; dioterms is re-aligned to policymaker where the two diverge.

## [Pre-2.0]

See git history for changes prior to the introduction of this changelog (2021–2026).
