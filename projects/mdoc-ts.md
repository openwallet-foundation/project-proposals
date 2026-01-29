# Project Name

mdoc-ts

# Preferred Maturity Level

lab

# Project Description

A TypeScript implementation of ISO 18013-5 (mDL - mobile Driver's License) and ISO 18013-7 standards for issuing and verifying CBOR-encoded mobile documents. The library is designed to work across all JavaScript environments including Node.js, browsers, and React Native.

ISO 18013-5 defines the international standard for mobile driver's licenses. These standards are foundational for digital identity wallets, particularly in mobile contexts where platform compatibility is essential.

## Key Features

The library provides:
- Full implementation of ISO 18013-5:2021 and extensions to create ISO 18013-7 compliant SessionTranscripts.
- CBOR encoding and decoding for mobile documents
- Platform-agnostic architecture with pluggable crypto interface
- Support for Node.js, browsers, and React Native environments
- Zod-based validation and schema enforcement
- Standardized CborStructure class for consistent CBOR handling

The implementation will be extended to support ISO 23220, which is set to release in 2026, defining a generalized way to use mDOCs separate from mDls.

## Evolution from Original Implementation

While this project was initially based on [auth0/mdl](https://github.com/auth0-lab/mdl), the library has diverged greatly from the original implementation with significant architectural improvements:

- **Replaced the crypto implementation** with a pluggable context so it can work in any JavaScript environment (Node.js, browsers, React Native)
- **Reworked the CBOR encoding/decoding** based on a standardized CborStructure class for consistency and maintainability
- **Added zod-based validation** and encoding/decoding for type safety and runtime validation
- **Added updated Session Transcript encoding** for OpenID4VP 1.0 and DC API compliance

These changes make the library fundamentally different from the original, providing a modern, type-safe, and platform-agnostic foundation for mDoc/mDL implementations.

Since several OWF projects already depend on this implementation (Credo/EUDIPLO), we think it would be good to have this library hosted at the OpenWallet Foundation. The authors of the original library have publicly stated that forking is recommended at this point due to lack of time and resources (https://github.com/auth0-lab/mdl/pull/67#issuecomment-3783783755) 

# Alignment with the OpenWallet Foundation Mission

ISO 18013-5 (mDL) and ISO 18013-7 are critical standards for digital wallets, particularly mobile wallets. The European Digital Identity Wallet (EUDI) Architecture Reference Framework explicitly includes support for mDL/mDoc formats, making this library essential for EUDI compliance.

By providing a platform-agnostic, production-ready implementation, this project:
- Enables interoperability between different wallet implementations
- Reduces duplication of effort across the identity ecosystem
- Supports the mission of the OpenWallet Foundation to foster collaboration and standardization
- Provides a foundation that other OWF projects can build upon, such as Credo and EUDIPLO

The library's platform-agnostic design ensures it can be used by a wide range of TypeScript projects implementing mobile document features, from high-level wallet SDKs to low-level integration libraries.

The core COSE/CBOR foundation will be extracted from this library into the newly proposed Identity Common TS, to allow the new COSE/CBOR/CWT Status List to also depend on the same COSE abstraction (which is currently being duplicated in the SD-JWT JS repository).

# Code of Conduct

[OpenWallet Foundation code of conduct](https://tac.openwallet.foundation/governance/code-of-conduct/)

# TAC Sponsor

none

# Project License

Apache 2.0

# Source Control

https://github.com/animo/mdoc

Will be transferred to the OpenWallet Foundation organization upon acceptance.

# Issue Tracker

https://github.com/animo/mdoc/issues

# External Dependencies

- cbor-x: CBOR encoding/decoding (MIT License)
- zod: Schema validation (MIT License)
- zod-validation-error: Enhanced validation error messages (MIT License)

# Release Methodology

The project follows semantic versioning and uses changesets for version management. Releases are published to npm under the `@animo-id/mdoc` package name (to be updated to an OWF namespace upon acceptance). The current version is 0.5.2, with a 0.6.0-alpha ready to be released soon containing improved validation.

# Initial Maintainers

- Timo Glastra - [@TimoGlastra](https://github.com/TimoGlastra)
- Berend Sliedrecht - [@berendsliedrecht](https://github.com/berendsliedrecht)
- Alexis Delamare Deboutteville [@marsouin](https://github.com/marsouin)

# Proposed Project Governance

-

# Financial Sponsorship

none

# Infrastructure

Will utilize standard OpenWallet Foundation services:
- GitHub repository hosting
- CI/CD through GitHub Actions
- npm package publishing