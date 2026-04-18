# terms/ — the four canonical disclose.io term templates

These are the canonical term templates. They mirror the four template families served by [policymaker.disclose.io](https://policymaker.disclose.io) from its `gh-pages` branch 1:1:

| Folder | Policymaker template | What it is |
|--------|---------------------|------------|
| [`vdp/`](./vdp/) | `disclose-io-vdp` | Full VDP policy boilerplate without a stated coordinated-disclosure window |
| [`vdp-with-cvd/`](./vdp-with-cvd/) | `disclose-io-vdp-with-cvd` | Same, with `{{disclosure_window}} days` specified |
| [`safe-harbor/`](./safe-harbor/) | `disclose-io-safe-harbor` | Standalone full safe-harbor clause |
| [`simple-safe-harbor/`](./simple-safe-harbor/) | `disclose-io-simple-safe-harbor` | Condensed safe-harbor clause |

Each folder contains one file per supported language, named after the locale:

- `en-US.md` — English (US)
- `ar.md` — Arabic
- `np-NP.md` — Nepali

The supported-locale list lives in [`languages.json`](./languages.json).

## Source of truth

**This repo is where the prose lives.** Edit here, PR here, comment here. Policymaker's `gh-pages` branch carries deployed copies used by the Nuxt app at runtime; changes here flow into policymaker on its next release.

If you find policymaker serving something that differs from what's here, the discrepancy should be resolved by updating policymaker — dioterms wins.

## Template variables

These templates use mustache-style placeholders that consumers substitute at render time:

- `{{organization}}` — the organisation's name
- `{{channel}}` — the security reporting channel (email, form URL, platform)
- `{{disclosure_window}}` — days until the coordinated-disclosure timeline expires (default `90`)

See [`../metadata.yaml`](../metadata.yaml) for the canonical variable list and defaults.

## Contributing translations

To add a language:

1. Create `<template>/<locale>.md` in each of the four folders (preserve the exact markdown structure of `en-US.md`).
2. Add the locale to [`languages.json`](./languages.json).
3. Open a PR.

## Licence

[CC0 1.0](../LICENSE). Public domain.
