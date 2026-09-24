# Cairn Web

This repository will contain the Cairn web application. The application has not been scaffolded yet, so there is no local web server to start. This repository currently contains only the project setup and collaboration instructions.

New developers: read this file first. If setup instructions change, update this README in the same pull request.

## Prerequisites

- Git
- [Bun](https://bun.sh/docs/installation), the JavaScript runtime and package manager used by this project
- Access to the private GitHub repository

Check that Git and Bun are installed:

```sh
git --version
bun --version
```

## Get the code

```sh
git clone https://github.com/prumoh/cairn-web.git
cd cairn-web
```

If the organization or repository name changes, use the clone URL shown on the GitHub repository page.

## Set up and run

Install the project dependencies (none are needed yet):

```sh
bun run setup
```

`bun run update` also installs dependencies in an existing checkout. There are no application dependencies or lockfile yet.

The application has not been created, so `bun run dev` is not available yet. When application tooling is added, this README and `package.json` will be updated in that same pull request.

## Project commands

| Command | Purpose |
| --- | --- |
| `bun run setup` | Prepare a fresh checkout by installing dependencies. |
| `bun run update` | Install dependencies after updating an existing checkout. |

There are no test, lint, typecheck, check, or CI commands yet. Do not treat a missing check as a passing check. Add these commands when the corresponding tools and meaningful checks exist.

## Work through GitHub

GitHub Issues are the source of truth for project work. The [Cairn Web project board](https://github.com/orgs/prumoh/projects/1) tracks work through Backlog, Ready, In Progress, In Review, and Done. The customer can describe a problem or ask a question in an Issue; they do not need to create branches, use a terminal, or understand implementation details. The senior and mid-level developers follow up and turn the problem into development work.

For a change:

1. Find or create the GitHub Issue describing the work. Ask the senior or mid-level developer if you are unsure whether an issue already exists.
2. Update your local `main` branch:

   ```sh
   git switch main
   git pull --ff-only origin main
   ```

3. Create a short-lived branch. Use the Issue number when there is one:

   ```sh
   git switch -c feat/123-short-description
   # or: fix/123-short-description
   # or: chore/short-description
   ```

4. Make a focused change and commit it. Push your branch:

   ```sh
   git add <files-you-changed>
   git commit -m "Describe the change"
   git push -u origin HEAD
   ```

5. Open a Pull Request on GitHub, link the Issue (for example, `Closes #123`), and explain what changed and how you checked it. Keep PRs small.
6. Request a review. Changes to `main` should go through a PR and receive at least one approval. GitHub is not currently enforcing this rule because the private repository's plan does not include branch protection. Until that is resolved, do not merge your own PR; ask the organization owner if you are unsure.
7. Address review feedback, then squash-merge after approval. GitHub deletes the merged branch automatically when configured.

## Before opening a PR

There are no automated application checks yet. Review your changes and run any relevant manual check you can. In particular:

```sh
git diff --check
git status --short
git diff
```

State in the PR what you verified. If a check cannot be run, say so rather than claiming it passed.

## Questions and help

Ask in the related GitHub Issue or PR. If you cannot access the repository or something in these instructions does not work, contact the senior or mid-level developer.
