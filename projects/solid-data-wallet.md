# Project Name

Solid Data Wallet

Proposed repository name `solid-data-wallet`.

[Solid is an open standard for structuring data, digital identities, and applications on the Web](https://solidproject.org/about). The Solid standards are developed at W3C by the [Solid Community Group](https://www.w3.org/community/solid/). The Solid Project is a community of volunteers formed by Tim Berners-Lee to complement the standardization efforts at W3C, such as publishing [technical reports](https://solidproject.org/TR/), manage [github repositories](https://github.com/solid), a forum, events calendar, and so forth. It is however not an incorporated legal entity. As such the Solid term is not trademarked by the solid project, nor are we aware of any attempts of any entity to register the Solid trademark (in this context).

The `solid-` prefix for the project is intended to be descriptive of the intention behind and the functionality of the wallet project; it reflects the project roots, it is not a brand.

The project is currently open source and hosted on [github](https://github.com/inrupt/inrupt-data-wallet) by Inrupt. 


# Preferred Maturity Level

The project is based on production ready technologies with significant adoption. Due to the wallet project being in early stage though, we would suggest it being adopted by [Labs](https://tac.openwallet.foundation/governance/project-lifecycle/#labs).

# Project Description

The proposed project is a [React Native](https://reactnative.dev/) and [Expo](https://expo.dev/) based mobile data wallet implementation.

The project was initially developed by [Inrupt](https://www.inrupt.com/solutions/data-wallet), part of an effort to build a [Solid](https://solidproject.org/) backed wallet infrastructure so that *"organizations deliver innovative apps, products, and experiences \[...] powered by flexible, secure, and user-centric data sharing"*.

The timing is also important, as Solid moved to the final stage of standardization at W3C, with the creation of the [Linked Web Storage](https://www.w3.org/groups/wg/lws/) workgroup. In addition to that, Inrupt decided to open source the wallet technology and make it available to a larger audience.

# Alignment with the OpenWallet Foundation Mission
[OpenWallet Foundation mission](https://tac.openwallet.foundation/governance/charter/) emphasizes three core elements:
* *"develop and maintain open source code for wallets to enable and ensure wallet interoperability,"* - The project is very well aligned with this principle and, arguably, goes a step further in that it promotes a larger scoped data interoperability, via the Solid set of specifications. The wallet code proposed is, as expected, open sourced under the permissive ALv2 license.
* *"advocate for the adoption of the interoperable digital wallet technology, \[...]"* - Inrupt, the company that originally developed the wallet is already strongly advocating for data interoperability. The Solid specs where initially imagined by Inrupt's CTO, Sir Tim Berners-Lee with the intent of extending *"the web to include identity management, access control and universal standards for data. These capabilities decouple data from applications so that data is organized around individuals."*
* *"collaborate with Standards Development Organizations (SDOs) in the development and proliferation of open standards related to digital wallets"* - Inrupt will continue to be active in the definition of standards at W3C, as well as development and promotion of the wallet technologies backed by Solid and related specs, such as DID, verifiable credentials, and others.

# Code of Conduct

[OpenWallet Foundation code of conduct](https://tac.openwallet.foundation/governance/code-of-conduct/).

# TAC Sponsor
TBD

# Project License
[ALv2](https://www.apache.org/licenses/LICENSE-2.0) - SPDX:Apache-2.0

# Source Control

The project is currently open source and hosted on [github](https://github.com/inrupt/inrupt-data-wallet) by Inrupt.

# Issue Tracker

[OpenWallet Foundation Labs](https://github.com/openwallet-foundation-labs)

# External Dependencies

React Native Typescript project. Code dependencies explicitly defined in the project.

There is a dependency on Solid based storage for data. There are a few open source and commercial [implementations of Solid](https://solidproject.org/for-developers#hosted-pod-services) servers available. Inrupt also provides a [Solid hosting service](https://start.ap.inrupt.com/profile) free for non-commercial purposes.

# Release Methodology

The project builds cross-platform mobile application wallets for both iOS and Android. Maintainers will issue official releases at regular times, but there is no intent (both from Inrupt and the project) to release the apps on the Play or App Store(s). The project is white-labeled so that adopters could add their branding and enhancements as desired before publishing to app stores.

# Initial Maintainers

* [Kyra Assaad](https://github.com/KyraAssaad)
* [Pete Edwards](https://github.com/edwardsph)
* [Seila Gonzales-Estrecha](https://github.com/seilagonzalez)
* [Nicolas Seydoux](https://github.com/NSeydoux)
* [Hadrian Zbarcea](https://github.com/hzbarcea)

# Proposed Project Governance

Everyone is encouraged to contribute to the project. Contributors will be able to open issues via Github, submit patches and discuss their ideas. We encourage everyone interested in adopting the technology to share use-cases and requirements.

# Financial Sponsorship

* [Inrupt](https://www.inrupt.com/about)

# Infrastructure

Inrupt already provides the required project infrastructure. That said, we aim to align with processes used by other OWF projects and use available
[services for labs](https://tac.openwallet.foundation/governance/project-and-lab-services/) as much as possible without adding a significant burden to the OWF staff.

