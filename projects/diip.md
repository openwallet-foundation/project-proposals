# Project Name
Decentralized Identity Interop Profile (DIIP)

# Preferred Maturity Level
Growth (Specification project)

# Project Description
The Decentralized Identity Interoperability Profile (DIIP) is an open interoperability profile that defines how digital wallets, issuers, and verifiers can interoperate using decentralized identity and verifiable credential technologies. DIIP provides deployment-oriented interoperability guidance that helps implementers build interoperable solutions based on existing open standards.

DIIP was initiated to address a practical challenge observed in early real-world deployments of decentralized identity technologies: while the underlying standards provide flexibility, this flexibility led to fragmentation, isolated implementations, and lengthy implementation discussions between technology providers. As a result, many projects evolved as isolated “islands” that were difficult to interoperate with other solutions.

Interoperability profiles help address this challenge by defining a clear set of conventions, supported features, and implementation choices that ecosystem participants can rely on. By following a shared interoperability profile, implementers can focus on building solutions and real-world use cases rather than resolving technical compatibility questions. This approach helps accelerate adoption and allows organizations to benefit from emerging digital trust infrastructures without needing to navigate the full complexity of the underlying specifications.
While standards such as the W3C Verifiable Credentials Data Model and the OpenID for Verifiable Credentials (OID4VC) family of specifications provide the foundational building blocks, real-world deployments often face interoperability challenges due to different implementation choices and optional features. DIIP addresses this by providing an interoperability profile, implementation guidance, and testing scenarios that help wallet providers, issuers, and verifiers build interoperable solutions. DIIP does not define new core standards but profiles and builds upon existing open standards.

The project was initiated in 2022 by the Dutch Blockchain Coalition (DBC) in collaboration with TNO, Sphereon, and Animo Solutions. Since August 2024 DIIP has been facilitated by FIDES Labs. DIIP has evolved as a community-driven interoperability profile, developed through open collaboration with implementers and ecosystem participants from multiple countries and sectors. Over the past years the profile has been applied in interoperability experiments, plugfests, and early implementations across a variety of use cases.

The DIIP community already includes implementers and ecosystem participants from a growing number of countries, including the Netherlands, Finland, Belgium, France, Germany, Spain, Italy, Greece, Switzerland, Canada, India, Japan, Taiwan, and South Korea, reflecting the growing global interest in interoperable digital wallet and verifiable credential ecosystems. Alongside its technical development, DIIP has fostered an active and growing community of implementers and ecosystem participants. The community meets regularly to discuss interoperability challenges, share implementation experiences, and guide the evolution of the profile. To date, more than 30 community meetups have been organized, creating a collaborative environment for implementers working with decentralized identity technologies.

From the beginning, DIIP has followed a pragmatic and iterative development approach. The profile evolves approximately every six months in response to the maturity of the underlying specifications and lessons learned from implementations. Early versions of DIIP were intentionally not designed to be complete or perfect, but to provide a practical and useful starting point for implementers. This approach allowed a growing group of ecosystem participants to experiment, test interoperability, and deploy early solutions while the underlying standards continued to evolve.

DIIP exists alongside other interoperability profiles in the decentralized identity ecosystem, such as the Aries Interop Profile (AIP). AIP focuses on interoperability between Aries-based agent frameworks using DIDComm, while DIIP focuses on interoperability between wallet ecosystems implementing the OpenID for Verifiable Credentials (OID4VC)family of protocols. The DIIP profile is also complementary to the OpenID4VC High Assurance Interoperability Profile (HAIP), which focuses primarily on person identification data within the EUDI Wallet ecosystem. Both profiles build on the OID4VC specifications but address different use cases and architectural approaches.
HAIP primarily focuses on high-assurance personal identity scenarios. DIIP, in contrast, combines OID4VC protocols with W3C Decentralized Identifiers (DIDs) and the Verifiable Credentials Data Model 2.0 (VCDM 2.0). This combination enables Linked Data–based credential interoperability and supports broader cross-ecosystem scenarios beyond person identification.

This makes DIIP applicable to a wide range of credential ecosystems. In particular, it can play an important role in organizational and machine-to-machine scenarios, where verifiable credentials are used by organizations, devices, software agents, or emerging AI agents, rather than individuals. As a result, DIIP is relevant for ecosystems and initiatives such as Gaia-X and Catena-X (data spaces), MOSIP, the United Nations Transparency Protocol (UNTP), CIRPASS-2 (Digital Product Passports), Digital Twins, and Open Badges.

Unlike many projects within the OpenWallet Foundation, DIIP does not focus on developing core software components. Instead, the project focuses on defining an interoperability profile, implementation guidance, and testing scenarios that help wallet implementations interoperate. In this way, DIIP complements open source wallet implementations by providing practical interoperability guidance that can be adopted by different projects and technology stacks.
DIIP builds on standards developed by multiple standards organizations, including W3C, the Decentralized Identity Foundation (DIF), and the OpenID Foundation (OIDF). Because DIIP connects technologies from multiple standards ecosystems while supporting interoperability across implementations, the OpenWallet Foundation (OWF) is considered a natural and neutral home for the project.

Bringing DIIP under the OpenWallet Foundation will support the next stage of the project’s evolution. OWF governance and infrastructure will help increase the maturity, sustainability, and global reach of the project. It will also reduce reliance on a limited number of individuals and allow the project to benefit from established open-source processes, tooling, and community governance. Maintaining the existing collaborative community dynamic remains an important objective. By bringing DIIP under the OpenWallet Foundation, the project aims to expand participation from a broader international community, including wallet providers, governments, standards organizations, and technology implementers.

As the ecosystem evolves, future DIIP releases will incorporate additional interoperability mechanisms and technologies as relevant specifications mature. Examples include emerging DID methods such as DID:webvh and DID:CEL, as well as trust mechanisms such as OpenID Federation.
By bringing DIIP under the OpenWallet Foundation, the project aims to further strengthen interoperability across decentralized identity ecosystems and support the development of secure, interoperable digital wallet infrastructures worldwide.

# Alignment with the OpenWallet Foundation Mission
DIIP aligns with the OpenWallet Foundation mission by enabling practical interoperability between wallet implementations through open standards and shared interoperability profiles.

# Code of Conduct
DIIP will adopt the OpenWallet Foundation code of conduct

# TAC Sponsor
Stephen Curran

# Project License
Apache 2.0

# Source Control
DIIP is currently using a Github repo from FIDES Community. This will be migrated to a OWF Github.

https://fidescommunity.github.io/DIIP/

https://github.com/FIDEScommunity/DIIP

# Issue Tracker
DIIP is currently using a Github repo from FIDES Community. This will be migrated to a OWF Github.
https://github.com/FIDEScommunity/DIIP/issues

# External Dependencies
Use of the spec-up package that renders the Markdown document into HTML.

# Release Methodology
The profile evolves approximately every six months in response to the maturity of underlying specifications and lessons learned from implementations. Updates and new releases are approved by majority vote within the project governance process.

# Initial Maintainers
Editors:
Eelco Klaver (Credenco) - 
Harmen van der Kooij (FIDES Labs)
Niels Klomp (Sphereon)
Niels van Dijk (SURF)
Samuel Rinnetmäki (Findynet)
Timo Glastra (Animo Solutions)

Contributors and previous editors:
Adam Eunson (Auvo)
Jelle Millenaar (Impierce Technologies)
Maaike van Leuken (TNO)
Thierry Thevenet (Talao)

# Proposed Project Governance
Harmen van der Kooij (FIDES Labs) and Samuel Rinnetmäki (Findynet) will chair the monthly project meetings on an alternating basis and act as neutral coordinators, representing the community rather than any specific wallet provider. Decisions are discussed within the community and formalized through GitHub. As the project grows, additional working groups and coordinators may be introduced.

# Financial Sponsorship
None

# Infrastructure
Marketing
Zoom & meeting calendar
Github repo
Discord channel
Mailing list


