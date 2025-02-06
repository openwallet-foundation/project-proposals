# Project Name

OID4VC TypeScript

# Preferred Maturity Level

Labs

# Project Description

The OpenID for Verifiable Credentials set of standards provide integration of existing OpenID and OAuth2 standards with verifiable credentials.

OID4VC TypeScript is a generic, and low-level implementation of specifications. Currently it provides APIs for Issuers, Wallets, Clients, Authorization Servers and Resource Providers, covering OpenID for Verifiable Credential Issuance, and OAuth2. In addition, it supports a wide range of other OAuth2 related specifications for interoperability and security (such as Pushed Authorization Requests, Demonstrating Proof of Possesion, and PKCE).

Having experience with integration of these standards into another OWF project, Credo, we were able to create a lower-level reusable library that handles the complex parts of the specification, while still allowing full control over the full flow.

In the coming months this project will be extended with support for OpenID for Verifiable Presentations and related specifications.

The goal of this library is to stay as agnostic as possible to the credential formats being used. This keeps the dependencies minimal, while also making it less opinionated. Dependent libraries or frameworks (such as Credo) can provide the needed credential formats, crypto suites, and persistence.

The library was created by Animo as part of the SPRIN-D Funke wallet competition.

# Alignment with the OpenWallet Foundation Mission

The OID4VC TypeScript library provides a reusable library that is crucial to wallet interoperability. It is implementing the standards that are being adopted as part of the EU Digital Identity Wallet, as well as other regions in the world (such as California's drivers license project which also supports OID4VC).

The library is already being used by Credo, which is part of the reason why we think it's important this library is also contributed to OWF rather than managed by Animo.

# Code of Conduct

Will adopt OWF code of conduct.

# TAC Sponsor

Stephen Curran

# Project License

Apache 2.0

# Source Control

Project already exists on Github: https://github.com/animo/oid4vc-ts. Slug should become oid4vc-ts once transferred.

# Issue Tracker

https://github.com/animo/oid4vc-ts/issues?q=sort%3Aupdated-desc+is%3Aissue+is%3Aopen

# External Dependencies

- [Valibot](https://github.com/fabian-hiller/valibot) - MIT
- [Buffer](https://github.com/feross/buffer) - MIT

# Release Methodology

Packages are relased on NPM, OWF will be added as owner on NPM:

- https://www.npmjs.com/package/@animo-id/oid4vci
- https://www.npmjs.com/package/@animo-id/oauth2
- https://www.npmjs.com/package/@animo-id/oauth2-utils

The scope (`@animo-id/`) should be changed. As `@oid4vc` is taken we have reserved the `@openid4vc` scope on NPM.

We use changesets to write changelog entries, and a bot will create a pull request for new releases. Once the PR is merged a new release will be created automatically. We have used this method extensively and it automates 99% of the process, and works well with keeping restrictions of bots pushing to main (you can use the normal PR approval and merge process to trigger releases). Example: https://github.com/animo/oid4vc-ts/pull/8

# Initial Maintainers

- Timo Glastra - [@TimoGlastra](https://github.com/TimoGlastra) - Creator of the library, maintainer of Credo (that leverages this project)
- Martin Auer - [@auer-martin](https://github.com/auer-martin) - maintainer of Credo, experienced with OpenID4VC standards
- Berend Sliedrecht - [@berendsliedrecht](https://github.com/berendsliedrecht) - maintainer of Credo
- Alexis Delamare Deboutteville [@marsouin](https://github.com/marsouin) - verifiables.com

# Proposed Project Governance

The projects will mostly be managed by the existing Credo maintainers. Large decisions will be initially discussed as part of the Credo working group calls, but we would still like a dedicated discord channel. Later if desired by the community, the project can be more separated from the Credo project.

The design of the project is mostly led by Timo Glastra, who created this library for Animo as part of the SPRIN-D Funke wallet competition. Timo Glastra will also mostly take on general maintenance and releases of the library. Alexis Delamare Deboutteville has indicated he and his company are also interested in contributing and taking on a maintainer role for the project. Although Martin and Timo are both associated with Animo, Martin should be seen as independent maintainer of this library, not associated with Animo.

# Financial Sponsorship

The development of this library was funded by Animo, which in turn received funding through the SPRIN-D Funke wallet competition.

# Infrastructure

- Github repo
- Discord channel
- Github actions
- NPM
