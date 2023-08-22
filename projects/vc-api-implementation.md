# Project Name

VC API Implementation

# Project Description

The VC API is specification for a set of APIs for VC lifecycle management (https://w3c-ccg.github.io/vc-api/). This includes operations such as credential issuance, verification and exchange. It is a W3C CCG work item and, as of the submission of this proposal, it is in “draft community report” status. 

The VC API’s design is informed by use cases across a range of domains. Several of these use cases are collected in a working group note (https://w3c-ccg.github.io/vc-api-use-cases/). 

This project is an implementation of the VC API. The implementation aims to enable organizations and individuals to effortlessly conduct SSI operations over HTTP without requiring technical expertise, making it seamless to integrate into existing projects. 

Easy to adapt new feature requirements and changes since the implementation is generic (can be used for different use-cases, energy use case is one of them). 

The VC API specification was presented to the Open Wallet Foundation Architecture Special Interest Group during the 2023-04-24 meeting (https://github.com/openwallet-foundation/architecture-sig/wiki/2023-04-24-Meeting-Minutes). This project was used during the demonstration portion of the presentation.

## Project Motivation and History 

This project was initiated in late 2021 and has been developed by the Energy Web Foundation (EWF) and the Elia Group. 

The Energy Web Foundation is a non-profit whose mission is to accelerate the energy transition by developing and deploying open-source Web3 technologies that help companies unlock business value from clean and distributed energy resources.  

The Elia Group (https://www.eliagroup.eu/) is an electricity grid transmission system operator operating in Belgium and the north and east of Germany. An important piece of Elia’s mission is to make the energy transition happen to decarbonise Europe by delivering the needed power infrastructure and shaping the European markets. The Elia Group believes that digital transformation is a reality of the changing energy landscape. 

The project was initiated because Energy Web and Elia see a requirement for an API that can be used in the energy sector to issue and verify credentials. Energy Web and Elia believe that an HTTP API lowers the technical barrier to entry for use of SSI, which is important given that organizations which can benefit from SSI often do not have large technical teams dedicated to digital identity. 

Energy Web and Elia chose to implement the VC API specification for the following reasons: 

- An API specification reduces vendor lock-in for consumers choosing to consume the API 
- The VC API specification is developed in an open process 
- The VC API specification prioritizes the relevant design goals of modularity, simplicity, composability and extensibility (https://w3c-ccg.github.io/vc-api/#design-goals-and-rationale)

The API has been used by Energy Web and Elia for demonstration projects such as the Rebeam project, in which verifiable credentials were exchanged to authorize electric vehicle charging. Elia’s summary page for Rebeam is available here: https://innovation.eliagroup.eu/en/projects/rebeam. 

Though the project was initiated and is currently being driven by organizations in the energy domain, the implementation is generic and usable across a range of domains.

## Technical information 

The following section describes technical details of the project. *Please note that Elia and Energy Web have some development resources available to make technical changes to the project in order to enable its adoption by the OWF.*

### Technology selections 

| Technology           | Selection  | Selection Rationale |
|----------------------|------------|----------------|
| Programming language | Typescript | - Energy Web’s primary development language <br> - Among the most popular programming languages, according to Stack Overflow surveys (https://survey.stackoverflow.co/2023/#most-popular-technologies-language-prof) <br> - Widely used in SSI ecosystem |
| API framework | Nest.js (https://nestjs.com/) | - Energy Web’s primary web API development framework |
| Persistence layer | In-memory SQLite | - Ease of setup and development <br> - [A pull request](https://github.com/energywebfoundation/ssi/pull/158) is available which could add support for PostgreSQL |
| Library: credential signatures | DIDKit (https://www.spruceid.dev/didkit) | - Support for many DID methods <br> - Support for both Data Integrity and JOSE VCs (allowing for future JOSE support for this project) <br> - Packaged as libraries for several programming languages, providing future technical agility |

### Implementation details 

#### Key Management 

A VC API implementation which provides the Verifiable Credential issuance (https://w3c-ccg.github.io/vc-api/#issue-credential) or Verifiable Presentation proving (https://w3c-ccg.github.io/vc-api/#prove-presentation) endpoints must have access to private keys (or key services which utilize private keys) in order to create the proofs. However, the API between VC API and a key service is currently out of scope of the VC API specification. 

The project has integrated key material by having a dedicated key module which has HTTP endpoints for the creation, import and export of key material. A tutorial covering key export and import is available here: https://github.com/energywebfoundation/ssi/blob/develop/apps/vc-api/docs/tutorials/key-export-import-tutorial.md.

#### Exchange configuration 

A feature of the VC API specification is support for credential exchanges. This refers to the movement of Verifiable Credentials between actors defined in the Verifiable Credentials Data Model (Issuers, Holders & Verifiers). 

The project has defined a concept of Exchange Definitions in order to specify the configuration of an exchange. Exchange Definitions are documented here: https://github.com/energywebfoundation/ssi/blob/develop/apps/vc-api/docs/exchanges.md#exchange-definitions. The Exchange Definition data model and API endpoints are currently not included in the VC API specification, as noted in this table: https://github.com/energywebfoundation/ssi/tree/develop/apps/vc-api#standard-vs-custom-endpoints. 

However, recent discussions in the VC API working group suggest that APIs for the configuration of exchanges may be included in the specification. An example of these discussions is recorded in this GitHub Issues comment from the 2023-08-08 teleconference: https://github.com/w3c-ccg/vc-api/issues/285#issuecomment-1670228974 

#### Automated Testing 

The project is tested by the two automated test suites which have been developed by the W3C CCG for testing credential issuance (https://github.com/w3c-ccg/vc-api-issuer-test-suite) and credential verification (https://github.com/w3c-ccg/vc-api-verifier-test-suite).

The project is also tested by unit tests and end-to-end tests. 

Integration tests are implemented based on Energy and Mobility use cases, which have historically come from Elia and BloXmove energy and mobility as use-case requirements respectively. 

### Documentation 

The project contains technical documentation and tutorials to facilitate understanding of the API and experiment with the implementation: https://github.com/energywebfoundation/ssi/tree/develop/apps/vc-api/docs/tutorials 

Furthermore, Energy Web has documentation on VC-API and general documentation on SSI available the Energy Web gitbook: 

- https://energy-web-foundation.gitbook.io/energy-web/foundational-concepts/self-sovereign-identity-introduction
- https://energy-web-foundation.gitbook.io/energy-web/ew-dos-technology-components-2023/identity-and-access-management-iam/iam-guides/verifiable-credential-api

# Alignment with the OpenWallet Foundation Mission

The project team believes that the project is well aligned with the OpenWallet Foundation mission. 

An implementation of VC API developed and hosted by the OWF would advance the adoption of interoperable and privacy enhancing digital wallets. This is because VC API is an open specification of an interface for Verifiable Credential operations, which are relevant functions for digital wallets.
Furthermore, as an HTTP API, the project is a technology well understood by many organizations and will plausibly accelerate their efforts to develop or integrate digital wallets. 

In addition, development of a VC API implementation would promote the development and proliferation of the VC API specification itself, which is an open standard related to digital wallets. 

The project has been open source since its inception and aims to be inclusive, in so far as it should be usable across a wide range of domains and infrastructure requirements.

# Current Code of Conduct

https://github.com/energywebfoundation/ssi/blob/develop/apps/vc-api/CODE_OF_CONDUCT.md

# TAC Sponsor

The project has not yet identified a TAC sponsor.

# Project License

GNU General Public License 3.0 -https://github.com/energywebfoundation/ssi/blob/develop/apps/vc-api/LICENSE 

# Source Control

The project source code is at the following location: https://github.com/energywebfoundation/ssi/tree/develop/apps/vc-api 

The git repository containing the code is a monorepo which contains the applications and libraries in the tables below, in addition to the VC API implementation. *To enable the donation of the project to OWF, Energy Web and Elia are willing to refactor the project as required and have the development resources for doing so.* For example, the monorepo could be converted to a simple npm project, with the libraries subsumed in the VC API implementation and the “input-descriptor-to-credential" application separated into a new project and repository. 

### Monorepo Libraries 

| Name     | Location within the repo  | Relevance to the project |
|--------------------|------------|----------------|
| @energyweb/ssi-did | [Repo link](https://github.com/energywebfoundation/ssi/tree/develop/libraries/did) | Imported as a dependency by VC API. Provides generation of DIDs from key pairs |
| @energyweb/w3c-ccg-webkms | [Repo link](https://github.com/energywebfoundation/ssi/tree/develop/libraries/webkms) | Imported as a dependency by VC API. Provides interfaces conforming to the Web KMS specification (https://w3c-ccg.github.io/webkms)

### Monorepo Applications other than VC API 

| Name     | Location within the repo  | Relevance to the project |
|--------------------|------------|----------------|
| @energyweb/input-descriptor-to-credential | [Repo link](https://github.com/energywebfoundation/ssi/tree/develop/apps/input-descriptor-to-credential) | Independent from VC API. The app is an HTTP service to convert a Presentation Exchange input descriptor to a credential to be signed.

# Issue Tracker

https://github.com/energywebfoundation/ssi/issues

# External Dependencies

Key external dependencies are listed below. Not all dependencies are listed.

| Dependency Repository     | Importance to the project   | License |
|--------------------|------------|----------------|
| https://github.com/spruceid/didkit | Provides credential signing and verification | Apache License 2.0 
| https://github.com/decentralized-identity/did-resolver | Resolves DID documents | Apache License 2.0 
| https://github.com/Sphereon-Opensource/PEX | Provides presentation exchange functionality | Apache License 2.0 

# Release Methodology

The project contains a Dockerfile (https://github.com/energywebfoundation/ssi/blob/develop/apps/vc-api/Dockerfile) to build a container image for portable deployment. 

The project repository contains GitHub workflows for: 

Building and testing the repository’s libraries and applications  

Deploying the applications to Energy Web’s infrastructure via a “continuous deployment” workflow 

The project does not yet have a release methodology whereby the application is versioned and built into release artifacts.  

If the project were to be accepted and hosted by the Open Wallet Foundation, Energy Web’s deployment workflow would be removed from the repository hosted by the Open Wallet Foundation.

# Initial Maintainers

- John Henderson - https://github.com/jrhender 

# Proposed Project Governance

The project is currently governed by Energy Web and Elia. The project is not yet a community initiative, and no external feature requests or issues have been received. 

As the core of the project is a specification implementation, some of the project’s design choices will be directed by the specification. The project team has collaborated with the specification’s writer group to receive clarification and guide the specification’s development. The following GitHub issues are examples of this collaboration: 

- https://github.com/w3c-ccg/vc-api/issues/305 
- https://github.com/w3c-ccg/vc-api/issues/330 
- https://github.com/w3c-ccg/vc-api/issues/295 

In general, design and implementation decisions will be drafted and discussed using GitHub Issues prior to implementation. 

Regarding development prioritization, the following categorization is proposed: 
- High priority: If a feature or issue is essential for a specific use case and acts as a blocker. 
- Lower priority: If a feature or issue enhances the current user experience. 
For future requirements, the team recommends considering the use cases defined by the business group or TAC to prioritize development needs. 

*Elia and Energy Web are open to adopting governance practices as suggested by OWF.* 

# Links to Documented Governance Practices

Contribution guidelines: https://github.com/energywebfoundation/ssi/blob/develop/contributing.md  

# Preferred Maturity Level

The requested maturity level is “Labs”.  

Though the project team believes that the “Labs” stage is appropriate, the following points highlight early signs of project usefulness and maturity: 

- This implementation is being utilized by BloxMove proof of concepts to accomplish the next real-world Mobility use-cases. 
- Elia has integrated its wallet with the project, enabling users to leverage it for various energy use cases. 
- The project is accompanied by comprehensive technical documentation and tutorials, aimed at facilitating adoption. 

# Communication Channels

GitHub Issues in the project's repository are enabled and publicly available. The project does not currently have any additional communication channels. 

# Project Website

# Social Media

Elia made a short video to introduce the concept of SSI to newcomers: https://eliagroup.sharepoint.com/:v:/s/InnovationTeam/EUfrphynLWlLsMhJ8mMkjboBxIHTyyoy3RqGalcdFGqn-g?e=JcYOLU  

# Financial Sponsorship

Elia has funded the development of the project and is currently funding maintenance and minor feature development, in the context of initiatives which are ongoing through 2023. Furthermore, Elia has made funding available for any changes required for the project to be donated to the OWF. 

Beyond the context of the ongoing initiatives and donation of the project to OWF, Elia may provide future funding. Questions which Elia plans use to evaluate provision of future funding include: 
- Would the funding enable changes which better align the implementation to the VC API specification? 
- Would the funding enable changes which improve support of the implement for Elia’s use cases? 

# Infrastructure

The following is requested as repository infrastructure:

| Infrastructure Technology | Purpose  |
|---------------------------|----------|
| GitHub Actions | Continuous integration and release workflows |

The following is requested as release artifact infrastructure: 

| Infrastructure Technology | Purpose |
|---------------------------|----------|
| *no technology preference* | Public container image repository |

