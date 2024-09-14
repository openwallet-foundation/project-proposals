# Askar

## Project Name: Askar

We plan to keep the name Askar, dropping the “Aries” prefix. The project is well known in the global identity community.

## Preferred Maturity Level

The project should at least be a “Growth”, and arguably, “Impact”, given its maturity, robustness, the number of projects (all Aries frameworks, Credo-TS, and others outside of Aries) in which it is embedded, and the myriad of production deployments of those projects. The project is lacking sufficient documentation and the documentation website, which might hold it back from being an “Impact” project.

## Project Description

Askar is an open-source, secure storage and key management service implemented in Rust (with wrappers for Python and JavaScript/TypeScript), designed to support the needs of decentralized trust systems within and beyond the Aries ecosystem. It is a critical component that securely manages cryptographic keys, credentials, and other sensitive data used in decentralized identity frameworks. Askar is the secure storage/key management solution for Credo-TS, ACA-Py, Identus, Aries VCX, and other decentralized trust projects.

Askar implements a lightweight, efficient, and secure way to store and manage decentralized trust data such as keys, credentials, and DIDs (Decentralized Identifiers). It is designed to work seamlessly with Aries and other decentralized identity agents, ensuring that the data these agents require is stored securely and can be accessed and used as needed. The project focuses on offering robust cryptographic support, including encryption, signing, and key management, all essential for secure decentralized identity operations. Contributors have extended Askar to work with HSM-based keys.

Askar supports various backend storage options from SQLite to Postgres, making it adaptable to different environments and use cases from mobile and IoT to large scale Enterprise deployments. It is designed to be embedded in a wide variety of decentralized trust implementations and includes wrappers for Python and JavaScript/TypeScript (for NodeJS and React Native implementations).

The project is developed and maintained by a community of sophisticated developers that are building Askar into their own digital trust projects and deployments. It contributes to the broader goal of creating secure, scalable, open-source infrastructure for decentralized identity management.

## Alignment with the OpenWallet Foundation Mission

Askar supports the OWF’s goals by providing a secure, scalable technological foundation necessary for storage and key management. Notably, Askar’s goals in common with the OpenWallet Foundation are:

1. Secure Data Management: Askar is designed to provide secure storage for cryptographic keys, credentials, DIDs, and other sensitive data. It emphasizes strong encryption, key management, and secure storage practices, which are critical for ensuring the integrity and confidentiality of digital identity data.
2. Interoperability: Askar is built to be interoperable with various components of the Aries ecosystem and other decentralized identity systems. It supports different backend storage options and is adaptable to a variety of environments from mobile to enterprise, ensuring that it can be used in conjunction with a wide range of digital identity and wallet solutions.
3. Open Source Development:  Askar is an open-source project, inviting collaboration and contributions from developers around the world. This approach ensures that the project benefits from diverse input and continuous improvement, fostering innovation and transparency in the development of secure storage solutions.
4. Support for Decentralized Identity: As a secure storage solution tailored to decentralized identity systems, Askar plays a critical role in enabling decentralized, user-controlled identity management. It ensures that the cryptographic materials required for decentralized identities are stored securely and can be accessed reliably by agents and wallets.

## Code of Conduct

Askar follows the [Hyperledger Code of Conduct](https://github.com/hyperledger/aries-askar/blob/main/CODE_OF_CONDUCT.md), which is what the OWF code of conduct is based on.  

## TAC Sponsor

* Tracy Kuhrt
* TBD

## Project License

The project has an Apache 2.0 and MIT License:  [Askar - Apache License](https://github.com/hyperledger/aries-askar/blob/main/APACHE_LICENSE) and [Askar - MIT License](https://github.com/hyperledger/aries-askar/blob/main/MIT_LICENSE)

## Source Control

The project is hosted in GitHub and includes the following repositories:

* [Askar](https://github.com/hyperledger/aries-askar) — code and documentation for Askar

## Issue Tracker

The issues are tracked using GitHub's Issues feature in the corresponding repository.

## External Dependencies

The ACA-Py dependency list is maintained in the [source repository](https://github.com/hyperledger/aries-askar/blob/main/Cargo.toml).

## Release Methodology

All proposed repositories have continuous deployment/delivery pipelines built using [GitHub Actions](https://github.com/features/actions). The individual packages follow the [semantic versioning](https://semver.org/) method, ensuring consistency and safety. Whenever a pull request is merged into the main branch that doesn't cause a major, minor or patch version increase, an alpha version is released.

## Initial Maintainers

| Name              | Github           | Organization                             |
| ----------------- | ---------------- | ---------------------------------------- |
| Andrew Whitehead  | andrewwhitehead  | Funded by Government of British Columbia |
| Wade Barnes       | WadeBarnes       | Funded by Government of British Columbia |
| Berend Sliedrecht | berendsliedrecht | Animo Solutions                          |
| Timo Glastra      | TimoGlastra      | Animo Solutions                          |

## Proposed Project Governance

The current governance model under Hyperledger is consensus-based. This means that decisions are made through discussions, with the aim of community consensus, as outlined in the [Aries Project Charter](https://docs.google.com/document/d/1F6RbR7xDaBt5CDJhqLJzR4c1pDJtyPGshp9fy6eVtSM/edit?usp=sharing). In cases where no clear consensus is established, a project Technical Steering Committee, or the maintainers (those with escalated GitHub privileges) are granted a louder voice. This approach has proven effective.

## Links to Documented Governance Practices

Hyperledger [Project Charter for Aries](https://docs.google.com/presentation/d/18vMC85R_UqSirTatMQnj7iCFEUX0QP7EZE7lD1FgEa0/edit?usp=sharing).

## Financial Sponsorship

Hyperledger has covered infrastructure related costs. Besides that, None.

## Infrastructure

* GitHub repositories
* CI (GitHub actions)
* Bug Tracking (GitHub Issues and GitHub Projects)
* Communication channels (Discord)
* Mailing list
* Video conference (Zoom)
* Published Artifacts — Cargo, PyPi, NPM
