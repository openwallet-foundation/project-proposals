@@ -1,83 +0,0 @@
# Project Name

KapunSDK

# Preferred Maturity Level

Growth

# Project Description

The SDK consists of a collection of independent modules, where each module implements specific features used for digital identity wallets and verifiers. It is highly customizable and implemented in Kotlin Multiplatform and Rust. Making it available for Android, iOS, JVM and partially for WASM.

The modules are:
  - kapun-credentials: SD-JWT VC, mdoc, BBS, W3C credential format.
  - kapun-crypto: Implements JWT, JWS, and cryptographic helper functions.
  - kapun-dcql: Low-level implementation of the query langugage.
  - kapun-issuance: OID4VCI
  - kapun-pdf: Pdf renderer based on typst.
  - kapun-presentation: OID4VP with transaction data support.
  - kapun-proximity: DC-API over ISO 18013-5 for wallet and verifier side.
  - kapun-trust: Implements the EUDI profile, openid-federation, swiss-profile.
  - kapun-x509: X509 Certificate utility. (Will be added once moved)
  - kapun-zkp: Zero knowledge proof utility. (Will be added once moved)
  - kapun-rdf: RDF utility. (Will be added once moved)
  - kapun-util: Helper functions such as logger, random, platform, etc.
  - kapun-visualization: Oca renderer.
  - kapun-wallet: Wallet SDK that brings everything together.

The project originates from the SPRIND Funke Wallet Competition and has been further extended with research use cases such as BBS ZKP, ZK-JWT (SD-JWT but ZKP), and more to come.

# Alignment with the OpenWallet Foundation Mission

The KapunSDK has been built with a focus on privacy and security. The reusable modules of the SDK allow a high degree of customizability to help build safe and interoperable wallets, issuers and verifiers in the digital identity space. It is implementing the standards that are being adopted by the EU Digital Identity Wallet, mDL, and the Swiss Profile. We are actively collaborating with developers, the standards bodies, and academia.

# Code of Conduct

Will adopt OWF code of conduct.

# TAC Sponsor

N/A

# Project License

Apache 2.0

# Source Control

Project already exists on Github: https://github.com/heidiverse/heidi-sdk. Slug should become kapun-sdk once transferred.

# Issue Tracker

https://github.com/heidiverse/heidi-sdk/issues

# External Dependencies

The KapunSDK dependency list is maintained in the [cargo.toml](https://github.com/heidiverse/heidi-sdk/blob/main/Cargo.toml) for Rust as well as in the [libs.versions.toml](https://github.com/heidiverse/heidi-sdk/blob/main/gradle/libs.versions.toml) file for Kotlin.

The dependencies are open source and most use Apache 2 licenses.

# Release Methodology

- Github actions for CI/CD  
- Tagged releases with changelog entries for each release.

# Initial Maintainers

- Patrick Amrein [@ubamrein](https://github.com/ubamrein)
- Alexey Lebedenko [@lebedenko-ubique](https://github.com/lebedenko-ubique)
- Stefan Mitterutzner [@stmitt](https://github.com/stmitt)
- Christopher Meier [@Mawdie](https://github.com/Mawdie)
- Fabian Aggeler [@UBaggeler](https://github.com/UBaggeler)

# Proposed Project Governance

The projects will mostly be managed by the existing KapunSDK maintainers. We have yet to adopt any formal process but can work with contributors and OpenWallet community to adopt one.

# Financial Sponsorship

The development of this library was funded by Ubique Innovation, which in turns received funding through the SPRIN-D Funke wallet competition.

# Infrastructure

- Github repo
- Github actions
- maven
