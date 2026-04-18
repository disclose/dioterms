# Changelog

All notable changes to this repository are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) semantics for its content structure.

## [Unreleased]

### Added
- `terms/` — the four canonical term templates mirrored 1:1 with policymaker.disclose.io's `gh-pages` templates: `terms/vdp/`, `terms/vdp-with-cvd/`, `terms/safe-harbor/`, `terms/simple-safe-harbor/`. Each provided in `en-US`, `ar`, and `np-NP`.
- `terms/vdp/*` — the plain VDP template (no coordinated-disclosure window) that was previously missing from dioterms but carried by policymaker.
- `terms/safe-harbor/*` — the standalone full safe-harbor clause that was previously only embedded inside the VDP; now exposed as its own template for reuse.
- Translations (`ar`, `np-NP`) for all four canonicals, copied from policymaker.
- `terms/languages.json` — supported-locale manifest, mirrored from policymaker.
- `terms/README.md` — explains the four-canonical layout and the dioterms ↔ policymaker relationship.
- `bbp/` — the existing BBP template relocated here as a fifth canonical (policymaker does not carry BBP; dioterms preserves it for community use).
- `maturity/` — diostatus maturity model as per-level content (`_index.md` + `level-0.md` through `level-5.md`). Migrated from `content/docs/diostatus.md` in disclose/website.
- `CHANGELOG.md` — this file.
- `CODEOWNERS` — scoped review routing.

### Changed
- **Reconciled term prose with policymaker (authoritative).** The four canonical templates now match policymaker's `gh-pages` templates byte-for-byte in every supported language.
- README restructured around the four canonical templates (plus BBP, regional, maturity, archive).
- `metadata.yaml` — pillars section simplified to `terms` and `maturity`. Added `canonical_templates` section mapping each template to its policymaker counterpart.
- `CODEOWNERS` — path globs updated to the new layout.
- "DIOstatus" → "diostatus" casing normalised across README, metadata, CODEOWNERS, and maturity pages.

### Moved (with `git mv` to preserve blame)
- `core-terms-vdp.md` → `terms/vdp-with-cvd/en-US.md` (the existing file contained `{{disclosure_window}}` — it was the with-CVD variant).
- `core-terms-bbp.md` → `bbp/en-US.md`.
- `simple-safeharbor/simple-safe-harbor.md` → `terms/simple-safe-harbor/en-US.md`; `simple-safeharbor/` removed.
- `core-terms/` folder (modular section fragments) → `archive/core-terms/`.

### Removed
- `practices/` — the operational-playbook pillar with its five "Coming soon" stubs. The pillar never carried substantive content; operational how-to guidance belongs on the disclose.io website, not in the terms repo. Git history preserves the stubs.

### Notes
- Policymaker (`disclose/policymaker`) is treated as the canonical source for term prose drift; dioterms is re-aligned to policymaker where the two diverge. Once this PR lands, the two are 1:1 and future edits to these templates should happen here first, with policymaker picking them up on its next release.

## [Pre-2.0]

See git history for changes prior to the introduction of this changelog (2021–2026).
