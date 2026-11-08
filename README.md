# Versat Labs · Organization Defaults

[English](README.md) | [Português](README.pt.md) | [Español](README.es.md)

English is the canonical source for this README. The Portuguese and Spanish translations are maintained alongside it, following the Versat AI Harness language convention for community-facing documentation.

## Purpose

`versat-labs/.github` is maintained by Versat Labs to centralize the organization's public profile, default contribution guidelines, and issue templates. It follows GitHub's special `.github` repository convention so repositories across the organization can share consistent contribution resources.

This repository contains organization metadata and documentation. It has no application runtime, build process, or automated test suite.

## How GitHub Uses This Repository

- GitHub displays `profile/README.md` on the organization's public profile. See [organization profile documentation](https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/customizing-your-organizations-profile).
- `CONTRIBUTING.md` supplies default guidance where a repository has no contribution guide of its own.
- `.github/ISSUE_TEMPLATE/` supplies default issue forms. A repository's own valid issue templates or template configuration override the entire default folder.
- GitHub references these defaults without copying them into consuming repositories. See [default community health files](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).

`AGENTS.md` and `.gitignore` apply to this repository; GitHub does not distribute them as organization defaults.

## File Guide

| File | Purpose |
| --- | --- |
| [README.md](README.md) | Canonical English overview of this repository, its files, and maintenance workflow. |
| [README.pt.md](README.pt.md) | Portuguese translation of this overview. |
| [README.es.md](README.es.md) | Spanish translation of this overview. |
| [profile/README.md](profile/README.md) | Public organization profile: Versat Labs' mission, vision, areas of work, contribution paths, and useful resources. |
| [CONTRIBUTING.md](CONTRIBUTING.md) | Contribution entry point and links to maintained Harness guidance. |
| [AGENTS.md](AGENTS.md) | Instructions for agents working in this repository, including scope, editing conventions, and validation requirements. |
| [.gitignore](.gitignore) | Excludes local environment files, editor settings, logs, and generated artifacts from version control; allows `.env.example`. These patterns do not imply that build tooling exists here. |
| [.github/ISSUE_TEMPLATE/bug_report.yaml](.github/ISSUE_TEMPLATE/bug_report.yaml) | Bug report form. Requires a description, reproduction steps, and expected behavior; also provides fields for screenshots, device details, and additional context. Uses the `fix: ` title prefix and `Bug` issue type. |
| [.github/ISSUE_TEMPLATE/chore.yaml](.github/ISSUE_TEMPLATE/chore.yaml) | Maintenance form. Requires a description, scope, and completion criteria. Uses the `chore: ` title prefix and `Task` issue type. |
| [.github/ISSUE_TEMPLATE/feature_request.yaml](.github/ISSUE_TEMPLATE/feature_request.yaml) | Feature request form. Requires the problem, job to be done, and user/buyer personas, with optional additional context. Uses the `feat: ` title prefix and `Feature` issue type. |

All three issue forms declare `versat-labs/1` in their `projects` metadata.

## Using the Contribution Resources

Open the repository you want to contribute to, read its contribution guidance, and choose **Issues → New issue**. Where the organization defaults apply, select the bug, feature, or maintenance form, complete its required fields, and submit it. The resulting issue captures the information needed to begin planning. Repository-specific guidance takes precedence.

## Maintaining This Repository

Read [CONTRIBUTING.md](CONTRIBUTING.md) and [AGENTS.md](AGENTS.md) before editing. Keep the three README versions aligned whenever their content changes.

Detailed development instructions are maintained in the [Harness SDD guide](https://github.com/versat-labs/versat-ai-harness/blob/27735687a37e896cd6b0c95cd9d2d848ee166d90/docs/user-docs/guides/sdd-with-codex.md) (private access required). Follow this repository’s AGENTS.md for local review and checks. Public contributors can start from [CONTRIBUTING.md](CONTRIBUTING.md).

### Validation

Start with the validation requirements in [AGENTS.md](AGENTS.md):

1. Review the diff and run `git diff --check`.
2. For Markdown, check headings, formatting, links, and translation alignment. Preview public-facing content when layout matters.
3. For changed issue forms, parse the YAML and verify required keys, unique field IDs, required flags, title prefixes, issue types, and project metadata. Check the form on GitHub when behavior cannot be verified locally.
4. Report the changes, completed checks, and any validation that could not be performed in the pull request.
