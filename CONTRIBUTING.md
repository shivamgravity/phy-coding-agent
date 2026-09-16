# Contributing

Thank you for your interest in contributing to this project!

This project is being developed as an open-source coding agent, with the goal of building a capable, transparent, and developer-focused agentic system that can understand codebases, analyze dependencies, plan changes, and assist developers with complex software-engineering tasks.

Contributions of all kinds are welcome, including code, documentation, bug reports, feature ideas, tests, examples, and improvements to the developer experience.

## Before You Start

For larger changes, please open an issue or discussion first so that we can talk about the proposed approach before significant development work begins.

Small fixes, documentation improvements, tests, and clearly scoped changes can generally be submitted directly as a pull request.

Please make sure your contribution aligns with the project's goals and existing architecture.

## Contribution Workflow

External contributions should be made through a fork and pull request.

The general workflow is:

1. **Fork** this repository on GitHub.
2. **Clone** your fork locally.
3. Add this repository as an `upstream` remote.
4. Create a dedicated branch for your change.
5. Make your changes and add or update tests where appropriate.
6. Run the relevant tests and checks locally.
7. Push your branch to your fork.
8. Open a pull request from your branch to the `main` branch of this repository.
9. Respond to review feedback and make any requested changes.
10. Once approved, the maintainers will merge the pull request.

Example:

```text
Your fork
    │
    ├── main
    │
    └── feature/your-change
              │
              │ Pull Request
              ▼
This repository
    │
    └── main
```

### Branches

The `main` branch is the primary stable branch of the project.

Please do not push directly to `main`. Changes should be submitted through pull requests.

Use a separate branch for each change. Some examples:

```text
feature/context-ranking
feature/dependency-graph
fix/parser-error
fix/windows-paths
docs/improve-installation
test/agent-planner
```

Avoid combining unrelated changes in the same branch or pull request.

### Keeping Your Fork Updated

Before starting new work, it is recommended to update your local `main` branch from the upstream repository:

```bash
git fetch upstream
git checkout main
git merge upstream/main
```

Then create a new branch:

```bash
git checkout -b feature/your-change
```

The exact Git workflow may vary depending on your preferred tools.

## Development Setup

Clone your fork:

```bash
git clone https://github.com/<your-username>/phy-coding-agent.git
cd phy-coding-agent
```

Add the upstream repository:

```bash
git remote add upstream https://github.com/shivamgravity/phy-coding-agent.git
```

Create and activate a Python virtual environment:

```bash
python -m venv .venv
```

On Linux/macOS:

```bash
source .venv/bin/activate
```

On Windows:

```shell
.venv\Scripts\Activate.ps1
```

Install the project and its development dependencies according to the instructions in the repository README.

Before making changes, make sure the existing tests pass.

## Making Changes

Please keep changes focused and avoid combining unrelated changes in a single pull request.

When working on a feature or architectural change:

1. Understand the existing implementation.
2. Check the relevant documentation and tests.
3. Make the smallest reasonable change.
4. Add or update tests where appropriate.
5. Update documentation when behavior or APIs change.
6. Run the relevant test suite before submitting your pull request.

For changes to the agent's behavior or decision-making, please explain the intended behavior and reasoning in the pull request description.

## Code Quality

Please try to follow the project's existing coding style and conventions.

In particular:

* Prefer clear and maintainable code over clever code.
* Keep functions and modules focused.
* Avoid unnecessary abstractions.
* Do not introduce dependencies without a clear reason.
* Add tests for new behavior where practical.
* Keep public interfaces stable unless a breaking change is intentional.
* Document non-obvious design decisions.

## Pull Requests

Before opening a pull request, please make sure:

* The project builds or runs successfully.
* Relevant tests pass.
* New functionality has appropriate tests where practical.
* Documentation has been updated when necessary.
* The pull request has a clear and descriptive title.
* The pull request description explains what changed and why.
* Unrelated changes have been excluded.

A useful pull request description should generally include:

```text
## What changed?

Briefly describe the changes.

## Why?

Explain the problem or motivation.

## How?

Describe the approach taken.

## Testing

Describe the tests or checks performed.
```

## Issues and Bug Reports

When reporting a bug, please provide as much relevant information as possible.

Useful information includes:

* Operating system
* Python version
* Project version or commit
* Relevant configuration
* Steps to reproduce the issue
* Expected behavior
* Actual behavior
* Error messages or logs
* A minimal reproduction, when possible

Please avoid posting secrets, API keys, passwords, access tokens, private source code, or other sensitive information in issues or pull requests.

## Feature Requests

Feature requests are welcome.

Please describe:

* The problem you are trying to solve.
* Why the feature would be useful.
* Your proposed approach, if you have one.
* Any alternatives you considered.

For larger features, discussing the design before implementation can help avoid unnecessary work.

## Architecture and Design

This project is intentionally designed around a clear separation between its open-source core and any potential future hosted services.

The open-source repository should remain capable of functioning independently without requiring proprietary hosted infrastructure.

When proposing architectural changes, please consider:

* Separation of concerns
* Local-first functionality where appropriate
* Clear interfaces between components
* Extensibility
* Maintainability
* Testability
* Minimal unnecessary coupling

Future hosted or commercial services may be developed separately from this repository. Such services are not part of the current open-source codebase.

## Licensing

This repository is licensed under the MIT License. See [`LICENSE`](LICENSE) for the full license text.

By submitting a contribution to this repository, you agree that your contribution may be distributed as part of this project under the project's applicable open-source license.

You retain ownership of the copyright in your original contribution, subject to the rights granted by the project's license.

At this stage, the project does not require contributors to sign a Contributor License Agreement (CLA) or Developer Certificate of Origin (DCO).

The project's contribution and licensing policies may evolve as the project grows. Any future changes will apply according to their stated terms and will not retroactively alter the licensing terms under which previous contributions were accepted.

## Code of Conduct

Please be respectful and constructive when interacting with other contributors.

Disagreements about technical decisions are expected and can be healthy. Focus criticism on ideas, implementations, and technical trade-offs rather than individuals.

Harassment, personal attacks, discrimination, and deliberately disruptive behavior are not welcome.

## Questions

If you are unsure about where or how to contribute, feel free to open an issue or discussion before starting significant work.

Thank you for helping improve the project!
