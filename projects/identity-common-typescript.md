# Project Name

Identity Common TypeScript

# Preferred Maturity Level

lab

# Project Description

To avoid reinventing the wheel, many identity projects share common needs for data types and utility functions. This project aims to provide a shared library of TypeScript types and utilities for identity-related projects, promoting consistency and reducing duplication across the ecosystem.

Some examples of utils that will added to the common identity libraries:
- X509 certificate parsing, creation and verification
- generic JOSE/JWT implementation, with common validation methods
- generic COSE/CWT implementation, with common validation methods

The goal of the project is to stay lightweight (keep dependencies to a minimum), and platform agnostic (no dependency on platform specific APIs, e.g. Crypto). This ensures that the libraries can be used by a wide range of TypeScript implementing identity features.

# Alignment with the OpenWallet Foundation Mission

By providing a common set of types and utilities, this project helps ensure interoperability between different identity solutions. It supports the OpenWallet Foundation's mission to foster collaboration and standardization in the identity space, making it easier for developers to build compatible and robust identity applications.

There is already intention for the `sd-jwt-js`, `oid4vc-ts`, `openid-federation-ts` and `credo-ts` libraries under OWF to update to the common library. For example an implementation of the JOSE/JWT standard has been made 3 times in those four libraries.

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

Need to check if releases are per package or monorepo wide.

# Initial Maintainers

- cre8 (Mirko Mollik)
- TimoGlastra (Timo Glastra)

# Proposed Project Governance


# Financial Sponsorship

none

# Infrastructure

none