# ESSI Studio

## Project Name

ESSI Studio (Enterprise Self-Sovereign Identity Studio)

## Preferred Maturity Level

Labs

ESSI Studio is a comprehensive credential management platform that is production-ready but seeking community adoption and collaboration within the OWF ecosystem. As a Labs project, we aim to:

- Gain visibility within the OWF community
- Collaborate with related projects (Credo-ts, Bifold Wallet, ACA-Py)
- Build a diverse contributor community
- Work toward Growth stage maturity

## Project Description

ESSI Studio is a comprehensive open-source platform for issuing, managing, and verifying digital credentials built on open standards. It provides a complete solution for organizations to implement Self-Sovereign Identity (SSI) and Verifiable Credentials infrastructure.

### Core Capabilities

**Credential Management**
- Visual drag-and-drop credential designer for creating branded credential cards
- Schema management with support for multiple DID methods (did:web, did:key, did:kanon)
- Credential definitions with OCA (Overlay Capture Architecture) branding overlays
- Multi-format credential support: AnonCreds, SD-JWT, mDocs (ISO 18013-5), OpenBadges 3.0

**Issuance & Verification Protocols**
- **OID4VCI** - OpenID for Verifiable Credential Issuance (wallet-initiated flows)
- **OID4VP** - OpenID for Verifiable Presentations (QR-code and deep-link verification)
- **DIDComm v1/v2** - Peer-to-peer secure messaging and credential exchange
- **ISO 18013-5** - Mobile driver's license (mDL) and mdoc credential support

**Advanced Features**
- OpenBadges 3.0 credential issuance and verification
- Workflow engine for multi-step credential issuance
- P2P video calls with WebRTC for remote identity verification
- P2P document and PDF signing with verifiable credentials
- Post-quantum cryptography support (ML-KEM-768 key encapsulation)
- Proof of Execution (POE) for zero-knowledge proof verification
- Institutional credential provider integrations

### Architecture

```
essi-studio/
├── frontend/                    # Next.js 15 frontend application
│   ├── app/                     # App router pages and components
│   └── lib/                     # State management and utilities
├── backend/                     # Express.js backend with Credo-ts agent
│   └── src/
│       ├── routes/              # API route handlers
│       ├── services/            # Business logic and agent services
│       └── db/                  # Database schema and queries
├── packages/                    # Shared workflow SDK packages
│   ├── workflow-client/         # Browser SDK for workflows
│   ├── workflow-react/          # React hooks and components
│   └── workflow-backend-express/ # Express middleware
└── docker-compose.yml           # Production deployment
```

### Technology Stack

| Layer | Technologies |
|-------|--------------|
| **Frontend** | Next.js 15, React 19, TypeScript, Tailwind CSS, Zustand, Craft.js |
| **Backend** | Express.js, TypeScript, Credo-ts (OWF project) |
| **Database** | PostgreSQL 15+ with Aries Askar wallet storage |
| **Cache** | Redis (for horizontal scaling and pub/sub) |
| **Protocols** | DIDComm v1/v2, OID4VCI, OID4VP, OpenBadges 3.0, ISO 18013-5 |
| **Cryptography** | Ed25519, BBS+, ML-KEM-768, AES-GCM |

## Alignment with the OpenWallet Foundation Mission

ESSI Studio strongly aligns with OWF's mission to develop secure, interoperable, and privacy-preserving digital wallet technology:

1. **Interoperability**: ESSI Studio implements multiple open standards (OID4VCI, OID4VP, DIDComm, OpenBadges 3.0, ISO 18013-5) enabling interoperability across different wallet ecosystems. It is designed to work with OWF wallets like Bifold.

2. **Built on OWF Projects**: ESSI Studio is built on top of Credo-ts (formerly Aries Framework JavaScript), an OWF Growth project. It uses OWF Askar for secure wallet storage. This demonstrates the composability of OWF projects.

3. **Open Source Collaboration**: As an Apache 2.0 licensed project, ESSI Studio encourages collaboration and contributions from the broader identity community.

4. **Privacy & Security**: The platform implements privacy-preserving credential formats (AnonCreds, SD-JWT), secure key management via Askar, and post-quantum cryptography readiness.

5. **User-Centric Identity**: ESSI Studio enables organizations to issue credentials that users control in their own wallets, supporting the self-sovereign identity paradigm.

## Code of Conduct

ESSI Studio will adopt the [OpenWallet Foundation Code of Conduct](https://tac.openwallet.foundation/governance/code-of-conduct/).

## TAC Sponsor

Stephen Curran ([@swcurran](https://github.com/swcurran))

## Project License

Apache License 2.0

## Source Control

- **Current Repository**: https://github.com/ajna-inc/essi-studio

## Issue Tracker

GitHub Issues in the main repository.

## External Dependencies

### Core OWF Dependencies
| Package | License | Description |
|---------|---------|-------------|
| @credo-ts/core | Apache 2.0 | Credo-ts core framework (OWF) |
| @credo-ts/askar | Apache 2.0 | Askar wallet integration (OWF) |
| @credo-ts/openid4vc | Apache 2.0 | OID4VCI/OID4VP support (OWF) |
| @credo-ts/anoncreds | Apache 2.0 | AnonCreds support (OWF) |
| @credo-ts/tenants | Apache 2.0 | Multi-tenant support (OWF) |
| @openwallet-foundation/askar-nodejs | Apache 2.0 | Askar Node.js bindings (OWF) |

### Other Dependencies
| Package | License | Description |
|---------|---------|-------------|
| express | MIT | Web framework |
| next | MIT | React framework |
| pg | MIT | PostgreSQL client |
| redis | MIT | Redis client |
| jsonwebtoken | MIT | JWT handling |
| ethers | MIT | Ethereum utilities (for POE) |

All dependencies use OSI-approved open source licenses (Apache 2.0 or MIT).

## Release Methodology

- Semantic versioning (semver)
- GitHub Actions for CI/CD
- Docker images published to GitHub Container Registry (GHCR)
- Tagged releases with changelogs

## Initial Maintainers

| Name | GitHub | Organization |
|------|--------|--------------|
| Vinay Singh | [@vinaysingh8866](https://github.com/vinaysingh8866) | Ajna Inc. |

## Proposed Project Governance

### Contribution Process
- All contributions require DCO sign-off
- Pull requests reviewed by at least one maintainer
- CI checks must pass before merge

### Maintainer Selection
- Active contributors may be nominated as maintainers
- Existing maintainers vote on new maintainer additions
- Maintainers should represent diverse organizations (goal)


## Related OWF Projects

ESSI Studio has strong relationships with existing OWF projects:

| Project | Relationship |
|---------|--------------|
| **Credo-ts** | Core dependency - ESSI Studio is built on Credo-ts |
| **Askar** | Wallet storage backend |
| **Bifold Wallet** | Compatible wallet for credential holders |
| **ACA-Py** | Complementary server-side agent (Python vs TypeScript) |
| **SD-JWT** | Credential format support |

## Differentiation

ESSI Studio differentiates from existing OWF projects:

1. **Complete Platform vs Framework**: While Credo-ts is a framework, ESSI Studio is a complete, deployable application with UI
2. **Visual Credential Designer**: Unique drag-and-drop credential card designer
3. **Multi-Protocol Support**: Single platform supporting DIDComm, OID4VCI/VP, OpenBadges, and mDL
4. **Enterprise Focus**: Built for organizational deployment with multi-tenancy
5. **Workflow Engine**: Configurable credential issuance workflows