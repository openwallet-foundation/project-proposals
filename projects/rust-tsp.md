# Project Name
The project is currently known as "rust-tsp". 

We may or may not change this name to something that does not directly reference "Rust" because although the core is implemented in Rust, we expect additional language bindings in the project.

# Preferred Maturity Level
Lab

# Project Description
This project is an early impementation of the draft Trust Spanning Protocol (TSP): https://github.com/trustoverip/tswg-tsp-specification.

According to the above referenced specification, "The Trust Spanning Protocol (TSP) facilitates secure communication between endpoints with potentially different identifier types, using message-based exchanges. As long as these endpoints use identifiers based on public key cryptography (PKC) with a verifiable trust root, TSP ensures their messages are authentic and, if optionally chosen, confidential. Moreover, it presents various privacy protection measures against metadata-based correlation exploitations. These attributes of TSP together allow endpoints to form authentic relationships rooted in their respective verifiable identifiers (VIDs), viewing TSP messages as virtual channels for trustworthy communication.
".

A shorter introduction of TSP can be found in this blog post: https://www.trustoverip.org/blog/2023/08/31/mid-year-progress-report-on-the-toip-trust-spanning-protocol/

This project's current code includes a Rust implementation of all TSP features. We also plan to incorporate/develop related features such as additional Verifiable Identifier types, additional transport layer mechanisms, different language bindings as needed and integration modules needed to be compatible with other OpenWallet projects.
In addition, we may add and welcome trust task or application specific extensions.

# Alignment with the OpenWallet Foundation Mission
TSP's core features provide a foundation for interoperability of different trust basis mechanisms and ensuring a very strong sense of authenticity, confidentiality and optionally meta-privacy.
These features are critical to open, secure, and safe wallets, decentralization of various system components, interoperability between domains (e.g. different technical approaches, different countries or regulatory or industry ecosystems) and communication or sharing of data between endpoints empowered by modern open wallets. The TSP specification is being developed by the Trust over IP Foundation, a sister organization also under the Linux Foundation. This project will be a collaboration with the standard spec work in ToIP.

# Code of Conduct
We will adopt the [OpenWallet Foundation code of conduct](https://tac.openwallet.foundation/governance/code-of-conduct/).

# TAC Sponsor
- Wenjing Chu (myself), and
- Tracy Kuhrt
- Mike Varley

# Project License
Current code is Apache 2.0.

# Source Control
It's in a GitHub repo that can be moved to OpenWallet: https://github.com/wenjing/rust-tsp.

# Issue Tracker
We use GitHub issue tracker open to all:https://github.com/wenjing/rust-tsp/issues.

# External Dependencies
_If there are any external dependencies, please list those here including licenses._

# Release Methodology
This is an early implementation in progress. There is not currently a release methodology, so we will answer with "N/A (not applicable)".

# Initial Maintainers
- Marlon Baeten: @marlonbaeten
- Marc Schoolderman: @squell
- Wenjing Chu: @wenjing
- Additional maintainers are expected in the near future

# Proposed Project Governance
We have yet to adopt any process but can work with contributors and OpenWallet community to adopt one.

# Links to Documented Governance Practices
_Include a link to the project charter. The project charter can be obtained by completing the [project intake form](https://docs.google.com/forms/d/e/1FAIpQLSeO1bDGHUP-ZpCo1uynm94YOxZlek6RhCH7o3FnX1lZSXXfSQ/viewform?fbzx=4351560609072672295)._

The LF Intake form completed/submitted.

# Financial Sponsorship
The project is currently sponsored by Futurewei Technologies Inc. but we do not expect financial sponsorship in the future as an OpenWallet Foundation project.

# Infrastructure
Within the [services for projects and labs](https://tac.openwallet.foundation/governance/project-and-lab-services/), we request 
- GitHub repo (move to OWF repo)
- OWF Discord chat
- OWF mailing list (for people who have difficulties in accessing Discord readily)
- Paid tooling: e.g. GitHub based build tools/actions

To properly test TSP in various modes, we wish to request if OWF can support testing infrastructure (to be discussed).
