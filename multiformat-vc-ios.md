# Project Name

Multiformat Verifiable Credentials for iOS

# Preferred Maturity Level

Labs

# Project Description

Pure Swift package for creating Verifiable Credentials (VCs) in multiple formats

- SD JWT "Selective Disclosure for JWTs (SD-JWT)" using the specification defined at https://datatracker.ietf.org/doc/draft-ietf-oauth-sd-jwt-vc/
- VC JWT "Verifiable Credentials as JWTs" using the format defined at JWT VC Presentation Profile https://identity.foundation/jwt-vc-presentation-profile/

Support for multiple data types for disclosed values including

- String
- Int
- Boolean
- Array of Strings - [String]
- Dictionary of String keys and String values - [String:String]

This project is a contribution of the work done at Ping Identity to test and establish interoperability of the various formats representing the Verifiable Credentials Data Model https://www.w3.org/TR/vc-data-model/. Along with the SD-JWT VC and JWT VC formats described above, Ping Identity has also participated in the interoperability event for OpenID4VP to present a VC JWT. That code will also be released as a part of this project.

# Alignment with the OpenWallet Foundation Mission

This Swift package implements three popular formats for Verifiable Credentials. SD-JWT, JWT, and ISO mDoc (coming soon). The library helps with the adoption of these formats for iOS apps written in Swift. This library promotes best practices for the adoption of these standards in user wallets for iOS devices.

# Code of Conduct

[OpenWallet Foundation code of conduct](https://tac.openwallet.foundation/governance/code-of-conduct/)

# TAC Sponsor

Jeremie Miller (https://github.com/quartzjer)

# Project License

[Apache License, Version 2.0](https://opensource.org/license/apache-2-0/)

# Source Control

[https://github.com/pingidentity/MultiformatVC-iOS](https://github.com/pingidentity/MultiformatVC-iOS)

# Issue Tracker

- Github Issues

# External Dependencies

- None

# Release Methodology

_N/A (not applicable)_

# Initial Maintainers

Gaurav Khot([Github](https://github.com/gauravping))

# Proposed Project Governance

_None_

# Links to Documented Governance Practices

https://docs.google.com/forms/d/e/1FAIpQLSeO1bDGHUP-ZpCo1uynm94YOxZlek6RhCH7o3FnX1lZSXXfSQ/viewform?fbzx=4351560609072672295

# Financial Sponsorship

[Ping Identity, Denver, CO](https://pingidentity.com)

# Infrastructure

- None
