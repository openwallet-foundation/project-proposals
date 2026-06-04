# ISO MDL UniFFI
This project provides Python bindings for the ISO 18013-5 Mobile Driver's License (mDL) library using UniFFI, allowing interaction with mDL documents from Python applications.

# Preferred Maturity Level
Given that this project serves primarily as a component piece to a different project ([OID4VC](https://github.com/openwallet-foundation/acapy-plugins/tree/main/oid4vc)), the `Labs` maturity level seems most appropriate. 

# Project Description
The ISO MDL UniFFI library provides a Python interface to the Rust-based isomdl library, enabling:
- Holder functionality: Create presentation sessions for mDL documents
- Reader functionality: Verify and read mDL documents from holders
- Document management: Create, manage, and present mobile driver's licenses
- Cross-platform support: Works on macOS, Linux, and Windows

```
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   Python App    │ ←→ │  UniFFI Bindings │ ←→ │   Rust Library  │
└─────────────────┘    └──────────────────┘    └─────────────────┘
                                                        │
                                                ┌───────▼───────┐
                                                │  isomdl crate │
                                                └───────────────┘
```

# Alignment with the OpenWallet Foundation Mission
1. **Interoperability**: This project exists primarily to bridge the gap between SpruceID's `isomdl` library and the OID4VC plugin, allowing for multiple projects to use the same underpinnings for mDL support, which reduces friction when developing different components of a credential ecosystem.

# Code of Conduct
This project has a code of conduct derived from [Contributor Covenant 2.1](https://www.contributor-covenant.org/version/2/1/code_of_conduct.html).

# TAC Sponsor
N/A

# Project License
This project is currently under both the Apache 2.0 and MIT licenses.

# Source Control
[Here](https://github.com/Indicio-tech/isomdl-uniffi) is a link to the current project repository.

# Issue Tracker
Any issues in this project will be captured in the [Issues tab](https://github.com/Indicio-tech/isomdl-uniffi/issues) on GitHub.

# External Dependencies
The primary external dependency is SpruceID's [`isomdl`](https://github.com/spruceid/isomdl) repository.

# Release Methodology
There is not a particularly established release process for this project yet.

# Initial Maintainers
- Micah Peltier: `mepeltier`
- Patrick Kenyon: `TheTreek`

# Proposed Project Governance
N/A

# Financial Sponsorship
None.

# Infrastructure
N/A