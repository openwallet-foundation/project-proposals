# Project Name

mdl-js

# Preferred Maturity Level

Labs

# Project Description

This is a Typescript(Javascript) implementation of the [ISO 18013-5:2021](https://www.iso.org/standard/69084.html) (MDL) specification.

There is only one mdl implementation from Auth0 labs, but they don't support React Native which is most crucial for mobile wallets. This project aims to provide a platform agnostic implementation of the MDL specification.

I guess the main reason for not providing a React Native is that core dependencies like CBOR, COSE and X509 libraries are not available for React Native. So I decided to make them all platform agnostic.

To provide mdl features to Biggest Wallet SDKs like credo or veramo, direction of the project will be:

- Provide a platform agnostic implementation of the MDL specification
- Bring your own crypto
- Modular approach
- Provide platform sepcific helper implementations for developers to use easily

# Alignment with the OpenWallet Foundation Mission

ISO 18013-5 (MDL) is one of the most important standards for digital wallets. The architecture reference framework of the EU also includes MDL.

# Code of Conduct

[OpenWallet Foundation code of conduct](https://tac.openwallet.foundation/governance/code-of-conduct/)

# TAC Sponsor

@aceshim Ace Shim

# Project License

Apache 2.0

# Source Control

https://github.com/lukasjhan/mdoc

# Issue Tracker

https://github.com/lukasjhan/mdoc/issues

# External Dependencies

- js-base64: pure js base64 encoder/decoder

# Release Methodology

Project will be released on NPM. I have `@m-doc` organization on NPM for this project. Package name will be like `@m-doc/mdl`.

# Initial Maintainers

Lukas Han ([Github](https://github.com/lukasjhan))

# Proposed Project Governance

Everyone should be able to contribute to the project. Contributors will be able to open issues via Github to discuss their ideas.

# Links to Documented Governance Practices

# Financial Sponsorship

None

# Infrastructure

None
