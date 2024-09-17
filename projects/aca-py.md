# ACA-Py

## Project Name: ACA-Py

At this time we are planning to keep the name ACA-Py, although we may drop that it is an acronym or change the full name to something that produces the same acronym (perhaps “A Cloud Agent Python” or “ACA-Py is Cloud Agent Python”). Or perhaps someone will come up with a new naming. Naming is hard!

## Preferred Maturity Level

Given the “[1.0.0](https://aca-py.org/latest/CHANGELOG/#100)” maturity of this project, its global recognition (including a [UN “Future of Digital Government” award](https://www.undp.org/policy-centre/singapore/blog/celebrating-future-digital-government)) and its widespread production use, we think ACA-Py should be an “Impact” project at OWF. ACA-Py is broadly used across the world (with [50M+ docker image downloads](https://hub.docker.com/r/bcgovimages/aries-cloudagent)), contains years of evolving contributions, and an [LTS Policy](https://aca-py.org/latest/LTS-Strategy/). ACA-Py includes a “plugins” capability, a [repository](https://plugins.aca-py.org) of up-to-date extensions, and a mature process for contributing and maintaining those plugins.

The following sub-sections how ACA-Py meets OpenWallet Foundation maturity level criteria for Growth and Impact projects.

### Growth

* 2 TAC sponsors to champion the project and provide mentorship as needed.
* Development of a growth plan, to be done in conjunction with their project mentor(s) at the TAC.
* Development of a project roadmap that provides differentiated features and capabilities and the timeframe for completion.
    * Defined Roadmap Activities:
        * Broader DID registration support, including did:web, did:tdw and others.
        * Integration with Servers for publishing did:web and did:tdw DIDs
        * Encouragement of [plugins](https://plugins.aca-py.org) publication and continued optimization of plugins
        * Expanded support for OpenID4VCs, largely implemented as a [plugin](https://plugins.aca-py.org/latest/oid4vc/)
        * Expanded SD-JWT issuing and verification support, based on the OWF [sd-jwt-py](https://github.com/openwallet-foundation-labs/sd-jwt-python) project.
        * Support for DIDComm v2 and [TSP](https://trustoverip.github.io/tswg-tsp-specification/)
        * Orderly deprecation of AIP v1.0 features
* Document that it is being used successfully in either proof of concepts or pilots by at least two independent end users which, in the TAC’s judgment, are of adequate quality and scope.
    * [Government of British Columbia](https://digital.gov.bc.ca/digital-trust/home/)
    * [Indicio, PBC](https://indicio.tech/)
    * [AYANWORKS](https://www.ayanworks.com/)
    * [Anonyome Labs](https://anonyome.com/)
    * [DIDx](https://www.didx.co.za/)
    * [Northern Block](https://northernblock.io/)
    * [CPQD](https://www.cpqd.com.br/)
    * [SCOPEfusion](https://scopefusion.net/)
    * [GAN](https://gan.foundation/)
    * Open Security and Identity inc.
* Demonstrate a substantial ongoing flow of commits and merged contributions.
    * 100 [Contributors](https://github.com/hyperledger/aries-cloudagent-python/graphs/contributors) since project inception
    * [314 PRs merged since 2024.01.01](https://github.com/hyperledger/aries-cloudagent-python/pulls?q=is%3Apr+is%3Amerged+merged%3A%3E2024-01-01+)
    * [50M+ Docker Hub pulls](https://hub.docker.com/r/bcgovimages/aries-cloudagent)
* Demonstrate that the current level of community participation is sufficient to meet the goals outlined in the growth plan and roadmap.
    * Contributors driven by organizations with diverse goals — [AIP v2.0](https://github.com/hyperledger/aries-rfcs/tree/master/concepts/0302-aries-interop-profile#aries-interop-profile-version-20) and beyond, OpenID4VCs, DIDComm v2, mDL, [UN Transparency Protocol](https://uncefact.github.io/spec-untp/), [W3C VC-API](https://w3c-ccg.github.io/vc-api/), technical debt elimination, and so on. The community participation allows for coherent progress on a variety of goals in parallel. The maintainer community coordinates the additions, recommending new features be added in the core and in plugins.
* Since these metrics can vary significantly depending on the type, scope and size of a project, the TAC has final judgment over the level of activity that is adequate to meet these criteria.
* Demonstrates how this project differs from existing projects in the Growth and Impact stages.
    * ACA-Py is a companion to the [Credo-TS](https://github.com/openwallet-foundation/credo-ts) and [Bifold Wallet](https://github.com/openwallet-foundation/bifold-wallet) projects— a server side digital trust framework and toolkit.
    * ACA-Py has a dependency on the OWF [sd-jwt-py](https://github.com/openwallet-foundation-labs/sd-jwt-python) project.
    * Several other OWF Projects are candidates to be imported into ACA-Py.

### Impact

* Have a defined governing body of at least 5 or more members (owners and core maintainers), of which no more than one-third is affiliated with the same employer. In the case there are 5 governing members, 2 may be from the same employer.
    * [Government of British Columbia](https://digital.gov.bc.ca/digital-trust/home/)
    * [Indicio, PBC](https://indicio.tech/)
    * [AYANWORKS](https://www.ayanworks.com/)
    * [Anonyome Labs](https://anonyome.com/)
    * [Northern Block](https://northernblock.io/)
    * [CPQD](https://www.cpqd.com.br/)
* Have a documented and publicly accessible description of the project's governance, decision-making, and release processes.
    * Initially the [Aries Project Charter](https://docs.google.com/document/d/1F6RbR7xDaBt5CDJhqLJzR4c1pDJtyPGshp9fy6eVtSM/edit?usp=drive_link) and Aries [TSC.md](https://github.com/hyperledger/aries/blob/main/TSC.md) and [MAINTAINERS.md](https://github.com/hyperledger/aries/blob/main/MAINTAINERS.md) and evolving them to be ACA-Py specific in the OWF context.
* Have a healthy number of maintainers from at least two organizations. A maintainer is defined as someone with the commit bit; i.e., someone who can accept contributions to some or all of the project.
    * 100 total [contributors](https://github.com/hyperledger/aries-cloudagent-python/graphs/contributors)
    * Maintainers are currently from 2 Organizations (BC Gov, Indicio), but we have a number of other contributors more than capable of being maintainers, with the process started for one to become a maintainer.
* Have a Code of Conduct in a form acceptable to the OpenWallet Foundation.
    * Based on the Hyperledger Code of Conduct
* Explicitly define a project governance and maintainer process. This is preferably laid out in a GOVERNANCE.md file and references a CONTRIBUTING.md and MAINTAINERS.md file showing the current and emeritus maintainers (see MAINTAINERS.md File Contents for more information).
    * Initially the[ Aries Project Charter](https://docs.google.com/document/d/1F6RbR7xDaBt5CDJhqLJzR4c1pDJtyPGshp9fy6eVtSM/edit?usp=drive_link) and Aries[ TSC.md](https://github.com/hyperledger/aries/blob/main/TSC.md) and[ MAINTAINERS.md](https://github.com/hyperledger/aries/blob/main/MAINTAINERS.md) and evolving them to be ACA-Py specific in the OWF context.
* Document that it is being used successfully in production by at least two independent end users which, in the TAC’s judgment, are of adequate quality and scope.
    * [Government of British Columbia](https://digital.gov.bc.ca/digital-trust/home/)
    * [Indicio, PBC](https://indicio.tech/)
    * [AYANWORKS](https://www.ayanworks.com/)
    * [Anonyome Labs](https://anonyome.com/)
    * [DIDx](https://www.didx.co.za/)
    * [Northern Block](https://northernblock.io/)
    * [CPQD](https://www.cpqd.com.br/)
* Have a public list of project adopters for at least the primary repo (e.g., ADOPTERS.md or logos on the project website).
    * We have not collected this information to now, but will add it to the repo.
* Have a good standing with respect to security.
    * We have excellent practices around the use of dependabot, and the regular updating of all dependencies, including a track record of updating the version of Python supported.
* Other metrics as defined by the applying Project during the application process in cooperation with the TAC.
* Receive a supermajority vote from the TAC to move to Impact stage. Projects can move directly from Labs to Impact, if they can demonstrate sufficient maturity and have met all requirements.

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

The ACA-Py dependency list is maintained in the [source repository](https://github.com/hyperledger/aries-cloudagent-python/blob/main/pyproject.toml). A NOTICES file is also in the repository, but needs to be updated. All of the
dependencies are open source, and we believe most use the Apache 2 license, but some legwork may be required to verify that.

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
