# Project Name

OpenID Federation TypeScript

# Preferred Maturity Level

Labs

# Project Description

Trust is still a complex and relatively unsolved topic in the decentralized identity, EU Identity Wallet and digital credential ecosystems.

OpenID Federation defines basic components used to build multilateral federations for building trust infrastructure.

OpenID Federation TypeScript is a generic, and low-level implementation of the OpenID Federation specification, with a focus on [OpenID Federation Wallet Architecture](https://openid.net/specs/openid-federation-wallet-1_0.html). Currently it provides APIs for creating and resolving of entity configuration and statements. In the coming months support will be added for metadata policies and trust marks.

The goal of this library is to provide minimal and reusable primitives for building a federation client or server. This keeps the dependencies minimal, while also making it less opinionated. Dependent libraries or frameworks (such as Credo) can provide the needed hosting of endpoints, signing callbacks, and persistence.

The library was created by Animo as part of the SPRIN-D Funke wallet competition.

# Alignment with the OpenWallet Foundation Mission

The OpenID Federation library provides a reusable library that is crucial building trust ecosystems for wallets.

The library is already being integrated into Credo, which is part of the reason why we think it's important this library is also contributed to OWF rather than managed by Animo.

# Code of Conduct

Will adopt OWF code of conduct.

# TAC Sponsor

- TDB

# Project License

Apache 2.0

# Source Control

Project already exists on Github: https://github.com/animo/openid-federation-ts. Slug should become openid-federation-ts once transferred.

# Issue Tracker

https://github.com/animo/openid-federation-ts/issues?q=sort%3Aupdated-desc+is%3Aissue+is%3Aopen

# External Dependencies

- [Zod](https://github.com/colinhacks/zod) - MIT
- [Buffer](https://github.com/feross/buffer) - MIT

# Release Methodology

Packages are relased on NPM, OWF will be added as owner on NPM:

- http://npmjs.com/package/@openid-federation/core

The library will be updated to changesets to write changelog entries, and a bot will create a pull request for new releases. Once the PR is merged a new release will be created automatically. We have used this method extensively and it automates 99% of the process, and works well with keeping restrictions of bots pushing to main (you can use the normal PR approval and merge process to trigger releases). Example: https://github.com/animo/oid4vc-ts/pull/8

# Initial Maintainers

- Berend Sliedrecht - [@berendsliedrecht](https://github.com/berendsliedrecht) - initial creator and current maintainer of the library, maintainer of Credo
- Tom Lanser - [@tommylans](https://github.com/tommylans) - current maintainer of the library
- Timo Glastra - [@TimoGlastra](https://github.com/TimoGlastra) - maintainer of Credo (that leverages this project)

# Proposed Project Governance

The projects will mostly be managed by the existing Credo maintainers. Large decisions will be initially discussed as part of the Credo working group calls, but we would still like a dedicated discord channel. Later if desired by the community, the project can be more separated from the Credo project.

The design of the project is mostly led by Berend Sliedrecht and Tom Lanser, who created this library for Animo as part of the SPRIN-D Funke wallet competition. Timo Glastra and Berend Sliedrecht will moslty take on general maintenance and releases of the library.

# Financial Sponsorship

The development of this library was funded by Animo, which in turn received funding through the SPRIN-D Funke wallet competition.

# Infrastructure

- Github repo
- Discord channel
- Github actions
- NPM
