# AI Development Capstone

An AI-assisted software development capstone project, built with a documented, repeatable workflow between a developer and AI coding assistants.

## Project Overview

This repository is the foundation for a capstone that demonstrates how to plan, build, test, and version a software project with AI assistance while keeping the developer in control of design decisions and code review.

The project is currently in its **setup phase**. No application code has been written yet.

## Purpose of the Capstone

- Show a disciplined, professional workflow for AI-assisted development.
- Establish clear rules that AI coding assistants follow when working in this repository.
- Keep a clean, reviewable Git history using Conventional Commits.

## Technology Stack

Current tooling:

- Node.js
- JavaScript / TypeScript
- Git and GitHub
- Claude Code and/or Cursor as AI coding assistants

Application frameworks, databases, and libraries have not been chosen yet and will be listed here once they are adopted.

## AI-Assisted Development Approach

AI assistants are used as collaborators, not autonomous authors. Their behavior is governed by [`CLAUDE.md`](./CLAUDE.md), which requires them to:

- Inspect and understand existing code before changing it.
- Make the smallest appropriate change.
- Run relevant tests and review the diff before a task is considered done.
- Never handle secrets unsafely.

All AI-generated changes are reviewed by the developer before being committed.

## Development Workflow

1. Define the task and its scope.
2. Have the AI assistant inspect the relevant files and propose the smallest appropriate change.
3. Implement the change.
4. Run tests or validation and review `git diff`.
5. Commit using Conventional Commits.
6. Push and open a pull request or merge, as appropriate.

## Repository Structure

```text
.
├── .gitignore    # Files and folders excluded from version control
├── CLAUDE.md     # Rules and workflow for AI coding assistants
├── LICENSE       # MIT License
└── README.md     # Project documentation
```

The structure will be updated as source code, tests, and configuration are added.

## Setup Instructions

Prerequisites:

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/) (current LTS recommended)

```bash
git clone <repository-url>
cd <repository-folder>
```

There are no dependencies to install yet. Install and run instructions will be added once the application is scaffolded.

## Development Conventions

- **Commits:** [Conventional Commits](https://www.conventionalcommits.org/) (`feat:`, `fix:`, `docs:`, `test:`, `refactor:`, `chore:`).
- **Code:** readable, maintainable, small focused functions, clear naming, minimal dependencies.
- **Security:** never commit secrets; use environment variables and keep `.env` files out of Git.
- **Scope:** keep changes minimal and avoid touching unrelated files.

See [`CLAUDE.md`](./CLAUDE.md) for full details.

## Current Project Status

**Setup phase.** Repository documentation and configuration files are in place: `README.md`, `LICENSE`, `.gitignore`, and `CLAUDE.md`. No application features, tests, or dependencies have been added yet.

## License

Released under the [MIT License](./LICENSE).
