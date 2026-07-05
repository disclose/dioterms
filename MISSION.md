# Mission & Vision — the disclose.io Framework (dioterms)

## Mission

To provide the **canonical, public-domain reference language** for vulnerability disclosure — VDP, bug bounty, and safe-harbor terms — and to steward it **in the open**, so that any organization can adopt clear, defensible disclosure terms for free, and so the language itself improves through **transparent, accountable** community contribution rather than proprietary control.

## Vision

A world where standardized, legally sound disclosure terms are the default — where the canonical language lives in **one open, versioned, community-governed place**; where the tools people use to publish policy ([policymaker.disclose.io](https://policymaker.disclose.io)) and to verify it ([dioseal](https://github.com/disclose/dioseal), [diosts](https://github.com/disclose/diosts), the [directory](https://directory.disclose.io)) **ingest that one source directly**, so what is canonical and what is deployed never drift; and where *how the terms changed* is as public and accountable as the terms themselves.

## Why this repository exists — its two jobs

1. **Canonical reference language.** One authoritative, [CC0](./LICENSE), lawyer-reviewed source for disclosure terms — VDP, VDP-with-CVD, BBP, safe harbor, regional variants, and the diostatus maturity model. If it is the disclose.io language, it lives here, once.

2. **An open-source, accountable way to change it.** Language that carries legal weight must not change in a black box. Every modification is a public pull request, reviewed by named [CODEOWNERS](./CODEOWNERS), recorded in the [CHANGELOG](./CHANGELOG.md) and in git history, with [provenance](./CONTRIBUTING.md#provenance-rules-please-read) preserved on every file. Accountability *is* the product.

## Where it sits in the ecosystem

dioterms is the **STANDARDS** layer of the disclose.io flywheel. The **TOOLS** layer consumes it:

- **[policymaker.disclose.io](https://policymaker.disclose.io)** ingests these templates, so every policy it generates descends from the canonical source.
- **[dioseal](https://github.com/disclose/dioseal)** and **[diosts](https://github.com/disclose/diosts)** verify adoption in the wild.
- **[directory.disclose.io](https://directory.disclose.io)** is the open system of record for who has adopted what.

One source, many consumers, no drift. That single-source-of-truth architecture is the point — it is what makes the language both *canonical* (there is exactly one) and *accountable* (changing it is public and reviewable).

---

> Part of **[disclose.io](https://disclose.io)** — standardizing vulnerability disclosure so that researchers and organizations can work together in good faith. Everything here is [CC0 1.0](./LICENSE): public domain. Fork it, adopt it, adapt it, ship it.
