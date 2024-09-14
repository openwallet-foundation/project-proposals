# DIDComm Mediator Service

## Project Name: DIDComm Mediator Service

The DIDComm Mediator Service supports mobile DIDComm agents as a reliable intermediary providing an addressable HTTP endpoint for secure message routing. This enables mobile agents with intermittent connectivity to receive messages from enterprise or other agents through a trusted, decentralized communication channel. In leveraging DIDComm, the service ensures end-to-end encrypted, verifiable message delivery, allowing enterprises to send notifications and initiate interactions with mobile users in a secure and trusted manner.

The DIDComm Mediator Service offers a secure alternative to traditional, untrusted notification/communication methods like email, SMS, and mail. It is particularly beneficial for mobile users who need a persistent communication link without sacrificing privacy and security, playing an important role in maintaining seamless communication in decentralized identity ecosystems.

## Preferred Maturity Level

We propose that the project go into OWF as a “Growth” project. The implementation has been deployed by many parties in both production and proof of concept scenarios and has proven to be reliable and scalable. It is easily deployed and “just works”. The included “SocketDoc” repository can provide expanded horizontal scalability not currently part of the current deployment. We think a fully scalable implementation of a DIDComm mediator could be an “Impact” project.

## Project Description

The DIDComm Mediator Service is an open-source project designed to facilitate DIDComm communication between Aries agents, particularly in situations where agents are on mobile devices, behind firewalls, or have intermittent connectivity. A DIDComm mediator serves as a persistent endpoint for client agents, allowing them to receive messages securely and efficiently, even when direct peer-to-peer communication is not possible. This allows a peer contact, such as an enterprise issuer or verifier, to initiate a messaging exchange with a mobile agent. This is a substantial improvement of the situation today, when enterprises are limited to initiating interactions or sending notifications via untrusted emails and SMSs that are often discarded as phishing attacks.

### Key Features:

* **DIDComm Message Relaying**: The primary function of the DIDComm Mediator is to relay inbound DIDComm messages to client agents. It enables agents that cannot maintain an addressable endpoint to receive messages through a trusted third-party mediator, ensuring that communication remains uninterrupted. The mediator has no visibility to the embedded message being relayed.
* **Routing and Delivery**: The service offers routing capabilities, directing DIDComm messages to the correct recipient even if the recipient’s agent is temporarily offline. It queues messages and delivers them when the recipient becomes available, enhancing reliability in environments with unstable connections.
* **Extensibility and Customization**: DIDComm Mediator is designed to be flexible and customizable, allowing developers to extend its functionality according to specific use cases. It embeds the deployers' choice of ACA-Py or Credo-TS to handle the DIDComm messaging. That underlying power makes DIDComm Mediator Service adaptable to a wide range of deployment scenarios, from simple message relaying to more complex mediation tasks.
* **Community-Driven Development**: DIDComm Mediator Service is developed and maintained by a global community of contributors. This collaborative approach ensures that the service evolves in line with the needs of the broader decentralized identity ecosystem.

The service is particularly useful for agents operating on mobile devices or in environments where maintaining a constant connection is challenging. It ensures that unsolicited messages and notifications can be sent from a known peer via an established connection.

## Alignment with the OpenWallet Foundation Mission

The DIDComm Mediator aligns with the mission of the Open Wallet Foundation (OWF) in several critical ways, particularly in terms of enhancing interoperability, ensuring reliable communication, and promoting open-source solutions for digital wallets and decentralized identity systems.

1. **Interoperability and Seamless Communication**: The service is designed to facilitate DIDComm communication between DIDComm agents, especially when direct peer-to-peer connections are not possible due to network constraints like firewalls or intermittent connectivity. By ensuring that messages can be reliably routed and delivered through a mediator, the service enables seamless communication between different agents and systems.
2. **Support for Decentralized Identity**: The service plays a role in decentralized identity systems by ensuring that agents without persistent endpoints can securely receive DIDComm messages. This helps maintain the integrity and confidentiality of identity-related messages, even when direct communication channels are not available.
3. **Reliability in Diverse Environments**: By acting as an intermediary that queues and relays messages, the service ensures that inbound DIDComm messages to agents are reliable, even in environments with intermittent connectivity or where agents are behind firewalls. This is particularly important for mobile devices, edge computing, and other scenarios where maintaining a continuous connection is challenging.
4. **Open-Source Collaboration and Innovation**: As an open-source project, DIDComm Mediator is developed and maintained by a global community.
5. **Security and Privacy**: The service supports secure DIDComm messaging, ensuring that communication between agents is encrypted and privacy-preserving. A DIDComm mediator cannot decrypt the contents of the message sent to a client agent. This is critical in protecting user data and maintaining the security of decentralized identity systems.

## Code of Conduct

DIDComm Mediator Service follows the [Hyperledger Code of Conduct](https://github.com/hyperledger/aries-agent-test-harness/blob/main/CODE_OF_CONDUCT.md), which is what the OWF code of conduct is based on.

## TAC Sponsor

* Tracy Kuhrt
* TBD

## Project License

The project has an Apache 2.0 license: [Aries Mediator Service - License](https://github.com/hyperledger/aries-mediator-service/blob/main/LICENSE)

## Source Control

The project is hosted in GitHub and includes the following repositories:

* [Aries Mediator Service](https://github.com/hyperledger/aries-mediator-service)
* [Aries SocketDock](https://github.com/hyperledger/aries-socketdock)

## Issue Tracker

Issues are tracked using GitHub's Issues feature in the corresponding repository.

## External Dependencies

DIDComm Mediator Service is deployed on an DIDComm Agent framework with examples
included using [ACA-Py](https://aca-py.org) and
[Credo-TS](https://github.com/openwallet-foundation/credo-ts). DIDComm Mediator
Service also uses (via its embedded DIDComm agent)
[Askar](https://github.com/hyperledger/aries-askar) for key management services
and secure storage.

## Release Methodology

DIDComm Mediator Service uses GitHub Actions for dependency notifications and
management. The primary artifacts are Docker files that can be configured and
used to deploy a fully featured, out of the box DIDComm mediator.

## Initial Maintainers

| Name           | Github      | Organization                             |
| -------------- | ----------- | ---------------------------------------- |
| Stephen Curran | swcurran    | Funded by Government of British Columbia |
| Wade Barnes    | WadeBarnes  | Funded by Government of British Columbia |
| Daniel Bluhm   | dbluhm      | Indicio, PBC                             |
| Timo Glastra   | TimoGlastra | Animo Solutions                          |

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
