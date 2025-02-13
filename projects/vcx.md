# Project Name

VCX

# Preferred Maturity Level

Growth

# Project Description

VCX is an open-source codebase that provides a wide suite of Rust modules for building DID & Aries-related applications (client/mobile and server). VCX is designed with a heavily modularized structure (20+ crates in the workspace) such that consumers can pick-and-choose which components they wish to build their DI application with. Currently, some of the significant modules provided by VCX include:
* `did_doc`, `did_parser`, `did_resolver` - a set of lightweight libraries which provide well-typed structures and interfaces for DID building, parsing, and resolving. We envision these components becoming defacto libraries for Rust projects involving DIDs.
* DID Method Crates - several DID method-specific crates for resolving and managing DIDs (peer, cheqd, web, key, jwk, sov/unqualified).
* `aries_vcx_ledger`, `aries_vcx_wallet`, `aries_vcx_anoncreds` - a set of libraries with interfaces for performing ledger, wallet, and anoncred operations involved in Aries protocols. Includes implementations for Indy & Cheqd ledgers (i.e. resolving anoncreds objects), Askar wallets, and anoncreds-rs.
* `messages` - well-typed library for building and parsing Aries (DIDComm V1) messages
* `aries_vcx` - Implementation of Aries protocol state machines, which provide APIs to step through Aries protocols, utilizing lots of the above-mentioned modules. Currently mostly for AIP1 protocols, but some AIP2 protocols such as DIDExchange/OOB.

VCX has a long history, it has been around since 2017 and is one of the first implementations of an Aries protocol-compliant library, and was originally embedded in the Indy SDK. In 2020, the project was moved into a dedicated Hyperledger project by Absa Group, beginning a new era of development beyond the Indy SDK. Anonyome Labs joined the Hyperledger project in 2022 and the project has been maintained since. VCX has been actively involved in the Aries community, including fortnightly community meetings, and previous participation in Linux Foundation Mentorship programs.

VCX has been used in industry projects, including mediator & cloud applications previously at Absa, and is a core component behind [Anonyome Lab's DI Edge Agent Mobile SDK](https://anonyome.com/resources/blog/aries-vcx-anonyomes-commitment-to-decentralized-identity/). Instnt is also building using VCX as a key component for their Multipass product.

Coming from the Aries ecosystem, VCX has strived to implement protocols that are interoperable with the other Aries frameworks (Credo, ACA-Py). As part of this mission, VCX is apart of the [OWL test harness](https://github.com/openwallet-foundation/owl-agent-test-harness), where it is tested against other OWF Aries implementations.

Given it's long history, VCX had previously grown in legacy code, however recent efforts have pushed VCX inline with modern DI. These efforts include complete replacement of Indy SDK components with indy-vdr, askar & anoncreds-rs, and moving away from unqualified DIDs/resources with alternatives such as Cheqd Anoncred methods.

VCX aims to continue this trajectory. Some current future plans include:
* VCX Framework (in development) - A credo-like framework solution for Rust-based Aries/DI consumers.
* Mobile bindings - Provide Android/iOS mobile bindings to the library, allowing *native* (Kotlin/Swift) mobile applications to utilize VCX functionality.
* More DID methods - continue growing the suite of DID method options, with modern methods such as did:webvh
* DIDComm v2 support

# Alignment with the OpenWallet Foundation Mission

VCX supports the OWF's goals by providing an extensive suite of tools to assist in the creation of secure & interopable DI applications.
* Secure Data Management: Whenever VCX manages data for the consumer, security is always the first consideration. VCX achieves secure data management via utilization of OWF's Askar project for cryptography and encrypted data storage.
* Interoperability: As mentioned, VCX comes from an Aries ecosystem, where interoperability is at the forefront. VCX holds itself accountable to this by participating in efforts such as the OWF OWL test harness.
* Open Source Development: VCX has always been community driven, and encourages participation with efforts such as fortnightly community calls and previous participation in the Linux Foundation Mentorship programs.
* Support for Decentralized Identity: VCX's purpose is to provide tools that make it easier for consumers to develop DI applications. VCX has been proven to succeed in this, with testimonies in the industry (such as from [Anonyome Labs](https://anonyome.com/resources/blog/aries-vcx-anonyomes-commitment-to-decentralized-identity/)).

# Code of Conduct

VCX currently follows the Hyperledger Code of Conduct, which is what the OWF code of conduct is based on.

# TAC Sponsor

Stephen Curran
Second Sponser - TBD

# Project License

Apache 2.0

# Source Control

Project already exists on Github: https://github.com/hyperledger/aries-vcx .

Ideally the new slug would be `vcx`. Dropping the Aries to reflect the capabilities beyond Aries protocols.

# Issue Tracker

https://github.com/hyperledger/aries-vcx/issues

# External Dependencies

The VCX dependency list is maintained in the [source repository](https://github.com/hyperledger/aries-vcx/blob/main/Cargo.toml). All are open source and we believe (but to be verified) that the majority use the Apache 2 License.

TODO - merge workspace dep related PRs for easier dep view

# Release Methodology

All proposed repositories have continuous deployment/delivery pipelines built using GitHub Actions. The individual packages follow the semantic versioning method, ensuring consistency and safety.

VCX publishes release on on an as-needed basis, but releases tend to be made every 4-12 weeks (6 releases were published in 2024).

TBD - VCX does not currently publish any crate releases to crates.io, but would like to in the future. VCX crates are currently "released" via github tags, which Rust consumers consume via github dependencies.

# Initial Maintainers

- George Mulhearn [@gmulhearn](https://github.com/gmulhearn) - Anonyome Labs
- James Ebert - [@JamesKEbert](https://github.com/JamesKEbert) - Instnt
- Luke Li - [@lukewli-anonyome](https://github.com/lukewli-anonyome) - Anonyome Labs

# Proposed Project Governance

The current governance model under Hyperledger is consensus-based. This means that decisions are made through discussions, with the aim of community consensus, as outlined in the Aries Project Charter. In cases where no clear consensus is established, a project Technical Steering Committee, or the maintainers (those with escalated GitHub privileges) are granted a louder voice. This approach has proven effective.

# Financial Sponsorship

Hyperledger has covered infrastructure related costs. 

# Infrastructure

- Github repo
- Discord channel
- Github actions
- Video conference (Zoom)
- Published Artifacts — Cargo, Docker Images, Crates.io (future)
