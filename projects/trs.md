# Project Name

TRS (Trust Resolver System)

# Preferred Maturity Level

Labs

# Project Description

Currently, there are many trust protocols such as "OpenID federation", "X.509 certificate", "EBSI Trust Chains" and so on. Due to the complexity of these protocols, it is not easy to implement a trust resolver system in client side. That's why Trust Registry Query Protocol(TRQP): https://trustoverip.github.io/tswg-trust-registry-protocol is created.

In this project, we aim to implement a Typescript reference implementation of the TRQP. and extends it so that people can obtain trust information even without detailed knowledge of the standards. My goal is to build an infrastructure like the one described below.

```
                                   +-------------+
                                   |             |
                                   | root server |
                                   |             |
                                   |             |
                                   +-------------+
                                       ↑      |
                   (not standardized)  |      |
                   who can process my  |      |
                         query?        |      |
                                       |      ↓
+-------------+      Query        +---------------+     Query      +--------------+
|             |      (TRQP)       |               |     (TRQP)     |              |
|   client    |------------------>| trust resolver|--------------->|trust registry|
|             |                   |               |                |              |
+-------------+                   +---------------+                +--------------+
```

# Alignment with the OpenWallet Foundation Mission

The Trust System is also a crucial component with the Issuer, Holder and Verifier. Trust System makes sure not only the credential is valid but also the issuers, wallet instances and relying parties are trusted.

# Code of Conduct

[OpenWallet Foundation code of conduct](https://tac.openwallet.foundation/governance/code-of-conduct/)

# TAC Sponsor

@aceshim Ace Shim

# Project License

Apache 2.0

# Source Control

github

# Issue Tracker

github

# External Dependencies

TBD

# Release Methodology

TBD

# Initial Maintainers

- Lukas Han ([Github](https://github.com/lukasjhan))
- Seohee Park ([Github](https://github.com/dvlprsh))

# Proposed Project Governance

Everyone should be able to contribute to the project. Contributors will be able to open issues via Github to discuss their ideas.

# Financial Sponsorship

None

# Infrastructure

Planning to deploy 2 servers for this project. 1 main, 1 backup, just like DNS resolver server.

Clients can access via ip address.
