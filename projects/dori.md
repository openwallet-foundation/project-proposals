# Project Name
DORI: Decentralized Online Resource for Identity

# Preferred Maturity Level
Labs

# Project Description
When talking about wallets for natural persons, a lot of people think that a smartphone based wallet is the only way to go. The user should feel the security and privacy by being independent from an external provider. But we are forgetting that online based services have a great user experience in daily live:
As a user I can use multiple clients where my data is synced, we do not have to care about backups or data recovery.
As a developer I can implement the business logic into the cloud and only need the rendering on the client side.

Yes, when I am offline, I do not have access to my data anymore. But beside that the user experience is great!

The DORI project is a typescript based monorepo, using [nx](https://nx.dev) to manage multiple components. Compared to other approaches, it also comes with an issuer and verifier service to issue and verify credentials.

## Clients
There are two clients that can be used to interact with a cloud wallet
- a PWA based on Angular
- a Chrome Browser Extension based on Angular

While the PWA is using the camera to scan QR codes, the browser extension is scanning the opened taps for QR codes and is able to show a little button next to the QR code to interact with the wallet. This approach was inspired by password managers like 1Password. In the daily use, People do not want to take out their smartphone to scan a QR code, they want an easy one click solution.

By implementing the whole business logic in the cloud, the client is only responsible for the rendering. Therefore building new clients in other programming languages is easy by using the OpenAPI endpoints. For authentication the OpenID Connect protocol is used, the project is using the [Keycloak](https://www.keycloak.org/) server for that.

## Issuer and Verifier

Both relying parties are implemented as separate services, each of them comes with a web client for demo purposes. Further integration like webhooks or other services can be implemented in the future. The authentication is done by using the OpenID Connect protocol.

## Modular approach
The usage of NX allows reusable components with a modular approach. Each backend implementation supports low security key management by storing the keys in the filesystem or the database, or the integration with Hashicorp Vault for high security key management. Other implementations are possible.

## Identity Stack
By validating existing SSI frameworks like Credo or Veramo, this project should primary focus on the architecture reference framework of the EU. Therefore other credential formats, transport protocols or key managements like multiple DIDs methods are not supported.

**Credential Profile:**
- Credential Format: SD-JWT-VC
- Key Management (issuer): VC-ISSUER Meta data, DID, X509
- Key Management (holder): CNF (json web key)
- Transport Protocol: OID4VC
- Signature Algorithm: P-256
- Status Management: OAUTH Status List

# Alignment with the OpenWallet Foundation Mission
One of the primary demands is the architecture reference framework of the EU. By following the standards, it is possible to implement the different components on different platforms, but still be able to test them in a functional environment.

It can also be used as a playground to test out new approaches: how can processes be automated for the best UX without a security tradeoff? Implementing alterative approaches like another signature algorithm and compare them with the current implementation.

# Code of Conduct
[OpenWallet Foundation code of conduct](https://tac.openwallet.foundation/governance/code-of-conduct/)

# TAC Sponsor
None

# Project License
Apache 2.0 for all projects inside the Monorepo.

# Source Control
[Github Repo](https://github.com/cre8/wallet)

# Issue Tracker
[Github Issues](https://github.com/cre8/wallet/issues)

# External Dependencies
None

# Release Methodology
Docker images will be released to the Github Registry. For versioning semantic versioning with synced version numbers should be used in the future.

# Initial Maintainers
Mirko Mollik [cre8](https://github.com/cre8)

# Proposed Project Governance
Everyone should be able to contribute to the project. As primary goal is to follow the architecture reference framework of the EU. Contributors will be able to open issues via Github or pitch their ideas in monthly calls.

# Links to Documented Governance Practices


# Financial Sponsorship
None

# Infrastructure
None right now, since the hosting of a demo instance would require to define a data policy. In case the legal part in covered, a minimal setup can be realized with with small VMs and a domain.
