# Project Name

EUDI (European Digital Identity) Tools TypeScript

# Preferred Maturity Level

lab

# Project Description

EUDI Tools TypeScript enables reusability of tools specific to the EUDI Wallet ecosystem. While the EUDI Wallet is built on open standards such as OpenID4VC, and SD-JWT VC, it requires specific extensions for things like Trust, Payments and document signing. Several projects at OWF already focus on integration with the EUDI Wallet, such as EUDIPLO and Credo. While EUDIPLO is specifically focused on EUDI deployments, other libraries at OWF can be used in any digital credential ecosystem, and so adding EUDI specific business logic will increase the scope of these libraries unnecessarily.

Some examples of tools that will be added to the EUDI Tools TypeScript libraries:
- Implementation of ETSI TS 119 602 that allows creating, parsing, resolving and verifying Lists of Trusted Entities (LoTE).
- Verifying registration and access certificates, and match requested attributes against the registered DCQL queries
- Creation, validation and parsing of EUDI ARF TS 12 Electronic Payment Strong Customer Authentication extensions, such as custom OpenID4VP Transaction Data types, and SD-JWT VC Type Metadata extensions.
- The EUDI Tools TypeScript aims to provide a reusable set of tools implementing EUDI specific standards, protocols and extensions, and is intended to be used in combination with the existing TypeScript projects at OWF.

The initial project will be based on already existing code implemented in:
- [EUDIPLO](https://github.com/openwallet-foundation-labs/eudiplo) (e.g. ETSI List of Trusted Entities implementation)
- [Paradym Wallet](https://github.com/animo/paradym-wallet) (Our open source wallet built on Credo, which has several EUDI-specific extensions implemented)
- [EUDI Wallet Functionality](https://github.com/animo/eudi-wallet-functionality) (Our current open source library implementing some common EUDI specific requirements) 

# Alignment with the OpenWallet Foundation Mission

By providing a common set of tools for integration with the EUDI Wallet ecosystem, this project helps ensure interoperability between different identity solutions. It supports the OpenWallet Foundation's mission to foster collaboration and standardization in the identity space, making it easier for developers to build compatible and robust identity applications.

It also strengthens the integration of existing OWF projects, promoting usage in combination with existing projects, and ensuring OWF projects build on each other instead of reimplementing different tools. These tools are intended to build on the newly proposed Identity Common TypeScript lab, as well as the existing DCQL TS and OpenID4VC TS, and SD-JWT JS projects. It is intended to be used by EUDIPLO and Credo, as well as direct integration for users looking for lower level integration libraries. We have seen good adoption of both higher level OWF projects (such as Credo and EUDIPLO) as well as lower level OWF projects (such as OpenID4VC TS, DCQL TS and SD-JWT JS).

# Code of Conduct

[OpenWallet Foundation code of conduct](https://tac.openwallet.foundation/governance/code-of-conduct/)

# TAC Sponsor

none

# Project License

Apache 2.0

# Source Control

Will be created on Github under the OpenWallet Foundation organization.

# Issue Tracker

Will use Github Issues in the repository.

# External Dependencies

none

# Release Methodology

Probably a monorepo publishing different eudi-specific features.

# Initial Maintainers

- cre8 (Mirko Mollik)
- TimoGlastra (Timo Glastra)
- berendsliedrecth (Berend Sliedrecht)

# Proposed Project Governance

# Financial Sponsorship

none

# Infrastructure

none