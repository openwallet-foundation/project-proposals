![OpenWallet Foundation Logo](https://openwallet.foundation/wp-content/uploads/sites/11/2023/02/OpenWallet_Logo_Color-with-descriptor.svg)

# Hosting Projects under the OpenWallet Foundation
The OpenWallet Foundation (OWF) is the home to various open source,
open data and/or other open projects relating to or supporting development
of digital wallets, including infrastructure and support initiatives related.
The [OWF Project Lifecycle](https://openwallet-foundation.github.io/tac/governance/project-lifecycle/)
specifies the stages that a project may be admitted under and what the
criteria and expectations are for a given stage, as well as the acceptance
criteria for a project to move from one stage to another.

The project proposal process is the same for both existing projects which
seek to move into the OpenWallet Foundation and new projects to be formed
within the OpenWallet Foundation.

This repository will be used for OpenWallet Foundation project proposals.
It contains the [proposal template](./proposal-template.md) and projects
that have been proposed for consideration to the OpenWallet Foundation TAC.

# Instructions for Proposing a Project
The seed of a new project has to be vetted in a public forum like the
[TAC mailing list](https://lists.openwallet.foundation/g/TAC) before
creating a project proposal. It is best if the project has specific maintainers
with a common software-implemented mission. A clear statement of the problem
and its technical details are helpful to coalesce the community around a
solution and prompt volunteers.

If this project proposal is for a feature that is unique to an existing
OpenWallet Foundation project, please reach out to that project’s maintainers
to see about joining that project instead of creating a new project proposal.
If discussion with the existing project community leads to not joining, then
the proposal will be reviewed on its own merits as an independent project.
Please note in the proposal the conversations with that project and the reason
for not joining their efforts.

1. Fork [this repository](https://github.com/openwallet-foundation/project-proposals).
2. Copy the `proposal-template.md` file to the `projects` directory and rename
the file to `project-name.md`, where _project-name_ is the name of your project.
3. Complete the template.
4. Commit your changes with proper sign-off. This means that your commit
log message must contain a line that looks like the following one,
with your actual name and email address:

        Signed-off-by: Jane Doe <jane.doe@example.com>

   Adding the `-s` flag to your `git commit` command will add that line
automatically. You can also add it manually as part of your commit
log message or add it afterwards with `git commit --amend -s`.
5. Submit a pull request.

# Fixing DCO on Existing Repositories

In order to bring an existing source base to the OpenWallet Foundation, the repository must have [DCO](https://developercertificate.org/) signoff on all commits. If your existing repository does not have DCO signoff on all commits, you will need to do one of two things:

1. bring your code by squashing all of your commits into a single first commit made against a new OWF repo with your DCO sign-off.

2. amend the commit history to include DCO sign-off for each of the commits. The Hyperledger Indy community has [documented steps to fix DCO on previous commits](https://github.com/hyperledger/indy-sdk/blob/main/docs/contributors/signing-commits.md#how-to-sign-previous-commits). Also, the [Fix DCO Guide from src-d](https://github.com/src-d/guide/blob/master/developer-community/fix-DCO.md) contains some different steps you can take.
