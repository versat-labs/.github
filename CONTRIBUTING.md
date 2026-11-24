# Contributing to Versat Labs

[English](CONTRIBUTING.md) | [Português](CONTRIBUTING.pt.md) | [Español](CONTRIBUTING.es.md)

Developers, architects, designers and other contributors can help plan or implement an existing issue, propose a new issue, or improve quality. Choose the repository you want to help and read its README, AGENTS.md and contribution guidance where available. A repository’s own CONTRIBUTING.md takes precedence over these organization defaults.

## Start a contribution

Open **Issues → New issue** in the target repository and use its available bug, feature or maintenance form. Describe the problem, relevant context and expected result; include reproduction steps for a bug. You can contribute a well-defined issue without implementing it. Before working on files, follow that repository’s setup, specifications and validation requirements. In a PR, link the issue, explain the change and report actual checks and any unavailable verification.

## Install the Versat AI Harness plugin

The `versat-ai-harness` plugin provides reusable Skills and guidance for planning, implementing and validating contributions with Codex. Follow the installation path for your account. The menu labels below are shown in English.

### Members of the Versat workspace

1. In Codex, select the Versat workspace and open **Settings > Plugins > Browse Directory > Versat**.
2. Open **Versat-ai-harness** and select **Install**.

The workspace administrator manages distribution. If the plugin is not listed or installation is unavailable, contact the workspace administrator.

### External contributors

If your Codex account is not part of the Versat workspace:

1. Open **Settings > Plugins > Add > Add Marketplace**.
2. In **Source**, enter the Harness repository URL: [https://github.com/versat-labs/versat-ai-harness](https://github.com/versat-labs/versat-ai-harness).
3. Confirm the marketplace addition. In the added **Versat Plugins** marketplace, find `versat-ai-harness` and select **Install**. Adding the marketplace and installing the plugin are separate steps.

**Update manually for every new release.** Review the release instructions and compatibility with your project, refresh the added marketplace, and update the installed plugin using the controls supported by your Codex version. Confirm the installed version in a new chat before continuing; refreshing the catalog alone does not confirm a plugin update. If the selected version is unavailable or the update fails, contact the Harness maintainers before continuing with that version.

The Harness repository is public. Access to the repository you want to contribute to is separate from plugin installation.

## Start using the plugin

1. Clone or open the target repository as your Codex project. Read its README, AGENTS.md and contribution guidance.
2. Start a new chat after installation or an update and ask Codex to verify the setup:

   ```text
   Confirm the current project folder, the installed versat-ai-harness version and where you found its versat-sdd Skill and matching canonical resources. Report any missing prerequisites before changing files.
   ```

3. Once the setup is confirmed, use a real issue to request an initial plan. Replace the placeholders below:

   ```text
   Use $versat-sdd to plan change <change-name> for issue <issue-url>: <describe the problem and expected result>. Create Proposal and Requirements only; do not implement. Stop for Gate 1 review.
   ```

Expect `specs/changes/<change-name>/proposal.md` and `requirements.md`, written in English. Review them before approving the next stage. Design and Tasks follow their respective approval gates; implementation requires an explicit request after Tasks review. If the Skill or its resources are missing, resolve the installation with the workspace administrator or Harness maintainers before continuing.

## Harness guides

These links point to the maintained Harness documentation on `main`; follow the documentation matching your installed release when working on a versioned project. You can still propose an issue through the public contribution route without installing the plugin.

- [First use](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/quickstart.md)
- [Workspace setup](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/guides/workspace-setup.md)
- [SDD and approvals](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/guides/sdd-with-codex.md)
- [GitHub delivery](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/guides/github-delivery.md)
- [Validation](https://github.com/versat-labs/versat-ai-harness/blob/main/docs/user-docs/guides/validation-and-evaluations.md)
- [Canonical language policy (English)](https://github.com/versat-labs/versat-ai-harness/blob/main/standards/core/language.md)

## Rights and provenance

Before proposing code, text or assets, identify their source, applicable permissions and required notices. If you cannot establish permission to contribute an illustration, omit it and ask the repository owner; an issue or technical review does not supply missing rights. Follow the target repository's actual terms. Permission to use an internal development tool is separate from the destination project's license, and installing that tool is not required for the public contribution route above. This guidance introduces no CLA, DCO or rights assignment.

## Security reports

For ordinary bugs, use Bug report. For suspected vulnerabilities in public repositories, use GitHub Private Vulnerability Reporting when enabled. For private repositories, email the relevant CODEOWNERS through existing internal Versat channels. Do not disclose vulnerability details in ordinary issues. See [security reporting](SECURITY.md) for routing and unavailable-channel recovery.
