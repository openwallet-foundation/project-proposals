# Project Name
ACA-py Minimal Example (AME)

# Preferred Maturity Level
Labs (fits under "long-established projects with minimal resource needs").

# Project Description

AME is a tool for creating a minimal reproducible instance of ACA-py, allowing users to quickly reproduce a bug or demo a feature with a simple script. It contains a hackable controller able to interact with an ACA-py instance, and some pre-defined protocols that cause two ACA-py instances to interact.

# Alignment with the OpenWallet Foundation Mission

This project hopes to support the OWF's mission to promote the development of digital wallets by providing a helpful tool for developers using ACA-py to interact with it quickly and easily.

It has been used for these purposes by Indicio (e.g. [here](https://github.com/Indicio-tech/acapy-did-indy/blob/feat/anon-creds/demo/demo.py)), as well as by the broader community (e.g. [here](https://github.com/openwallet-foundation/acapy/issues/3624#issuecomment-2809561863)).


# Code of Conduct

We will adopt the OWF's Code of Conduct.

# TAC Sponsor
Indicio

# Project License

Apache 2.0.

# Source Control

https://github.com/Indicio-tech/acapy-minimal-example

https://github.com/Indicio-tech/acapy-minimal-example-template

# Issue Tracker

https://github.com/Indicio-tech/acapy-minimal-example/issues

https://github.com/Indicio-tech/acapy-minimal-example-template/issues

# External Dependencies

```
async-selective-queue = "^0.1.1" (Apache 2.0)
aiohttp = "^3.9.5" (Apache 2.0)
pydantic = {version = "^2.8.2", optional = true} (MIT)
blessings = "^1.7" (MIT)
pytest = "^8.4.1" (MIT)
poetry = "^1.0.0" (MIT)
```

# Release Methodology

N/A

# Initial Maintainers

Athan Massouras (@Athan13)

# Proposed Project Governance

Will be led by the team at Indicio and managed by Athan Massouras, a member of that team.


# Financial Sponsorship

None.

# Infrastructure

None.
