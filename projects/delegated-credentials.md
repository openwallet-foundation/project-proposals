# Project Name

Delegated Credentials

# Preferred Maturity Level

Labs

# Project Description

## Summary

**Delegated Credentials** is an experimental lab for _credential delegation_: letting a holder
hand a down-scoped, verifiable slice of their credential to a third party — another person, or
an AI agent — so that a verifier can validate the whole delegation chain back to the original
issuer, without the issuer being involved in the delegation.

The lab covers two credential formats in one repository:

1. **SD-JWT VC**, implementing
   [`draft-gco-oauth-delegate-sd-jwt`](https://www.ietf.org/archive/id/draft-gco-oauth-delegate-sd-jwt-00.html)
   (Delegate SD-JWT, G. Oliver / Google), an individual draft pre-adoption in the IETF OAuth WG.
2. **ISO mdoc**, tracking the parallel delegation discussion in the mdoc/mDL community.

The goal is not just to ship libraries, but to produce implementation experience early enough to
influence both specifications while they are still malleable.

## Why this matters now

Selective disclosure lets a holder control _which_ claims are revealed. It does not let them
authorize _someone else_ to act on their behalf: SD-JWT+KB
([RFC 9901](https://www.rfc-editor.org/rfc/rfc9901.html)) proves only that the presenter holds
the key named in `cnf`.

Agentic systems make that gap urgent. An agent booking travel or completing a purchase needs
_"present this credential, for this purpose, up to this amount, until this time, and nothing
more."_ Today's alternatives are all bad: issuer re-issuance for every delegation, sharing the
holder's private key, or dropping to a bearer token and losing issuer-backed assurance. The same
problem underlies guardianship, power of attorney, and corporate authority-to-sign — requirements
that should be tested against the mechanism before it hardens.

## Deliverables

1. A TypeScript implementation of Delegate SD-JWT, tracking the draft as it evolves.
2. An mdoc delegation PoC covering equivalent scenarios.
3. A shared, format-neutral scenario suite (agentic payment, sub-delegation, expiry, revocation,
   chain tampering) and test vectors other implementers can use for interop.
4. A written comparison of the two approaches, and structured feedback to the IETF OAuth WG and
   the mdoc community.

## Relationship to existing OWF projects

Existing OWF projects such as [sd-jwt-js](https://github.com/openwallet-foundation/sd-jwt-js) and
[mdoc-ts](https://github.com/openwallet-foundation-labs/mdoc-ts) maintain production packages.
This work is experimental, so we propose it as a separate project.

# Alignment with the OpenWallet Foundation Mission

OWF builds open source software for interoperable digital wallets. Wallets will need delegation,
and the standards for it are still being written. This lab:

- **Sends implementer feedback to the standards while they can still change.** Working code finds
  problems that spec review does not.
- **Compares SD-JWT and mdoc side by side.** OWF hosts work on both formats, so it is a good place
  to keep the two designs aligned.

# Code of Conduct

The project will adopt the
[OpenWallet Foundation code of conduct](https://tac.openwallet.foundation/governance/code-of-conduct/).

# TAC Sponsor

Ace Shim - [@aceshim](https://github.com/aceshim)

# Project License

Apache 2.0

# Source Control

GitHub

The initial implementation exists at
[https://github.com/Dtitkaio/delegate-sd-jwt](https://github.com/Dtitkaio/delegate-sd-jwt) and
will be contributed to OWF. Proposed destination:
`https://github.com/openwallet-foundation-labs/delegated-credentials`, with the SD-JWT and mdoc
tracks as separate packages in one repository.

# Issue Tracker

GitHub

# External Dependencies

TBD

# Release Methodology

- npm releases
- Semantic versioning

# Initial Maintainers

- Kai Otsuki (NTT Digital) - [@Dtitkaio](https://github.com/Dtitkaio) - author of the initial
  Delegate SD-JWT implementation, maintainer of sd-jwt-vc-dm
- Lukas Han (Hopae) - [@lukasjhan](https://github.com/lukasjhan) - maintainer of sd-jwt-js and
  sd-jwt-vc-dm

# Proposed Project Governance

TBD

# Financial Sponsorship

None.

# Infrastructure

From the OWF [services for projects and labs](https://tac.openwallet.foundation/governance/project-and-lab-services/):

- GitHub repository under `openwallet-foundation-labs`
- Discord channel
- GitHub Actions for CI and releases
- npm organization for package publication
