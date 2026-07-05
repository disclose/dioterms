# Contributing to dioterms

Thanks for helping improve the **disclose.io Framework**. This repository is the public-domain source of truth behind [disclose.io/framework/](https://disclose.io/framework/) and [policymaker.disclose.io](https://policymaker.disclose.io). Small, well-scoped PRs are easiest to review and land.

> **Not legal advice.** These templates reflect the input of many practitioners and lawyers, but they are not legal advice. Adopters should consult their own counsel for suitability.

## The three pillars — where things live

| Pillar | What it is | Where |
|--------|-----------|-------|
| **Terms** | Legal policy boilerplate | `terms/` (the four canonicals + BBP), `regional/` (jurisdiction variants), `archive/` (frozen history) |
| **Practices** | Operational conduct guidance | `practices/` |
| **Maturity** | The diostatus 6-level model | `maturity/` |

`metadata.yaml` is the machine-readable index of the above. `CODEOWNERS` routes each path to the right reviewers.

## How to contribute, by pillar

- **Canonical term language** (`terms/vdp`, `terms/vdp-with-cvd`, `terms/safe-harbor`, `terms/simple-safe-harbor`) — these mirror policymaker 1:1 and carry legal weight. **Substantive wording changes require an RFC:** open a [GitHub Discussion](https://github.com/disclose/dioterms/discussions) first so the change can be debated, then a PR referencing it. Typo/formatting fixes can PR directly.
- **BBP template** (`terms/bbp/`) — PR directly; RFC for substantive wording.
- **Regional variants** (`regional/`) — fork → add or edit `regional/<file>.md` → PR. New jurisdictions welcome; adapt the safe-harbor language to local law and say what you changed and why.
- **Practices** (`practices/`) — PR against `practices/*.md`. Operational conduct guidance only, not policy templates. External documents may carry their own license (see Provenance below).
- **Maturity** (`maturity/`) — PR against `maturity/*.md`.
- **Translations** — add `<locale>.md` alongside `en-US.md` in a `terms/*/` folder (preserve the exact markdown structure), then add the locale to `terms/languages.json`. Use correct **[BCP-47](https://www.rfc-editor.org/info/bcp47)** codes (`fr-FR`, `de-DE`, `ne-NP` for Nepali, …). *(The legacy `np-NP` misnomer was corrected to `ne-NP` in Phase B — keep policymaker's locale list aligned.)*

## Provenance rules (please read)

Preserving where each term came from is a first-class goal of this repo.

1. **Never delete-and-recreate a file to "move" it.** Always use `git mv` (or GitHub's rename) so `git blame` and authorship survive. History is our provenance record.
2. **Every term file carries a provenance header** — an HTML comment at the top (`<!-- Provenance — … -->`). If you add a term file, copy the header from a sibling and fill it in. HTML comments are invisible when rendered, so they never leak into a published policy.
3. **License.** Everything disclose.io-authored is **[CC0 1.0](./LICENSE)** (public domain). By contributing disclose.io-authored content you agree it is released under CC0. If you contribute a document you did **not** author or that is **not** CC0 (e.g. an externally-published practice), say so in its provenance header and keep the original attribution — see `practices/good-faith-security-research.md` for the pattern.
4. **Don't touch `archive/`.** It preserves deprecated/historical terms as-is.

## Consumers (why renames need coordination)

Two downstream projects read this repo, so **moving or renaming files can break them** — flag such PRs so maintainers can coordinate:

- **`disclose/website`** builds `disclose.io/framework/` from this repo via a git submodule and reads specific paths (`terms/*/en-US.md`, `terms/bbp/en-US.md`, `practices/…`, `maturity/level-*.md`). A path change here needs a matching change in its `scripts/preprocess-framework.js` and a submodule-pin bump.
- **`policymaker.disclose.io`** carries the four canonical templates. Keep `terms/` aligned with it; `terms/languages.json` mirrors policymaker's locale list.

Content-only edits (including provenance headers) don't affect either.

## Checklist before you open a PR

- [ ] Change is scoped to one pillar / one concern.
- [ ] File moves used `git mv` (blame preserved).
- [ ] New term files have a provenance header.
- [ ] Substantive term wording changes link a Discussion (RFC).
- [ ] If a path moved, the PR notes the downstream consumer impact.
- [ ] Legal substance of existing terms is unchanged unless that is the explicit, RFC'd purpose.
