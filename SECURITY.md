# Security policy

## Reporting a vulnerability

Email `a@c4.io` with subject line starting `skillweave-marketplace security:`.
For vulnerabilities specific to a listed plugin, report directly to that
plugin's repo (e.g., `skillweave/loom`'s `SECURITY.md`).

Include:

- Which plugin entry is affected.
- Reproduction steps.
- Impact — e.g., pinning drifts, signed-tag bypass, channel-promotion race.

Acknowledgement within 72 hours; triage within seven days. Please do not
open a public GitHub issue for security-sensitive reports.

## Supported versions

Only the current `main` branch is supported. Historical marketplace
snapshots are not patched.

| Branch | Supported |
|---|---|
| `main` | Yes |
| Anything else | No |

## Signed commits

Every commit to `main` is GPG-signed. CI (added in a later alpha) verifies
signatures before merging. Users who pin to a specific commit SHA can audit
the signing fingerprint via `git log --show-signature`.
