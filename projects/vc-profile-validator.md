# Project Name
VC Profile Validator

# Preferred Maturity Level
Labs

# Project Description
VC Profile Validator provides a lightweight validation engine and CLI for checking whether a VC or VP satisfies a declared profile. Profiles are expressed as versioned YAML bundles, and the validator evaluates inputs against those rules to produce structured findings and summary results.

The project is valuable because it provides a reusable validation utility that can be run independently by implementers or used beneath broader interoperability and testing systems. This makes profile conformance checks more repeatable, transparent, and easier to automate in local development and CI workflows.

The project originated from practical implementation and contribution experience across the wallet ecosystem, where a recurring need emerged for a smaller validation tool that sits below a full interoperability harness. The current repository is an early pre-1.0 implementation with working CLI support, batch execution, Docker packaging, OWF-oriented fixtures and suites, and supporting design documentation.

The current implementation includes:

- Profile loading and schema validation
- Rule-based VC/VP validation
- CLI and batch execution
- JSON and HTML reporting
- Docker packaging
- OWF-oriented fixtures, suites, and design documentation

The project is intentionally narrow in scope. It is intended to complement broader OWF interoperability efforts such as OWL by providing a smaller reusable validation utility that can be run in local development and testing workflows. It is not a wallet, SDK, or certification program.

# Alignment with the OpenWallet Foundation Mission
VC Profile Validator aligns with the OpenWallet Foundation mission by supporting interoperable digital wallet ecosystems through open, reusable validation tooling. It helps projects express interoperability expectations as reusable profiles and verify them consistently in development, CI, and test workflows.

# Code of Conduct
The current repository does not yet include a dedicated project Code of Conduct. If accepted into OWF, the project will adopt and follow the [OpenWallet Foundation Code of Conduct](https://tac.openwallet.foundation/governance/code-of-conduct/).

# TAC Sponsor
TBD

# Project License
Apache License 2.0.

The current repository is already licensed under Apache-2.0. If accepted, the project will follow OWF contribution and asset transfer requirements.

# Source Control
Current source repository:

- https://github.com/sonivijayk/vc-profile-validator

If accepted, the project is expected to move to OpenWallet Foundation GitHub infrastructure.

# Issue Tracker
Current issue tracker:

- https://github.com/sonivijayk/vc-profile-validator/issues

If accepted into OWF, the project is expected to use GitHub issues in the OWF-hosted repository as the primary public issue tracker.

# External Dependencies
Current runtime dependencies are intentionally minimal:

- `PyYAML` (MIT License)
- `jsonschema` (MIT License)

Test dependency:

- `pytest` (MIT License)

# Release Methodology
The project is currently in an early phase and does not yet have a formal published release process. The intended release methodology is:

- GitHub-based tagged releases
- Semantic versioning
- CI-based test execution before release
- Release notes describing notable validation behavior changes

# Initial Maintainers
- Vijay Kumar Soni (`@sonivijayk`)

# Proposed Project Governance
The project is currently maintainer-led, with development and technical decisions handled through open pull requests and issue discussion. The initial maintainer is Vijay Kumar Soni, with the expectation that maintainer participation can broaden over time under OWF.

# Financial Sponsorship
None

# Infrastructure
The project expects to utilize the following OWF Lab services:

- GitHub repository hosting
- GitHub issues and pull requests
- Chat channel for project collaboration
- CI workflows for automated test execution
- Standard OWF project governance and community files

No special infrastructure beyond standard OWF Lab services is currently required. If accepted as a Lab, the project README and project materials will be updated to identify the project as an OpenWallet Foundation Lab.
