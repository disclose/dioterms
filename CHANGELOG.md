# Changelog

All notable changes to this repository are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) semantics for its content structure.

## [Unreleased]

### Phase B — structural standardization (2026-07-05, all `git mv` — blame preserved)
- `bbp/en-US.md` → `terms/bbp/en-US.md` — BBP now lives under `terms/` with the other term sets (no longer a top-level orphan). `disclose/website` `preprocess-framework.js` + submodule pin updated in lockstep.
- Regional `-draft` suffix retired — `AUS-core-terms-draft.md` → `AUS-core-terms.md`, `GBR-core-terms-draft.md` → `GBR-core-terms.md`; draft status now tracked in each file's provenance header, not the filename.
- `NZD-core-terms-draft.md` → `NZL-core-terms.md` — corrected the country code (`NZD` is a currency code; New Zealand is `NZL`).
- Locale `np-NP` → `ne-NP` across all four canonical folders + `terms/languages.json` — corrected the BCP-47 code for Nepali (`np` is a country code; Nepali is `ne`). **Keep policymaker's locale list aligned.**
- `MISSION.md` added; `metadata.yaml`, `CONTRIBUTING.md`, `CODEOWNERS`, `README.md`, `terms/README.md`, and templates updated to the new paths.
- Note: renaming `bbp/en-US.md` → `terms/bbp/en-US.md` breaks any external `raw.githubusercontent.com` hotlink to the old path — an accepted, deliberate cost of consolidating BBP under `terms/`.

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
- `practices/` — operational-conduct pillar, seeded with `good-faith-security-research.md` (originally published by NextJenSecurity, 2026; reproduced with attribution — author retains rights) and `practices/README.md`.
- `CONTRIBUTING.md` — per-pillar contribution guide covering provenance rules, the RFC flow for term-wording changes, and downstream-consumer coordination.
- `.github/` — pull-request template plus issue templates (regional variant, translation, practice, maturity feedback) and a Discussions-first config for term-wording RFCs.
- **Provenance headers** — every term file (`terms/**`, `bbp/**`, `regional/**`) now opens with a standardized `<!-- Provenance — … -->` HTML-comment block (source, license, and a `git log --follow` pointer). Invisible when rendered; verified against the `disclose/website` build.

### Changed
- **Reconciled term prose with policymaker (authoritative).** The four canonical templates now match policymaker's `gh-pages` templates byte-for-byte in every supported language.
- README restructured around the four canonical templates (plus BBP, regional, maturity, archive).
- `metadata.yaml` — pillars section simplified to `terms` and `maturity`. Added `canonical_templates` section mapping each template to its policymaker counterpart.
- `CODEOWNERS` — path globs updated to the new layout.
- "DIOstatus" → "diostatus" casing normalised across README, metadata, CODEOWNERS, and maturity pages.
- `metadata.yaml` — added the `practices` pillar, a top-level `provenance` policy block, and a `contributing` pointer.
- README — added a Provenance section, a `practices/` navigation row, and a CONTRIBUTING link.

### Moved (with `git mv` to preserve blame)
- `core-terms-vdp.md` → `terms/vdp-with-cvd/en-US.md` (the existing file contained `{{disclosure_window}}` — it was the with-CVD variant).
- `core-terms-bbp.md` → `bbp/en-US.md`.
- `simple-safeharbor/simple-safe-harbor.md` → `terms/simple-safe-harbor/en-US.md`; `simple-safeharbor/` removed.
- `core-terms/` folder (modular section fragments) → `archive/core-terms/`.

### Removed
- The five incomplete "Coming soon" practice stubs — `practices/{coordinated-disclosure,program-launch,researcher-relations,safe-harbor-implementation,triage}.md`. They never carried substantive content. The `practices/` pillar is **retained** for the one complete document (good-faith security research); git history preserves the removed stubs.

### Notes
- Policymaker (`disclose/policymaker`) is treated as the canonical source for term prose drift; dioterms is re-aligned to policymaker where the two diverge. Once this PR lands, the two are 1:1 and future edits to these templates should happen here first, with policymaker picking them up on its next release.

## [Pre-2.0]

See git history for changes prior to the introduction of this changelog (2021–2026).
