# Project Name

sd-jwt-vc-dm

# Preferred Maturity Level

Labs

# Project Description

This project aims to provide a reference implementation of the SD-JWT VC DM (Selective Disclosure JWT Verifiable Credentials Data Model) specification in TypeScript/JavaScript. SD-JWT VC DM combines the best features of SD-JWT VC and W3C VCDM, offering:

- Selective disclosure capabilities with compact payloads
- Support for schemas and vocabularies
- Compatibility with JSON-LD payloads
- Alignment with JAdES signature standards
- Support for various credential types (Simple credentials, PID, ELM, etc.)

Key features of this implementation:

- Platform-agnostic implementation (works in Node.js, browsers, React Native)
- Modular architecture separating core functionality from platform-specific features
- Pluggable cryptographic interface ("bring your own crypto")
- Support for both compact and JSON serialization formats
- Implementation of all SD-JWT VC DM features including type metadata, schemas, and JAdES signatures
- Comprehensive test suite covering all specification requirements

# Alignment with the OpenWallet Foundation Mission

SD-JWT VC DM is positioned as a crucial credential format that bridges existing standards (SD-JWT VC and W3C VCDM) while adding essential features for real-world deployments. This implementation will help accelerate the adoption of interoperable digital credentials by providing:

- A reference implementation that other projects can learn from
- A production-ready library that wallet developers can directly use
- A test suite that helps ensure specification compliance

# Code of Conduct

[OpenWallet Foundation code of conduct](https://tac.openwallet.foundation/governance/code-of-conduct/)

# TAC Sponsor

@aceshim Ace Shim

# Project License

Apache 2.0

# Source Control

https://github.com/openwallet-foundation/sd-jwt-vc-dm

# Issue Tracker

https://github.com/openwallet-foundation/sd-jwt-vc-dm/issues

# External Dependencies

TBD

# Release Methodology

TBD. hopefully will be released on NPM under OWF NPM organization

# Initial Maintainers

- Lukas Han (Hopae) - [Github](https://github.com/lukasjhan)
- (NTT) - [Github]()

# Proposed Project Governance

The project will follow a shared governance model between Hopae and NTT. All significant changes will require review from both organizations. The project welcomes contributions from the community through GitHub pull requests and issues.

# Links to Documented Governance Practices

# Financial Sponsorship

- Hopae
- NTT

# Infrastructure

- GitHub repository
- NPM organization
- CI/CD pipeline (GitHub Actions)
