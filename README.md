# dioterms — The disclose.io Framework

The canonical, public-domain reference for **vulnerability disclosure policy language**, **operational practices**, and **program maturity** — maintained by the [disclose.io](https://disclose.io) community.

> This repository is the source of truth behind [disclose.io/framework/](https://disclose.io/framework/) and [policymaker.disclose.io](https://policymaker.disclose.io). Everything here is [CC0 1.0](./LICENSE) — public domain. Fork it, adopt it, adapt it, ship it.

> Note: while we've engaged the legal opinion of many, this does not constitute legal advice. Please consult your own counsel for the specific suitability of these terms in your organisation.

## The three pillars

| Pillar | What it is | Directory |
|--------|-----------|-----------|
| **Terms** | Legal policy boilerplate — VDP, BBP, safe harbor, regional variants | `core-terms-*.md`, `core-terms/`, `regional/`, `simple-safeharbor/`, `archive/` |
| **Practices** | Operational playbooks for running a VDP/BBP | [`practices/`](./practices/) |
| **Maturity** | DIOstatus — the 6-level program maturity model | [`maturity/`](./maturity/) |

## Quick Links

| | |
|-|-|
| Generate a personalised policy | [policymaker.disclose.io](https://policymaker.disclose.io) |
| Canonical reference site | [disclose.io/framework/](https://disclose.io/framework/) |
| Community forum | [community.disclose.io](https://community.disclose.io) |
| Compare real-world programs | [disclose.io/programs](https://disclose.io/programs) |

## Navigating the terms

- **Core terms** — primary documents. Maximum flexibility with bilateral safety, readability, and accommodation of varying legal environments. [BBP terms](./core-terms-bbp.md) are a superset of [VDP terms](./core-terms-vdp.md) with additional rewards/scope fields. They are kept separate to avoid ambiguity.
- **[Core modules](./core-terms/)** — modular section fragments derived from the Core terms, used as the basis for regional/vertical translation.
- **[Regional terms](./regional/)** — contributed by PSIRTs, disclosure platforms, policy advocates, and vendor program operators. Adapt safe-harbor language to local legal and regulatory context.
- **[Simple Safe Harbor](./simple-safeharbor/)** — condensed safe-harbor clause designed to add protection language to VDPs and BBPs that are already in place.
- **[Archive](./archive/)** — deprecated or archived terms preserved for reference.

## Navigating the practices

Operational how-to guidance for running a program day-to-day — the counterpart to the legal text in `terms/`. Current stubs:

- [program-launch.md](./practices/program-launch.md) — preflight decisions, scoping, approvals, go-live
- [triage.md](./practices/triage.md) — intake, severity, deduplication, validation, communication
- [coordinated-disclosure.md](./practices/coordinated-disclosure.md) — timelines, negotiation, public disclosure, multi-party
- [safe-harbor-implementation.md](./practices/safe-harbor-implementation.md) — aligning Legal, TOS/AUP, platform agreements
- [researcher-relations.md](./practices/researcher-relations.md) — communication cadence, recognition, escalation

These pages are intentionally thin starting points. Community contribution fills them in over time — [open a PR](https://github.com/disclose/dioterms/pulls).

## Navigating the maturity model

**DIOstatus** is a 6-level self-assessment describing how prepared an organisation is to receive and handle external vulnerability reports.

**Findable → Communicating → Not hostile → Explicitly safe → Accountable.**

See [maturity/](./maturity/) for the per-level definitions and progression guide.

## About Safe Harbor

The core requirements for **Full Safe Harbor** are for the policy to provide:

- Authorisation against anti-hacking laws (CFAA, CMA, equivalent)
- Exemption from anti-circumvention laws (DMCA, equivalent)
- Exemption from violation of the organisation's own TOS/AUP during security testing
- A statement acknowledging good-faith research

The intent is for this language to be followed specifically, with minor modifications if any. If you modify, preserve the four tenets above.

Policies missing any of the core tenets but containing a good-faith non-pursuit commitment meet the criteria for **Partial Safe Harbor**.

> Incentives or "bounties" for vulnerability reports are not a prerequisite for Safe Harbor or for a program to be considered a VDP.

## Disclosure types

- **Coordinated Disclosure** — researcher may share details after a fix has been applied and the program owner has granted permission, or after a clearly-stated time has passed from submission, whichever is sooner.
- **Discretionary Disclosure** — researcher or program owner may request mutual permission to share details after explicit approval.
- **Non-Disclosure** — researchers are required to keep details and the existence of the program confidential. Generally inappropriate for VDPs.

## Additional policy sections (templated)

- **Scope** (required) — explicit "in-scope" assets. Err on the side of inclusiveness.
- **Out-of-Scope** (optional) — systems or activities the organisation discourages testing against.
- **Rewards** (optional, BBPs only) — payment policy and parameters.
- **Official Communication Channels** (required) — complete list of intake methods.
- **Disclosure Policy** (required) — conditions under which researchers may disclose to third parties.

## Contributing

- Regional variants — fork → add `regional/XXX-core-terms.md` → PR
- Core terms changes — RFC-style: open a GitHub Discussion, then a PR
- Practices — PR against `practices/*.md`
- Maturity — PR against `maturity/*.md`
- Translations — fork → add locale files → PR

`CODEOWNERS` routes reviews to the appropriate team.

## Once you've published your policy

- Add the [disclose.io seal](https://github.com/disclose/dioseal) to your public program brief
- Submit a PR to add your program to [diodb](https://github.com/disclose/diodb)
- Let the world know you've joined the initiative
- Contribute back to the framework you just adopted
