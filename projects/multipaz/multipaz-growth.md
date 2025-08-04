# Project Name
Multipaz

# Preferred Maturity Level
Growth

# Project Description
Multipaz is an Open Wallet Foundation (OWF) project that originated at Google and is a multiplatform Digital Credential SDK for usage by anyone. It is not a product of Google itself, such as Google Wallet or Google Pay, but rather an open-source initiative.

What it is and what it does: Multipaz provides a complete and comprehensive set of digital identity resources, including libraries, frameworks, and mobile reference applications, which are made freely available for anyone to use. Its core functionalities include:

*   Issuance/provisioning, storage, presentment, and verification of credentials.
*   Support for various credential formats such as ISO mdoc and IETF SD-JWT VC.
*   Implementation of presentation protocols like OpenID4VP and W3C Digital Credentials API, as well as ISO/IEC 18013-5 proximity presentation.
*   Development of multiplatform libraries for Android and iOS, with plans for WearOS/WatchOS companion apps. This involves sharing 99% of the code between Android and iOS versions, with only low-level Bluetooth stack implemented differently.
*   Offers capabilities such as a cloud secure area reference implementation, dual issuance for credentials, and a Zero Knowledge Proof (ZKP) prototype. It also supports mDoc direct access, enabling access to IDs when the device is off.

Why it is valuable: The mission of Multipaz is to build useful resources that move the digital credential ecosystem forward in a private, secure, and scalable way. It addresses key problems in digital identity, including interoperability, security & privacy, and the multitude of choices in the ecosystem.

*   By offering an all-encompassing SDK, Multipaz significantly lowers the barrier to entry for private and public entities looking to build their own digital identity solutions or integrate with existing ones. This is especially valuable for countries without a clear path forward for digitizing national IDs.
*   Multipaz aims to drive down certification costs for the entire digital identity ecosystem by making its code open-source and widely used for testing. Its open-source nature allows many others to use internal forks or test against Multipaz implementations as a sanity check.
*   The project also provides direction and input into ongoing standardization initiatives by actively contributing to ISO (e.g., ISO/IEC 18013-5), OpenID Foundation, and W3C working groups.

Origin and History: The project originated at Google, with Google joining ISO/IEC JTC1 SC17 WG10 in 2018 and beginning contributions that led to ISO/IEC 18013-5:2021. Work on the Identity Credential API for Android and mDL Reference Applications began in 2019. In 2023, the project was contributed to the Open Wallet Foundation (OWF) to make the resources available to a broader audience beyond Google. Key milestones include:

*   2021: ISO/IEC 18013-5:2021 published.
*   2022: DMVs in the US start issuing mDLs; Google Wallet adds mDL support in beta using the Multipaz library.
*   2023: First Maven release; contribution to OWF; SecureArea work begins.
*   2024: W3C Digital Credentials API support added; porting to Kotlin Multiplatform starts; IETF SD-JWT VC support added; OpenID4VP and OpenID4VCI support added.
*   2025: Project officially renamed to Multipaz; interoperability testing in Utrecht and with OpenID Foundation; Multipaz 0.90.0 released with initial iOS support.

What the project will include (scope and deliverables): Multipaz aims to provide everything needed to build multi-platform apps, issuance servers, and verification services. Deliverables include:

*   An externally accessible GitHub repository with multiplatform libraries and samples.
*   Fully featured issuer code with "issuer integration-in-a-box".
*   Production-level applications, specifically an Identity Wallet app for phones (Android, iOS, and potentially Harmony.NEXT) and watches (WearOS, WatchOS), and an Identity Reader app for phones (Android, iOS).
*   The "Utopia universe," which consists of fictional credential issuers and relying parties (e.g., DMV of Utopia, Brewery of Utopia) to demonstrate use-case scenarios like purchasing movie tickets or buying a beer, and to serve as a test bench for Wallet and ID app developers.
*   Regular releases of the Multipaz SDK, with version 1.0 planning to freeze API, data formats, and internal protocols.
*   Regular marketing, blogposts, and technical documentation.

The project aims to be a robust and user-friendly tool for relying parties to read various digital credentials like mDLs, Photo ID, and much more, addressing the current lack of suitable everyday readers in the ecosystem.

# Alignment with the OpenWallet Foundation Mission
Multipaz’s mission is inherently aligned with the goals of the OWF for the following reasons:

*   Open-Source Availability: Multipaz’s goal is to provide a complete and comprehensive set of digital identity resources, including libraries, frameworks, and mobile reference applications, free to anyone who wants to use them.
*   Addressing Ecosystem Challenges: Multipaz directly tackles key problems in digital identity, such as interoperability, security & privacy, and the multitude of choices in the ecosystem. By offering an all-encompassing SDK, it significantly lowers the barrier to entry for private and public entities to build or integrate their own digital identity solutions, especially benefiting countries without a clear path for digitizing national IDs.
*   Standardization and Interoperability: The project actively provides direction and input into ongoing standardization initiatives, contributing to working groups like ISO (e.g., ISO/IEC 18013-5), OpenID Foundation (e.g., OpenID4VP, OpenID4VCI), and W3C (for W3C Digital Credentials API). This commitment ensures that the digital credential ecosystem develops on common shared protocols and libraries, fostering interoperability among different wallets and systems.
*   Community and Adoption: Multipaz's open-source nature allows it to be widely used as a test bench by virtually everyone in the ecosystem, which helps to drive down certification costs and improve the overall quality of digital identity implementations. Its success is tied to its availability for all, encouraging widespread adoption.
*   Non-Proprietary Focus: Multipaz operates as a product-independent initiative at Google for the benefit of the open source community, with all decisions run by the OWF. This fosters a neutral, collaborative environment for digital identity advancement.

# Code of Conduct
https://github.com/openwallet-foundation-labs/identity-credential?tab=coc-ov-file

# TAC Sponsor
N/A

# Project License
https://github.com/openwallet-foundation-labs/identity-credential?tab=Apache-2.0-1-ov-file

# Source Control
https://github.com/openwallet-foundation-labs/identity-credential

# Issue Tracker
https://github.com/orgs/openwallet-foundation-labs/projects/7/views/1

# External Dependencies
N/A

# Release Methodology
Monthly or every 2 months.

# Initial Maintainers
David Zeuthen, Troy Kensinger

# Proposed Project Governance
David Zeuthen (Technical Lead) and Troy Kensinger (Technical Program Manager) maintain an ongoing roadmap that is reviewed regularly with Multipaz stakeholders. As priorities are set, the roadmap and release schedule is updated to align with ecosystem needs.

# Financial Sponsorship
OWF, Google

# Infrastructure
Continued domain hosting and tooling resources. Marketing and social media help would be great. Security audits where possible.