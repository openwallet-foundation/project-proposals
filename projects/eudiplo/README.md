# Project Name

EUDIPLO

## Preferred Maturity Level

Growth

## Project Description

EUDIPLO is an open-source middleware project designed to simplify integration with the European Digital Identity Wallet (EUDI Wallet) ecosystem.

What it is and what it does: EUDIPLO provides a developer-friendly integration layer and JSON-first APIs that help organizations issue and verify digital credentials without needing deep protocol expertise. It is focused on practical adoption by implementers in public and private sectors.

Core capabilities include:

* Credential issuance and verification workflows for EUDI-aligned use cases.
* Support for key protocols and formats including OID4VCI, OID4VP, and SD-JWT VC.
* Containerized deployment (Docker) for fast local setup and environment portability.
* A standards-first architecture intended to reduce vendor lock-in and support interoperability testing.

Why it is valuable: EUDIPLO helps reduce ecosystem complexity and lowers implementation barriers for teams adopting digital credentials in Europe.

* It enables faster prototyping and production onboarding through a lightweight middleware approach.
* It bridges protocol complexity behind practical APIs for issuer and verifier integrations.
* It supports interoperability goals by implementing open standards and encouraging transparent, open-source collaboration.

Origin and History: EUDIPLO was initiated to provide a focused, EUDI-native middleware path comparable in developer experience to agent-based ecosystems while remaining aligned with OWF values.

Key milestones include:

* 2025-09-17: Public webinar held to present architecture and implementation approach.
* 2026-01 to 2026-03: Frequent tagged releases published, indicating active maintenance and iterative delivery.
* 2026-02-19: v2.0.0 released with security and configuration hardening updates.
* 2026-02-27: v3.0.0 released with migration infrastructure and major operational changes.
* 2026-03-23: v4.0.0 released with protocol route/API restructuring and additional production-focused improvements.

The project started around July 2025 to build an MVP that could be used to test wallets and validate protocol implementations needed for the EUDI Wallet ecosystem.

Adoption signals are already visible through issue activity and Discord channel feedback. Specific company names are intentionally omitted until permission is granted.

What the project will include (scope and deliverables):

* Public source repository with implementation code, examples, and integration documentation.
* Stable APIs and middleware components for issuer and verifier scenarios.
* Docker images and deployment guidance for local, test, and production-like setups.
* Conformance and interoperability assets aligned with evolving EUDI and OWF ecosystem expectations.
* A 6-12 month roadmap focused on continued conformance hardening, protocol profile expansion, and operational maturity.
* Explicit next-phase deliverables include:
  * Full compatibility with all required features by end of year.
  * A benchmark test suite and published performance results.
  * Better monitoring and observability support.
  * Integration with registrars provided by each member state to manage access and registration certificates.
  * Interaction with the catalog of attestations.

![Overview](overview.excalidraw.svg)

## Alignment with the OpenWallet Foundation Mission

EUDIPLO aligns with the OpenWallet Foundation mission by advancing open, interoperable, and secure digital identity infrastructure.

* Open Source Availability: EUDIPLO is developed as open source and intended for broad community use.
* Interoperability and Standards: EUDIPLO is built around open protocols (OID4VCI, OID4VP, SD-JWT VC, mDOC ISO 18013-5, OAuth Token Status List) and reports OIDF conformance testing for OID4VCI and OID4VP.
* Adoption Enablement: EUDIPLO lowers technical barriers for issuers and verifiers entering the EUDI ecosystem.
* Community Collaboration: The project is intended to evolve with contributions, feedback, and shared implementation lessons.

Community interaction is active through public issues and Discord feedback loops, and the project roadmap is shaped by this implementation feedback.

A bi-weekly community call will start on 14 May 2026 to improve alignment and strengthen community building.

Multiple projects or companies are already using EUDIPLO in early testing and development like:

* [Intesi Group](https://www.intesigroup.com/)
* [German EUDI Wallet project](https://playground.eudi-wallet.org/)
* [Raiffeisen Bank International](https://www.rbinternational.com/)

## Code of Conduct

The project has a published Code of Conduct:[Code of Conduct](https://github.com/openwallet-foundation-labs/eudiplo/blob/main/CODE_OF_CONDUCT.md)

The project also aligns with OWF community conduct expectations.

## TAC Sponsor

* Ace
* Stephen Curran

## Project License

Apache License 2.0

[License file](https://github.com/openwallet-foundation-labs/eudiplo/blob/main/LICENSE)

## Source Control

[GitHub Repository](https://github.com/openwallet-foundation-labs/eudiplo)

## Issue Tracker

[GitHub Issues](https://github.com/openwallet-foundation-labs/eudiplo/issues)

## External Dependencies

EUDIPLO is designed to run self-contained via Docker, with dependencies primarily coming from open-source protocol and runtime libraries.

Key external tooling dependencies include:

* Docker and Docker Compose for deployment/runtime packaging.
* Node.js and pnpm for workspace build tooling.
* Semantic Release for automated release/versioning.
* Dependency licensing is restricted to open-source licenses, and a license checker is used in the delivery flow to ensure license compliance before changes are merged into main.

## Release Methodology

EUDIPLO uses Semantic Versioning (SemVer 2.0.0) with automated semantic-release workflows from the main branch.

* The main branch reflects active development.
* Stable releases are tagged and published with release notes.
* Container images are versioned and published for stable versions.
* Release automation is configured through semantic-release plugins (commit analysis, changelog generation, npm publish, GitHub release, and Docker publish hooks).
* The repository currently shows frequent releases (multiple releases per month in early 2026).
* Latest tagged release at time of writing: v4.0.0 (2026-03-23).

## Initial Maintainers

* @cre8
* @lukasjhan

## Proposed Project Governance

The project is currently led by maintainers listed in MAINTAINERS.md with open participation through issues and pull requests.

Governance will emphasize transparent decision-making, roadmap visibility, and contributor onboarding.

Current governance and collaboration signals include:

* Public contribution process via CONTRIBUTING.MD.
* Public issue tracking and labeling for community contribution (including good first issue labels).
* Maintainer roster documented at: [Maintainers](https://github.com/openwallet-foundation-labs/eudiplo/blob/main/MAINTAINERS.md)

A concrete feature acceptance and project decision process will be formalized during the Growth phase. Input from proven OWF governance models is explicitly welcomed.

## Financial Sponsorship

No financial sponsorship is required at this time because no project services are hosted.

## Infrastructure

Current project infrastructure is repository-driven and includes:

* GitHub repository, issues, pull requests, and Actions-based CI/CD.
* GitHub Releases and package publication workflows.
* Documentation publishing via GitHub Pages (versioned docs).
* Code quality/security integrations (for example Codecov and SonarCloud references in repository documentation).

No additional OWF-managed infrastructure is requested at this stage. The project currently avoids running a hosted external testing instance because this could introduce GDPR risk if users submit personally identifiable information (PII).
