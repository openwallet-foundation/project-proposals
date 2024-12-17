# Project Name

DCQL TypeScript

# Preferred Maturity Level

Labs

# Project Description

The Digital Credentials Query Language (DCQL, pronounced [ˈdakl̩]) is a JSON-encoded query language that allows a verifier to request verifiable presentations that match a query.

DCQL TypeScript is a generic, and low-level implementation of the query language. By providing it as a separate library from OpenID4VC we hope to see adoption of the library outside of the OpenID4VC set of standards (Credo is intending to adopt it for DIDComm protocols as replacement for DIF Presentation Exchange as well).

The library was created by Animo as part of the SPRIN-D Funke wallet competition, to experiment with the new query language added to the OpenID4VP specification.

# Alignment with the OpenWallet Foundation Mission

The DCQL library provides a reusable library that is crucial to wallet interoperability. It is already being adopted by Credo, as well as being integrated in [Sphereon OID4VC](https://github.com/Sphereon-Opensource/OID4VC/pull/171), which is used a lot for TypeScript/JavaScript projects integrating verifiable credentials.

# Code of Conduct

Will adopt OWF code of conduct.

# TAC Sponsor

- TDB

# Project License

Apache 2.0

# Source Control

Project already exists on Github: https://github.com/auer-martin/dcql. Slug should become dcql-ts once transferred.

# Issue Tracker

https://github.com/auer-martin/dcql/issues?q=sort%3Aupdated-desc+is%3Aissue+is%3Aopen

There are some issues related to aligning the project better with other projects we maintain at OWF and adding the needed license.

# External Dependencies

- [Valibot](https://github.com/fabian-hiller/valibot) - MIT

# Release Methodology

Package is relased on NPM, OWF will be added as owner on NPM: http://npmjs.com/package/dcql

We use changesets to write changelog entries, and a bot will create a pull request for new releases. Once the PR is merged a new release will be created automatically. We have used this method extensively and it automates 99% of the process, and works well with keeping restrictions of bots pushing to main (you can use the normal PR approval and merge process to trigger releases). Example: https://github.com/auer-martin/dcql/pull/21

# Initial Maintainers

- Martin Auer - [@auer-martin](https://github.com/auer-martin) - Creator of the library, maintainer of Credo, contractor for Animo
- Timo Glastra - [@TimoGlastra](https://github.com/TimoGlastra) - maintainer of Credo (that leverages this project)

# Proposed Project Governance

The projects will mostly be managed by the existing Credo maintainers. Large decisions will be initially discussed as part of the Credo working group calls, but we would still like a dedicated discord channel. Later if desired by the community, the project can be more separated from the Credo project.

The design of the project is mostly led by Martin Auer, who created this library for Animo as part of the SPRIN-D Funke wallet competition. Timo Glastra will mostly assist with the general maintenance and releases of the library. Although Martin and Timo are both associated with Animo, Martin should be seen as indepdant mainainer of this library, not associated with Animo.

# Financial Sponsorship

The development of this library was funded by Animo, which in turn received funding through the SPRIN-D Funke wallet competition.

# Infrastructure

- Github repo
- Discord channel
- Github actions
- NPM
