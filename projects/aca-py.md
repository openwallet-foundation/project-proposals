# ACA-Py

## Project Name: ACA-Py

At this time we are planning to keep the name ACA-Py, although we may drop that it is an acronym or change the full name to something that produces the same acronym (perhaps “A Cloud Agent Python” or “ACA-Py is Cloud Agent Python”). Or perhaps someone will come up with a new naming. Naming is hard!

## Preferred Maturity Level

Given the “[1.0.0](https://aca-py.org/latest/CHANGELOG/#100)” maturity of this project, its global recognition (including a [UN “Future of Digital Government” award](https://www.undp.org/policy-centre/singapore/blog/celebrating-future-digital-government)) and its widespread production use, we think ACA-Py should be an “Impact” project at OWF. ACA-Py is broadly used across the world (with [50M+ docker image downloads](https://hub.docker.com/r/bcgovimages/aries-cloudagent)), contains years of evolving contributions, and an [LTS Policy](https://aca-py.org/latest/LTS-Strategy/). ACA-Py includes a “plugins” capability, a [repository](https://plugins.aca-py.org) of up-to-date extensions, and a mature process for contributing and maintaining those plugins.

ACA-Py is a mature and proven project with a large user and contributor base.

## Project Description

ACA-Py (Aries Cloud Agent Python) is an open-source framework designed to facilitate the creation, management, and utilization of decentralized digital identities. ACA-Py enables secure, interoperable communication between entities using decentralized identifiers (DIDs) and verifiable credentials, adhering to standards such as DIDComm, OpenID4VCs and the W3C Verifiable Credentials.

It is both a full implementation of Aries Interop Profile (AIP) 2.0 and a toolkit for building issuers and verifiers beyond the AIP protocols, such as using [OpenID4VCs](https://openid.net/sg/openid4vc/) and the [UN Transparency Protocol](https://uncefact.github.io/spec-untp/) (UNTP). ACA-Py operates in the second and third layers of the [Trust Over IP framework](https://trustoverip.org/toip-model/) using DIDComm messaging and Aries DIDComm and other credential exchange protocols. The "cloud" in the name means that ACA-Py runs on servers (cloud, enterprise, IoT devices, and so forth), and is not designed to run on mobile devices.

While ACA-Py continues to support its initial DIDComm and Aries technical stack, it has evolved to include support for other important Verifiable Credential technologies, including OpenID4VCs and SD-JWTs, W3C VCDM Data Integrity credentials, a variety of DID Methods, and more. The “toolkit” nature of ACA-Py allows for it to be easily deployed in a wide variety of decentralized trust use cases. ACA-Py’s welcoming community and plugin-based extensibility makes it easy for others to build on its strong foundations.

ACA-Py emphasizes security, privacy, and user control, aligning with the broader goals of fostering an open, interoperable, and decentralized identity ecosystem. It is actively maintained and developed by a global community, contributing to the advancement of digital identity solutions.

ACA-Py includes [published documentation](https://aca-py.org/), a formal plugins model with a [repository of maintained plugins](plugins.aca-py.org), a tools repository, a powerful deployment load testing capability, and a repository of example controllers.

## Alignment with the OpenWallet Foundation Mission

ACA-Py supports the OWF’s goals by providing the technological foundation necessary for secure, interoperable, and user-centric digital identity management within open-source digital wallets. Notably, ACA-Py’s goals in common with the OpenWallet Foundation are:

1. **Interoperability**: A core mission of ACA-Py is to enable interoperability between different agents and systems in the decentralized identity ecosystem. It is designed to support various protocols like DIDComm and OpenID4VCs and credential formats like AnonCreds and the W3C Verifiable Credentials Data Model, allowing different entities to communicate securely and efficiently.
2. **Open-Source Collaboration**: As an open-source project, ACA-Py encourages collaboration among developers, organizations, and governments to build and improve decentralized identity solutions. This open-source approach ensures transparency, security, and continuous innovation.
3. **Decentralized Identity**:  ACA-Py is at the forefront of decentralized identity management, providing tools for creating, managing, and using decentralized identifiers (DIDs) and verifiable credentials. ACA-Py enables a user-centric approach to identity, where individuals control their own data and how it is shared.
4. **Security and Privacy**: Security and privacy are foundational to ACA-Py’s architecture, focusing on secure communication, storage, key management and data minimization.

## Code of Conduct

ACA-Py follows the [Hyperledger Code of Conduct](https://github.com/hyperledger/aries-cloudagent-python/blob/main/CODE_OF_CONDUCT.md), which is what the OWF code of conduct is based on.

## TAC Sponsor

* Tracy Kuhrt
* Wenjing Chu

## Project License

The project has an Apache 2.0 license: [ACA-Py - License](https://github.com/hyperledger/aries-cloudagent-python/blob/main/LICENSE)

## Source Control

The project is hosted in GitHub and includes the following repositories:

* [ACA-Py](https://github.com/hyperledger/aries-cloudagent-python) — documentation published to https://aca-py.org
* [ACA-Py Plugins](https://github.com/hyperledger/aries-acapy-plugins) — registry published to [https://plugins.aca-py.org](https://plugins.aca-py.org)
* [ACA-Py Tools](https://github.com/hyperledger/aries-acapy-tools) — various tools related to ACA-Py including those for upgrade data migrations.
* [ACA-Py Controllers](https://github.com/hyperledger/aries-acapy-controllers/blob/main/AliceFaberAcmeDemo/README.md) — demos of Aries ACA-Py controllers (business logic) using different technical stacks.
* [VC-Authn-OIDC](https://github.com/bcgov/vc-authn-oidc) — a multi-tenant OpenIDConnect Identity Provider (IdP) component to enable OIDC Relying Parties to use Verifiable Credential presentations for authentication.

## Issue Tracker

Issues are tracked using GitHub's Issues feature in the corresponding repository.

## External Dependencies

The ACA-Py dependency list is maintained in the [source repository](https://github.com/hyperledger/aries-cloudagent-python/blob/main/pyproject.toml). A NOTICES file is also in the repository, but needs to be updated.

## Release Methodology

All proposed repositories have continuous deployment/delivery pipelines built using [GitHub Actions](https://github.com/features/actions). The individual packages follow the [semantic versioning](https://semver.org/) method, ensuring consistency and safety.

## Initial Maintainers

| Name             | Github          | Organization                             |
| ---------------- | --------------- | ---------------------------------------- |
| Daniel Bluhm     | dbluhm          | Indicio, PBC                              |
| Stephen Curran   | swcurran        | Funded by Government of British Columbia |
| Wade Barnes      | WadeBarnes      | Funded by Government of British Columbia |
| Jamie Hale       | jamshale        | Funded by Government of British Columbia |
| Andrew Whitehead | andrewwhitehead | Funded by Government of British Columbia |
| Clement Humbert  | chumbert        | SICPA                                    |

## Proposed Project Governance

The current governance model under Hyperledger is consensus-based. This means that decisions are made through discussions, with the aim of community consensus, as outlined in the [Aries Project Charter](https://docs.google.com/document/d/1F6RbR7xDaBt5CDJhqLJzR4c1pDJtyPGshp9fy6eVtSM/edit?usp=sharing). In cases where no clear consensus is established, a project Technical Steering Committee, or the maintainers (those with escalated GitHub privileges) are granted a louder voice. This approach has proven effective.

## Links to Documented Governance Practices

[Project Charter for Aries](https://docs.google.com/document/d/1F6RbR7xDaBt5CDJhqLJzR4c1pDJtyPGshp9fy6eVtSM/edit?usp=sharing).

## Financial Sponsorship

Hyperledger has covered infrastructure related costs. Besides that, None.

## Infrastructure

* GitHub repositories
* CI (GitHub actions)
* Bug Tracking (GitHub Issues and GitHub Projects)
* Communication channels (Discord)
* Mailing list
* Video conference (Zoom)
* Wiki / Meeting Pages (Confluence, likely to move to GitHub/Mkdocs)
* Published Artifacts — PyPi, GHCR, mkdocs/GH-Pages
