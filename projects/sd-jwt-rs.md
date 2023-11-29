# Project Name

SD-JWT Rust Reference Implementation

# Project Description

This is the reference implementation of the [IETF SD-JWT specification](https://datatracker.ietf.org/doc/draft-ietf-oauth-selective-disclosure-jwt/) written in Rust.

Note: while the project is started as a reference implementation, it is intended to be evolved to a prodaction-ready, high-performance implementations in the long-run.

# Alignment with the OpenWallet Foundation Mission

This library implements the Selective Disclosure for JWTs specification, which is an important building block for future digital identity wallets.
Rust basis may be used as a source for high-performance wallets as well as a universal starting point for native platform-specific implementation for both mobile and desktop.

# Code of Conduct

[OpenWallet Foundation code of conduct](https://tac.openwallet.foundation/governance/code-of-conduct/)

# TAC Sponsor

To be defined.

# Project License

Apache 2.0

# Source Control

To be defined.
Please note: this is a brand-new source code. The DSR team is working on the initial implementation and may append this section to the nearest feature.

# Issue Tracker

GitHub Issues.

# External Dependencies

Dual license (MIT/Apache 2.0) dependencies:
- [base64](https://crates.io/crates/base64)
- [log](https://crates.io/crates/log)
- [serde_json](https://crates.io/crates/serde_json)
- [sha2](https://crates.io/crates/sha2)
- [rand](https://crates.io/crates/rand)
- [hmac](https://crates.io/crates/hmac)

MIT license dependencies:
- [jsonwebtoken](https://crates.io/crates/jsonwebtoken)

Note: the list of dependencies may be changed in the future.

# Release Methodology

To be defined.

# Initial Maintainers

- Sergey Minaev ([Github](https://github.com/jovfer))
- DSR Corporation Decentralized Systems Team ([Github](https://github.com/orgs/DSRCorporation/teams/decentralized-systems)

# Proposed Project Governance

--

# Links to Documented Governance Practices

--

# Preferred Maturity Level

Labs

# Communication Channels

- Github Issues
- Discord channel (https://discord.gg/openwalletfoundation - `#sd-jwt-rust` channel)

# Project Website

To be defined.

# Social Media

--

# Financial Sponsorship

DSR Corporation, LLC. Denver, Colorado.
DSR Decentralized Systems Team has extensive experience in the development of decentralized systems and digital identity solutions, and we are fun of Rust.
In our previous experience, we developed a Rust-based multiplatform SDK for the Hyperledger Indy project, which later evolved into the Aries initiative.
The DSR team is also one of the initial authors of Rust-based CL Anoncreds implementation as part of Hyperledger Ursa and Indy. CL Anoncreds is one of the alternative approaches for verifiable credentials with selective disclosure support.

# Infrastructure

GitHub Actions for CI/CD.
