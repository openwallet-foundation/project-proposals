# Agent Test Harness

## Project Name: To Be Determined

In proposing to bring the current [Aries Agent Test Harness](https://aries-interop.info) to OWF, we suggest merging into it the [Mobile Agent Test Harness](https://github.com/openwallet-foundation/mobile-wallet-test-harness), currently (but not supposed to be) part of the OWF”s Bifold Wallet project. The Mobile Agent Test Harness uses Aries Agent Test Harness in some of its test cases. We also propose including in this testing project the [Aries Akrida](https://github.com/hyperledger/aries-akrida) repository, an agent load testing tool for deployments of ACA-Py and compatible agents. Akrida’s engine is based on the open source [Locust](https://locust.io/) tool, and instances (single or clustered) of OWF’s [Credo-TS](https://github.com/openwallet-foundation/credo-ts). Together, the three components provide rich testing of Agents and Wallets for compatibility, interoperability, and scalability.

## Preferred Maturity Level

We propose that the project be at the “Growth” level.  All three of the components have been used extensively in the past and are well documented. Many groups have used the tools in testing their own instances of the various support agents and wallets.  As we move the project to OWF and start up the Wallet Interoperability Special Interest Group (link to PR to be added) these tools will be useful in enabling testing across frameworks and deployments built on those deployments. We look to expand their use in both the scope of the testing they enable, and their use by the community.

## Project Description

Agent Test Harness is an extensible open-source testing framework designed to validate the functionality and interoperability of agents and components within the decentralized trust ecosystem. A summary of its daily interoperability test runs are published on the website [https://aries-interop.info](https://aries-interop.info). The test harness is crucial for ensuring that different decentralized trust agent implementations, which are responsible for handling decentralized identifiers (DIDs) and exchanging verifiable credentials, can interoperate seamlessly. Agent Test Harness currently includes support for the OWF’s Credo-TS project, and is used by the OWF’s Mobile Agent Test Harness project.

The following are the key features of the Agent Test Harness.

* Interoperability Testing: Agent Test Harness is specifically designed to test the interoperability of agents by executing interactions between them, ensures that agent implementations can communicate using standard protocols, exchange verifiable credential, resolve DIDs, and other core functions reliably.
* Load Testing: Akrida provides a scriptable framework for generating load against a deployment of agents for messaging and exchanging credentials. This allows users of OWF technologies to apply a significant generated load on their deployment to ensure it will scale as needed, and to identify and address bottlenecks.
* Automation: The Agent Test Harness automates the testing of agents, making it easier for developers to continuously verify the compliance and performance of their implementations. Developers can configure what agent implementations with whom they want to test interoperability and for each, what specific tests they want executed. Implementations can even include their CI pipelines select Agent Test Harness interoperability tests.
* Extensibility: The framework is highly extensible, allowing developers to add their implementations for testing and to construct custom tests and scenarios that suit a wide variety of use cases. This flexibility is important for testing a wide range of decentralized identity solutions across different industries.
* Comprehensive Coverage: The test harness covers a wide array of functionalities that decentralized trust agents should support, including secure messaging, protocols, and credential issuance, verification and revocation across a range of credential formats.
* Community-Driven: Agent Test Harness is intended to be developed and maintained by a global community of contributors to ensure that it stays up-to-date with the latest standards and best practices in the decentralized identity space.

As mentioned in the [Project Name](#project-name-to-be-determined) section, we suggest that Agent Test Harness be combined into a single project with the Mobile Wallet Test Harness and Akrida load testing tool. All will be separate repos in the project, but share common project components (governance, meetings, Discord community, etc.).

## Alignment with the OpenWallet Foundation Mission

Agent Test Harness supports the OWF’s goals by focusing on interoperability, and the promotion of open standards within the decentralized identity ecosystem. Notably, Agent Test Harness’s goals in common with the OpenWallet Foundation are:

1. Interoperability: The primary purpose of Agent Test Harness is to ensure interoperability between different agents by validating their ability to communicate using standard protocols like DIDComm and to handle core functions like verifiable credential exchanges. It provides a consistent testing environment to verify that agents from different developers and organizations, evolving independently, can work together seamlessly.
2. Promotion of Open Standards: As an open-source tool, Agent Test Harness is built around open standards and protocols, ensuring that the agents it tests comply with widely accepted norms in the decentralized identity space. This approach encourages the adoption of these standards across the industry, fostering a more unified and interoperable ecosystem.
3. Facilitating Innovation and Adoption:  By providing developers with a tool to validate their agents with those developed by others in the space, Agent Test harness lowers the barriers to entry for creating new, compliant, and interoperable decentralized identity solutions. This facilitates innovation and encourages the adoption of decentralized identity technologies.

## Code of Conduct

ACA-Py follows the [Hyperledger Code of Conduct](https://github.com/hyperledger/aries-agent-test-harness/blob/main/CODE_OF_CONDUCT.md), which is what the OWF code of conduct is based on.

## TAC Sponsor

* Tracy Kuhrt
* TBD

## Project License

The project has an Apache 2.0 license: [Agent Test Harness - License](https://github.com/hyperledger/aries-agent-test-harness/blob/main/LICENSE)

## Source Control

The project is hosted in GitHub and includes the following repositories:

* [Agent Test Harness](https://github.com/hyperledger/aries-agent-test-harness) — test results published to [https://aries-interop.info](https://aries-interop.info)
* [Aries Akrida](https://github.com/hyperledger/aries-akrida) — load testing engine for deployments of ACA-Py and other compatible agents.

## Issue Tracker

Issues are tracked using GitHub's Issues feature in the corresponding repository.

## External Dependencies

The Agent Test Harness itself is built in [Python](https://www.python.org/) using the [Behave](https://github.com/behave/behave) [behavior-driven development](https://en.wikipedia.org/wiki/Behavior-driven_development) (BDD) engine. The repository also contains a component per agent implementation that uses Agent Test Harness.

Test results from the periodic (thrice weekly) interoperability test runs are pushed for later analysis into an instance (operated by [Government of British Columbia](https://www2.gov.bc.ca/gov/content/home)) of the [Allure](https://allurereport.org/docs/pytestbdd/) behavior driven development reporting tool. Those results are in turn published to [https://aries-interop.info](https://aries-interop.info) via a GitHub action in the Agent Test Harness repository.

Akrida is built on [Locust](https://locust.io/) and [Credo-TS](https://github.com/openwallet-foundation/credo-ts) to generate loads applied to any deployment.

## Release Methodology

The only “release” from Agent Test Harness is the test execution results summary published here: [https://aries-interop.info](https://aries-interop.info)

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
