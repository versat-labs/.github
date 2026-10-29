# Agent instructions

## Repository purpose

This is the `versat-labs/.github` repository for GitHub organization metadata and default contribution files. It is not an application repository. Changes to the organization profile are public-facing; changes to default issue templates can affect repositories across the organization that do not define their own issue templates.

These instructions apply to work in this repository. Do not treat this file as instructions automatically inherited by other repositories in the organization; follow each repository's own guidance when working there.

## Repository map

- `README.md` is the short README for this repository.
- `profile/README.md` is the public Versat Labs organization profile. It describes the mission, vision, areas of work, and contribution paths, and links to the contribution guide.
- `CONTRIBUTING.md` provides the default organization contribution guidelines, including the SDD workflow, approval checkpoints, validation expectations, and language convention.
- `.github/ISSUE_TEMPLATE/bug_report.yaml` is the bug report form (`fix: ` title, `Bug` issue type).
- `.github/ISSUE_TEMPLATE/chore.yaml` is the maintenance form (`chore: ` title, `Task` issue type).
- `.github/ISSUE_TEMPLATE/feature_request.yaml` is the feature request form (`feat: ` title, `Feature` issue type).

All three forms currently target the `versat-labs/1` project. Their required fields capture the information needed for the respective issue type. A repository with its own valid issue templates can override these organization defaults.

## Working conventions

1. Read the files relevant to the requested change and check the working tree before editing. Preserve unrelated user changes and keep the diff focused.
2. Write repository content, technical documentation, issue form text, and commit messages in English, as specified in `CONTRIBUTING.md`. Match the existing concise, welcoming tone of public-facing text.
3. Keep the organization profile accurate. Check proposed claims, destinations, and links before publishing them. Keep mission, vision, and contribution guidance consistent across files.
4. When editing an issue form, preserve its purpose, `name`, title prefix, issue `type`, project association, required questions, and existing field IDs unless the requested change calls for altering them. Keep IDs unique within each form. Use GitHub's [issue form syntax](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-issue-forms) for new fields and metadata.
5. For material changes to the contribution process or organization policy, follow the SDD lifecycle and human approval checkpoints described in `CONTRIBUTING.md`: Proposal & Requirements, Design, and Tasks before implementation. Apply proportionate review to routine copy edits and form maintenance.
6. Do not infer that this repository has a build, package manager, or test suite. Add tooling only when the task warrants it.

## Validation before finishing

- Review the diff and run `git diff --check` to catch whitespace errors.
- For changed YAML forms, parse the YAML and verify the required GitHub form keys, field IDs, required flags, and intended title, type, and project values. Check the rendered form on GitHub when a change depends on GitHub-specific behavior that local YAML parsing cannot verify.
- For changed Markdown, check headings, formatting, and every new or edited link. Preview public-facing content when layout matters.
- Report what changed, what was checked, and any validation that could not be completed.
