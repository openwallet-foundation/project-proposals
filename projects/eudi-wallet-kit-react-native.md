# Project Name
React Native kit for EUDI Wallet reference implementation.

Proposed repository name: `eudi-wallet-kit-react-native`.

# Preferred Maturity Level
Labs

# Project Description
The project is a cross-platform React Native wrapper for [EUDI Wallet reference](https://github.com/eu-digital-identity-wallet/.github/blob/main/profile/reference-implementation.md) implementation.

It allows building cross-platform Mobile Wallet applications compliant with [Electronic Identification, Authentication and Trust Services (eIDAS) Regulation](https://digital-strategy.ec.europa.eu/en/policies/eidas-regulation) and  [EUDI Architecture and Reference Framework (ARF)](https://github.com/eu-digital-identity-wallet/eudi-doc-architecture-and-reference-framework) and based on reference implementations from EUDI ([Android](https://github.com/eu-digital-identity-wallet/eudi-lib-android-wallet-core) and [iOS](https://github.com/eu-digital-identity-wallet/eudi-lib-ios-wallet-kit) correspondingly).

# Alignment with the OpenWallet Foundation Mission
EU has been standardising a concept of [EU Digital Identity (EUDI) Wallet](https://github.com/eu-digital-identity-wallet/eudi-doc-architecture-and-reference-framework) based on self-sovereign identity principles and built upon [eIDAS 2.0](https://digital-strategy.ec.europa.eu/en/policies/eidas-regulation) (Electronic Identification, Authentication and Trust Services) regulation. EU Digital Identity will be available to EU citizens, residents, and businesses who want to identify themselves or provide confirmation of certain personal information. It can be used for both online and offline public and private services across the EU. Every EU citizen and resident in the Union will be able (on a voluntary basis) to use a personal digital wallet.

The European Commission also released an initial [reference implementation of the EUDI Wallet software on GitHub](https://github.com/eu-digital-identity-wallet/.github/blob/main/profile/reference-implementation.md), serving as a foundation for further development by member states.

EUDI Wallet reference implementation consists of native Android and iOS libraries and components. Although developing native mobile applications is a reasonable approach in many cases, it would be great to provide a possibility to easily build a cross-platform Mobile application based on the EUDI Wallet reference components. Such cross platform mobile applications can be used for Demo/PoC purposes, as well as a foundation for custom wallets compliant with EUDI ARF.

React Native was selected as a basis for the project since it allows to develop high-quality cross-platform mobile applications efficiently, leveraging the power of JavaScript and the React ecosystem. React Native is a popular and demanded solution in decentralized identity space.
    
Overall, the proposed project aligns with the OpenWallet Foundation Mission as it
- provides a new open source tool for building cross-platform wallets;
- guarantees wallet interoperability since it's built on top of EUDI ARF, EUDI Wallet reference libraries and corresponding interoperable standards (mDL, SD-JWT, OID4VC, etc.);
- guarantees adoption of the solution since React Native and EUDI Wallet reference libraries are used;
- helps in adoption and development of open standards (EUDI, mDL, SD-JWT, OID4VC, etc.);
- helps in adoption and development of EUDI Wallet initiative which is important for advancing decentralized identity in EU.

# Code of Conduct
[OpenWallet Foundation code of conduct](https://tac.openwallet.foundation/governance/code-of-conduct/)

# TAC Sponsor
To be defined.

# Project License
Apache 2.0.

# Source Control
To be defined. Please note: this is a brand-new source code. The DSR team is working on the initial implementation and may append this section to the nearest feature.

# Issue Tracker
GitHub Issues.

# External Dependencies
As our project is essentially a React Native library, we're going to use a lot of common React/React Native dependencies that are hard to fully list here.

The proposed project is built on top of EUDI wallet reference implementation, so the key dependencies are:
- Apache 2.0 license:
  - [eudi-lib-android-wallet-core](https://github.com/eu-digital-identity-wallet/eudi-lib-android-wallet-core)
  - [eudi-lib-android-wallet-document-manager](https://github.com/eu-digital-identity-wallet/eudi-lib-android-wallet-document-manager)
  - [eudi-lib-android-iso18013-data-transfer](https://github.com/eu-digital-identity-wallet/eudi-lib-android-iso18013-data-transfer)
  - [eudi-lib-jvm-openid4vci-kt](https://github.com/eu-digital-identity-wallet/eudi-lib-jvm-openid4vci-kt)
  - [eudi-lib-jvm-siop-openid4vp-kt](https://github.com/eu-digital-identity-wallet/eudi-lib-jvm-siop-openid4vp-kt)
  - [nimbus.oauth2.oidc.sdk](https://bitbucket.org/connect2id/oauth-2.0-sdk-with-openid-connect-extensions/src/master/)
  - [eudi-lib-ios-wallet-kit](https://github.com/eu-digital-identity-wallet/eudi-lib-ios-wallet-kit)
  - [eudi-lib-ios-wallet-storage](https://github.com/eu-digital-identity-wallet/eudi-lib-ios-wallet-storage)
  - [eudi-lib-ios-iso18013-data-transfer](https://github.com/eu-digital-identity-wallet/eudi-lib-ios-iso18013-data-transfer)
  - [eudi-lib-ios-siop-openid4vp-swift](https://github.com/eu-digital-identity-wallet/eudi-lib-ios-siop-openid4vp-swift)
  - [eudi-lib-ios-openid4vci-swift](https://github.com/eu-digital-identity-wallet/eudi-lib-ios-openid4vci-swift)
  - [OWF identity-credential](https://github.com/openwallet-foundation-labs/identity-credential)
  
Note: the list of dependencies may be changed in the future.

# Release Methodology
Since this is a brand-new codebase, we plan to begin with a simple initial approach for releases and gradually enhance it over time.

**Initial approach**
- GitHub package registry: Dev builds and first releases will be published in GitHub repo package registry .
- Manual publish: Packages will be published manually.

**Target approach**
- NPM Packages: Packages will be published in NPM under OWF org scope.
- CI/CD Pipelines: Automated pipelines to handle integration, testing and publishing.
- Automated Checks: Automated tools to perform code quality and security scans.

# Initial Maintainers
- DSR Corporation Decentralized Systems Team ([Github](https://github.com/orgs/DSRCorporation/teams/decentralized-systems))
- Alexander Shenshin ([GitHub](https://github.com/AlexanderShenshin))

# Proposed Project Governance

--

# Links to Documented Governance Practices

--

# Financial Sponsorship
DSR Corporation, LLC. Denver, Colorado.
DSR Decentralized Systems Team has extensive experience in the development of decentralized systems, digital identity solutions and wallets. DSR team has contributed to more than 50 open source projects. In particular, we are one of the core contributors and maintainers of such open source projects as Hyperledger Indy, Hyperledger Indy Besu, Hyperledger AnonCreds, Hyperledger Aries, [OWF SD-JWT Rust](https://github.com/openwallet-foundation-labs/sd-jwt-rust), etc. DSR team has extensive experience with React Native and participated in development of a number of decentralized identity mobile wallets based on React Native.

# Infrastructure
GitHub Actions for CI/CD
