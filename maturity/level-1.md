# Level 1 — Contact Only

The organisation is findable and has a working intake method for security reports. This is typically evidenced by a `security.txt` file and/or a dedicated security contact (email, form, or URL). The bar is deliberately low — it just means a researcher can reach someone. There is no policy document, no legal commitment, and no defined process. But you exist, and you can be found.

## What observers see

- `security.txt` published at `/.well-known/security.txt` (RFC 9116)
- At least one valid `Contact:` entry (email, URL, or phone)
- Optionally: `Policy:`, `Encryption:`, `Acknowledgments:`, `Hiring:`, `Preferred-Languages:`

## Researcher protection

**None in writing.** There's an address to send things to, but no promises about what will happen after you do.

## Path to Level 2

Publish a VDP document at the `Policy:` URL listed in your `security.txt`. At minimum it should describe:

- What you accept reports about (scope)
- How to submit a report
- What researchers can expect back (response cadence, resolution process)

See [terms/core/vdp.md](../terms/) for a starting template.
