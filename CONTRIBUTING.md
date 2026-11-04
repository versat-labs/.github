# Contributing to Versat Labs

We welcome developers, architects, designers, and technology enthusiasts who want to help us build better solutions.

These are the default contribution guidelines for Versat Labs repositories. If a repository provides its own `CONTRIBUTING.md`, follow that guide. Each project may have specific setup instructions, validation requirements, and licensing terms.

## How You Can Contribute

You can participate at different stages of development:

1. **Plan an existing Issue:** Help refine requirements, define acceptance criteria, propose technical designs, or break work into actionable tasks.
2. **Implement an existing Issue:** Contribute code, tests, and documentation based on approved specifications.
3. **Propose a new Issue:** Identify bugs, suggest improvements, or introduce new ideas. You don't need to implement a solution to make a valuable contribution.
4. **Improve quality:** Strengthen tests, documentation, security, performance, and developer experience.

Explore the **Issues** section of the repository you want to contribute to. Use its available issue forms when reporting a bug, requesting a feature, or proposing maintenance work.

## Before You Start

Read the repository's `README.md`, `AGENTS.md`, `CONTRIBUTING.md`, and applicable specifications where available. Follow its setup instructions and contribution guidance.

If you have access to the private [Versat AI Harness](https://github.com/versat-labs/versat-ai-harness) repository, read its [README.md](https://github.com/versat-labs/versat-ai-harness/blob/main/README.md) before starting and follow its plugin setup guidance. The Harness is the source of truth for Versat's AI-assisted development standards and workflows. Internal Versat contributors already have the plugin installed automatically in our workspace.

Whenever you have questions about Versat's development process, ask Codex to consult the Versat AI Harness plugin and answer based on its documented standards and workflows.

## Set Up Your Local Development Environment

We use Codex in the ChatGPT desktop app for development. Create one local project in the Codex tab for each repository. The app provides file editing and an integrated terminal, so you do not need a separate development IDE.

1. Create a local project with the same name as the repository you want to contribute to.
2. We recommend keeping your repositories in a parent directory named `versat-labs`. Open a terminal in the ChatGPT app, navigate to that directory, and clone the repository:

   ```sh
   git clone <repository_url>
   ```

3. Attach the cloned repository folder to the project and set it as the primary folder. The folder should have the same name as the repository. Start your development chats from this project.

## Our Development Workflow

At Versat, we follow **Spec-Driven Development (SDD)**. We believe great software starts with a clear understanding of the problem, well-defined requirements, and shared agreement on the expected outcome — before writing code.

Our SDD process follows a structured lifecycle:

`Issue → Proposal & Requirements → Design → Tasks → Implementation → Validation → Pull Request`

Planning includes three human approval checkpoints: Proposal & Requirements, Design, and Tasks. Implementation begins after the plan is approved.

For material changes, contributors are expected to:

- Follow the project's SDD process and respect its approval checkpoints.
- Keep specifications, implementation, tests, and documentation aligned.
- Maintain traceability between Issues, requirements, tasks, and Pull Requests.
- Run the required validation checks and submit changes for human review.

## Validation and Pull Requests

Before submitting a Pull Request, run the checks required by the repository and review your changes against the approved specifications. Explain what changed, reference the relevant Issue and specifications, and report the validation results, including any checks you could not complete.

## Language

We use English for code, technical documentation, specifications, and commit messages. Follow each repository's communication and contribution guidelines.

**Helping us define the right problem and design the right solution is equally valuable to contributing code.**
