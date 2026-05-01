# Project Name
Health Wallet

# Preferred Maturity Level
Labs stage

# Project Description

Health Wallet is a blockchain-powered healthcare information solution designed to empower patients with full control over their medical data. The platform enables secure sharing of medical records, imaging data, and patient information using decentralized web3 technologies.

## What Health Wallet Does

Health Wallet addresses critical challenges in healthcare information exchange by providing:

1. **Decentralized Medical Record Management**: Patients store their health records on IPFS with references and access controls maintained via smart contracts, creating a secure, immutable record system outside traditional centralized databases.

2. **Patient-Controlled Data Sharing**: Through an intuitive interface, patients can grant temporary, specific access to their medical records to healthcare providers using smart contracts that enforce access rules without requiring central authority verification.

3. **Integrated Imaging Hub**: The platform seamlessly integrates medical imaging data (DICOM format) with textual records, providing a unified view of patient information with advanced filtering capabilities.

## Project Value and Impact

Health Wallet transforms healthcare data management by:

- **Increasing Patient Autonomy**: Shifting control from institutions to individuals, allowing patients to determine who sees their data and how it gets used.
- **Reducing Data Silos**: Creating interoperability between previously disconnected healthcare systems.
- **Enhancing Security**: Leveraging blockchain's immutable ledger to create tamper-proof medical records.

## Origin

This project was started to address a key issue in radiology when patients are provided care from a clinic or hospital and they don't have access to their own patient images afterwards. Sometimes they can access via proprietary systems or handed a CD-ROM but the system isn't designed to make it easier on patients.

## Technical Architecture

The Health Wallet system employs a hybrid architecture that combines traditional web technologies with blockchain components:

```
┌────────────────────────┐     ┌────────────────────────┐
│    User Interfaces     │     │   Blockchain Layer     │
│  ┌──────────────────┐  │     │  ┌─────────────────┐   │
│  │ Patient Portal   │  │     │  │ Smart Contracts │   │
│  └──────────────────┘  │     │  │  - AccessControl│   │
│  ┌──────────────────┐  │     │  └─────────────────┘   │
│  │ Provider Portal  │  │     │  ┌─────────────────┐   │
│  └──────────────────┘  │     │  │ Ethereum Network│   │
└──────────┬─────────────┘     │  └─────────────────┘   │
           │                   └──────────┬─────────────┘
┌──────────▼─────────────┐              │
│    Application Layer   │     ┌─────────▼─────────────┐
│  ┌──────────────────┐  │     │   Storage Layer       │
│  │ Next.js Frontend │  │     │  ┌─────────────────┐  │
│  └──────────────────┘  │     │  │ IPFS Network    │  │
│  ┌──────────────────┐  │     │  │ (Encrypted Data)│  │
│  │ API Routes       │  │     │  └─────────────────┘  │
│  └──────────────────┘  │     │  ┌─────────────────┐  │
└──────────┬─────────────┘     │  │ Traditional DB  │  │
           │                   │  │ (Metadata)      │  │
┌──────────▼─────────────┐     │  └─────────────────┘  │
│    Data Models         │     └─────────────────────────┘
│  ┌──────────────────┐  │
│  │ User/Patient     │◄─┐
│  └──────────────────┘  │
│  ┌──────────────────┐  │
│  │ HealthRecord     │  │
│  └──────────────────┘  │
│  ┌──────────────────┐  │
│  │ AccessGrant      │  │
│  └──────────────────┘  │
│  ┌──────────────────┐  │
│  │ Appointment      │──┘
│  └──────────────────┘
└────────────────────────┘
```

### Key System Components:

1. **Frontend Application**: Built with Next.js providing responsive interfaces for both patients and providers.

2. **Authentication System**: Dual authentication paths - traditional username/password and Web3 authentication using MetaMask wallet signatures.

3. **Blockchain Layer**:
   - Smart contracts for managing data access permissions
   - IPFS integration for decentralized storage of encrypted medical data
   - MetaMask wallet integration for digital identity and transaction signing

4. **Database Models**:
   - User/Patient models with Ethereum address integration
   - Health records linking to IPFS content identifiers
   - Access grants mapping permissions to specific records
   - Provider view of patient records

The architecture ensures that while metadata and access controls are maintained on the blockchain, sensitive medical data is encrypted and stored on IPFS, allowing for both security and scalability. The IPFS nodes can also be hosted by a provider or health system for data privacy laws.

## Key features include:

- **Blockchain-Based Health Records**: Secure, immutable patient records stored with Ethereum and IPFS technologies
- **Patient Data Ownership**: Complete control over personal health information with granular access permissions
- **Selective Data Sharing**: Share specific medical records with authorized providers via smart contracts

# Alignment with the OpenWallet Foundation Mission
This project aligns with the OWF mission by providing an open source implementation of blockchain wallet technology for healthcare data management. 

It empowers patients with data sovereignty using open medical standards such as FHIR and DICOM, creating an interoperable solution for secure health information exchange.

# Code of Conduct
[OpenWallet Foundation code of conduct](https://tac.openwallet.foundation/governance/code-of-conduct/)

# TAC Sponsor
N/A

# Project License
Apache 2.0

# Source Control
Currently a public GitHub repository (https://github.com/sbhavani/health-wallet) under a personal account, this project will be moved under OWF organization and all existing code will be contributed.

# Issue Tracker
https://github.com/sbhavani/health-wallet/issues

# External Dependencies

## Frontend
- Next.js (MIT)
- TypeScript (MIT)
- shadcn/ui (MIT)
- Tailwind CSS (MIT)
- Web3.js (LGPL-3.0)
- NextAuth.js (ISC)

## Blockchain
- Ethereum (LGPL-3.0)
- IPFS (MIT/Apache-2.0)
- MetaMask (MIT)

## Backend
- Prisma ORM (Apache-2.0)

All dependencies are open-source with compatible licenses.

# Release Methodology
The project will follow semantic versioning with container releases published using GitHub Packages. 

The web application is responsive and works across devices. The primary deployment is as a web application with Next.js, with Progressive Web App (PWA) capabilities to enable usage on mobile devices even in underresourced environments.

# Initial Maintainers
- [Ryan Stellar](https://github.com/rstellar)
- [Santosh Bhavani](https://github.com/sbhavani)

# Proposed Project Governance
Follow TAC advice.

# Financial Sponsorship
None

# Infrastructure
The project requires:
- GitHub Repository with Issues Tracking
- Chat (i.e. Discord) channel
- OWF marketing
