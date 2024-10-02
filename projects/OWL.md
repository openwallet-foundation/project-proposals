# OWL -- Wallet Test Tools

## Project Name: OWL

In proposing to bring the current [Aries Agent Test Harness](https://aries-interop.info) to OWF, we suggest merging into it the [Mobile Agent Test Harness](https://github.com/openwallet-foundation/mobile-wallet-test-harness), currently (but not supposed to be) part of the OWF”s Bifold Wallet project. The Mobile Agent Test Harness uses Aries Agent Test Harness in some of its test cases. We also propose including in this testing project the [Aries Akrida](https://github.com/hyperledger/aries-akrida) repository, an agent load testing tool for deployments of ACA-Py and compatible agents. Akrida’s engine is based on the open source [Locust](https://locust.io/) tool, and instances (single or clustered) of OWF’s [Credo-TS](https://github.com/openwallet-foundation/credo-ts). Together, the three components provide rich testing lab for Agents and Wallets covering compatibility, interoperability, and scalability.

The OWL name is a nod to the Telecom industry's interoperability "Labs", such as at [UNH](https://www.iol.unh.edu/), where environments are created to enable vendors and product creators can bring their products to test with others. The not-an-acronym name OWL is to prevent confusion with the OpenWallet Foundation's "Labs" maturity level.

## Preferred Maturity Level

We propose that the project be at the “Growth” level.  All three of the components have been used extensively in the past and are well documented. Many groups have used the tools in testing their own instances of the various support agents and wallets.  As we move the project to OWF and start up the Wallet Interoperability Special Interest Group (link to PR to be added) these tools will be useful in enabling testing across frameworks and deployments built on those deployments. We look to expand their use in both the scope of the testing they enable, and their use by the community.

The following sub-section covers how Agent Test Harness meets OpenWallet Foundation maturity level criteria for Growth projects.

### Growth

* 2 TAC sponsors to champion the project and provide mentorship as needed.
* Development of a growth plan, to be done in conjunction with their project mentor(s) at the TAC.
* Development of a project roadmap that provides differentiated features and capabilities and the timeframe for completion.
    * Defined Roadmap Activities:
        * Short Term (3 months)
            * Credo Backchannel OOB/DIDExchange Support
            * Full Credo AIP 2.0 Support in Backchannel
            * RFC 0794 DID Rotate with Credo/ACA-Py/VCX
            * Mobile Backchannel Headless App Support
            * Migrate AATH to use fully qualified credential identifiers instead of legacy indy
            * Remote agent in any role support
        * Medium Term (6 Months)
            * Expand AnonCreds Handling and Tests
            * Large Scenario Tests (test chaining)
            * Removal of the AIP 1.0 & 2.0 classifications/handling
            * Tests for Proof requests for multiple AnonCreds w/wo revocation
            * Backchannels moved to out of AATH and into the Frameworks purview
        * Long Term (9 month to 1 year)
            * OID4VC support in AATH
            * DIDComm V2 Test Scenarios
* Document that it is being used successfully in either proof of concepts or pilots by at least two independent end users which, in the TAC’s judgment, are of adequate quality and scope.
    * [Government of British Columbia](https://digital.gov.bc.ca/digital-trust/home/)
    * [Indicio, PBC](https://indicio.tech/)
    * [GAN](https://gan.foundation/)
* Demonstrate a substantial ongoing flow of commits and merged contributions.
    * 29 [Contributors](https://github.com/hyperledger/aries-agent-test-harness/graphs/contributors) and a steady flow of contributions
    * Ongoing maintenance to both add and remove tests and components being tested.
* Demonstrate that the current level of community participation is sufficient to meet the goals outlined in the growth plan and roadmap.
    * The interoperability and load testing is inherently crucial to all users and contributors to [Credo-TS](https://credo.js.org/), [Bifold Wallet](https://github.com/openwallet-foundation/bifold-wallet), [ACA-Py](https://aca-py.org) and [Aries VCX](https://github.com/hyperledger/aries-vcx) (Aries Framework).
* Since these metrics can vary significantly depending on the type, scope and size of a project, the TAC has final judgment over the level of activity that is adequate to meet these criteria.
* Demonstrates how this project differs from existing projects in the Growth and Impact stages.

## Project Description

OWL is an extensible set of open-source testing tools designed to validate the functionality, scalability, and interoperability of wallets and other components within the decentralized trust ecosystems. A summary of its daily interoperability test runs can be published, such as on the website [https://aries-interop.info](https://aries-interop.info). The test harness components are crucial for ensuring that different decentralized trust agent implementations, which are responsible for handling decentralized identifiers (DIDs) and exchanging verifiable credentials, can interoperate seamlessly. OWL currently includes support for the OWF’s Credo-TS and Bifold projects, plus the proposed ACA-Py project and other [Hyperledger Aries](https://www.hyperledger.org/projects/aries) sub-projects.

The following are the key features of OWL supported by its different tools.

* Interoperability Testing: Agent and Mobile Test Harnesses are specifically designed to test the interoperability of wallets and agents by executing interactions between them, ensuring that agent implementations can communicate using standard protocols, exchange verifiable credentials, resolve DIDs, and perform other core functions reliably.
* Load Testing: Akrida provides a scriptable framework for generating load against a deployment of agents for messaging and exchanging credentials. This allows users of OWF technologies to apply a significant generated load on their deployment to ensure it will scale as needed, and to identify and address bottlenecks.
* Automation: Agent Test Harness automates the testing of agents, making it easier for developers to continuously verify the compliance and performance of their implementations. Developers can configure what agent implementations with whom they want to test interoperability and for each, what specific tests they want executed. Implementations can even include their CI pipelines select Agent Test Harness interoperability tests.
* Extensibility: The tools are highly extensible, allowing developers to add their implementations for testing and to construct custom tests and scenarios that suit a wide variety of use cases. This flexibility is important for testing a wide range of decentralized identity solutions across different industries.
* Comprehensive Coverage: OWL covers a wide array of functionalities that decentralized trust agents should support, including secure messaging, protocols, and credential issuance, verification and revocation across a range of credential formats.
* Community-Driven: OWL is developed and maintained by a global community of contributors to ensure that it stays up-to-date with the latest standards and best practices in the decentralized identity space.

As mentioned in the [Project Name](#project-name-owl) section, we suggest that the newest components, Agent Test Harness and Akrida, be combined into a single project with the Mobile Wallet Test Harness. All will be separate repos in the project, but share common project components (governance, meetings, Discord community, etc.).

## Alignment with the OpenWallet Foundation Mission

OWL supports the OWF’s goals by focusing on interoperability, and the promotion of open standards within the decentralized identity ecosystem. Notably, OWL’s goals in common with the OpenWallet Foundation are:

1. Interoperability: The primary purpose of the OWL Test Harnesses are to ensure interoperability between different agents/wallets by validating their ability to communicate using standard protocols like DIDComm and to handle core functions like verifiable credential exchanges. It provides a consistent testing environment to verify that components from different developers and organizations, evolving independently, can work together seamlessly.
2. Promotion of Open Standards: As an open-source toolset, OWL is built around open standards and protocols, ensuring that the agents it tests comply with widely accepted norms in the decentralized identity space. This approach encourages the adoption of these standards across the industry, fostering a more unified and interoperable ecosystem.
3. Facilitating Innovation and Adoption:  By providing developers with tools to validate their agents with those developed by others in the space, OWL lowers the barriers to entry for creating new, compliant, and interoperable decentralized identity solutions. This facilitates innovation and encourages the adoption of decentralized identity technologies.

## Code of Conduct

OWL follows the [Hyperledger Code of Conduct](https://github.com/hyperledger/aries-agent-test-harness/blob/main/CODE_OF_CONDUCT.md), which is what the OWF code of conduct is based on.

## TAC Sponsor

* Tracy Kuhrt
* Wenjing Chu

## Project License

The project has an Apache 2.0 license: [Agent Test Harness - License](https://github.com/hyperledger/aries-agent-test-harness/blob/main/LICENSE)

## Source Control

The project is hosted in GitHub and includes the following repositories:

* [Agent Test Harness](https://github.com/hyperledger/aries-agent-test-harness) — test results published to [https://aries-interop.info](https://aries-interop.info)
* [Aries Akrida](https://github.com/hyperledger/aries-akrida) — load testing engine for deployments of ACA-Py and other compatible agents.
* [Mobile Wallet Test Harness](https://github.com/openwallet-foundation/mobile-wallet-test-harness)

## Issue Tracker

Issues are tracked using GitHub's Issues feature in the corresponding repository.

## External Dependencies

The Agent Test Harness part of OWL is built in [Python](https://www.python.org/) using the [Behave](https://github.com/behave/behave) [behavior-driven development](https://en.wikipedia.org/wiki/Behavior-driven_development) (BDD) engine. The repository also contains a component per agent implementation that uses Agent Test Harness.

Test results from the periodic (thrice weekly) interoperability test runs are pushed for later analysis into an instance (operated by [Government of British Columbia](https://www2.gov.bc.ca/gov/content/home)) of the [Allure](https://allurereport.org/docs/pytestbdd/) behavior driven development reporting tool. Those results are in turn published to [https://aries-interop.info](https://aries-interop.info) via a GitHub action in the Agent Test Harness repository.

Akrida is built on [Locust](https://locust.io/) and [Credo-TS](https://github.com/openwallet-foundation/credo-ts) to generate loads applied to any deployment.

## Release Methodology

The only “release” from OWL is the test execution results summary published here: [https://aries-interop.info](https://aries-interop.info)

## Initial Maintainers

| Name            | Github      | Organization                             |
| --------------- | ----------- | ---------------------------------------- |
| Sheldon Regular | nodlesh     | Funded by Government of British Columbia |
| Stephen Curran  | swcurran    | Funded by Government of British Columbia |
| Kim Ebert       | KimEbert42  | Indicio, PBC                             |
| Alex Walker     | anwalker293 | Inidicio, PBC                            |
| Ian Costanzo    | ianco       | Funded by Government of British Columbia |
| Timo Glastra    | TimoGlastra | Animo Solutions                          |

## Proposed Project Governance

The current governance model under Hyperledger is consensus-based. This means that decisions are made through discussions, with the aim of community consensus, as outlined in the [Aries Project Charter](https://docs.google.com/document/d/1F6RbR7xDaBt5CDJhqLJzR4c1pDJtyPGshp9fy6eVtSM/edit?usp=sharing). In cases where no clear consensus is established, a project Technical Steering Committee, or the maintainers (those with escalated GitHub privileges) are granted a louder voice. This approach has proven effective.

## Links to Documented Governance Practices

[Project Charter for Aries](https://docs.google.com/document/d/1F6RbR7xDaBt5CDJhqLJzR4c1pDJtyPGshp9fy6eVtSM/edit?usp=sharing).

## Financial Sponsorship

Hyperledger has covered infrastructure related costs. Besides that, None.

## Infrastructure

* GitHub repositories
* CI (GitHub actions)
* Bug Tracking (GitHub Issues and GitHub Projects)
* Communication channels (Discord)
* Mailing list
* Video conference (Zoom)
* Wiki / Meeting Pages (Confluence, likely to move to GitHub/Mkdocs)
* Published Artifacts — Allure (using a Government of British Columbia instance), mkdocs/GH-Pages
