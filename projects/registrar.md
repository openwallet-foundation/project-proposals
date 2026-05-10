# Project Name

Registrar

# Preferred Maturity Level

Growth

# Project Description

Registrar is an open-source registrar implementation that provides the trust infrastructure layer for digital wallet ecosystems. It enables Issuers, Verifiers, and Wallets to discover and validate each other through standards-based trust establishment mechanisms, serving as the missing trust anchor that production-grade wallet deployments require.

## Mission

Wallet interoperability does not end at credential formats and protocols — it depends on a working trust layer that every participant can rely on. Our mission is to provide a single, open-source Registrar that any country or ecosystem can adopt to stand up a compliant, interoperable trust infrastructure quickly and consistently — rather than rebuilding the same core component from scratch.

## Phase 1 — EUDI Wallet Ecosystem

Our immediate focus is the EUDI Wallet ecosystem. The first release targets the regulatory and technical baseline required for EU member states to deploy a production-grade Registrar:

- **EU ARF (Architecture and Reference Framework)** — Sections 3.17, 6.6.3, 6.6.5
- **ETSI TS 119 475** — WRPAC/WRPRC profiles and policy requirements
- **CIR 2025/848** — Implementing regulation for WRP certificates

We have already received a Letter of Intent from **France Titres**, validating both the need and the production readiness expectations for this work.

## Phase 2 — Beyond the EU

The same trust-infrastructure problem exists wherever digital wallets are being deployed — across APAC, LATAM, Africa, and other regions building national or cross-border identity systems. Once the EUDI baseline is stable, we will extend the Registrar to support additional trust frameworks, certificate profiles, and discovery mechanisms required by other jurisdictions. Where standards do not yet exist or are insufficient, we will build the necessary technical components and contribute them back to the relevant SDOs.

The long-term goal is a single open-source Registrar that any country can adopt to bootstrap a compliant, interoperable wallet ecosystem — turning trust establishment from a per-jurisdiction engineering project into a shared public good.

# Alignment with the OpenWallet Foundation Mission

The OWF mission explicitly commits to "develop and maintain open source code for wallets to enable and ensure wallet interoperability" and to "collaborate with SDOs in the development and proliferation of open standards related to digital wallets." A Registrar is the trust layer that makes this interoperability operational in practice — without an open-source Registrar, Issuers, Verifiers, and Wallets cannot reliably discover or validate one another, and wallet interoperability fragments at the deployment layer even when the underlying credential formats and protocols are standardized. This project complements existing OWF Technical Projects (credential format and protocol implementations) by filling the trust-infrastructure gap, directly advancing the Foundation's stated goal of enabling secure, privacy-preserving transactions across an interoperable wallet ecosystem.

# Code of Conduct

[OpenWallet Foundation code of conduct](https://tac.openwallet.foundation/governance/code-of-conduct/)

# TAC Sponsor

- Ace Shim

# Project License

Apache 2.0

# Source Control

https://github.com/hopae-official/registrar

# Issue Tracker

https://github.com/hopae-official/registrar/issues

# External Dependencies

TBA

# Release Methodology

Docker-based releases

# Initial Maintainers

- Ace Shim ([Github](https://github.com/pensivej))
- Lukas Han ([Github](https://github.com/lukasjhan))
- Tree Yoon ([Github](https://github.com/yunseorim1116))
- Florent TOURNOIS (florent.tournois@interieur.gouv.fr)
- Anthony CARMOY (anthony.carmoy@interieur.gouv.fr)

# Proposed Project Governance

TBA

# Financial Sponsorship

None

# Infrastructure

None
