# CLAUDE.md

Guidance for AI coding assistants (Claude Code, Cursor, or similar) working in this repository.

## Project Overview

This is an AI-assisted development capstone. The goal is a clean, well-documented project built through a disciplined workflow with the developer reviewing all changes. The repository is currently in its **setup phase**: only documentation and configuration files exist, and no application code has been written yet.

## Technology

Current tooling:

- Node.js
- JavaScript / TypeScript
- Git
- GitHub
- Claude Code / Cursor

Do not claim or assume that any framework, library, database, or service is in use unless it is actually present in the repository. Check `package.json` and the source tree first.

## Coding Conventions

- Write readable and maintainable code.
- Prefer small, focused functions with a single responsibility.
- Use clear, descriptive names for variables, functions, and files.
- Make minimal changes; do not refactor or reformat unrelated code.
- Reuse existing code and utilities where appropriate.
- Avoid unnecessary dependencies; justify any new one before adding it.

## Git Conventions

Use [Conventional Commits](https://www.conventionalcommits.org/). Examples:

- `feat: add user authentication`
- `fix: resolve validation issue`
- `docs: improve README`
- `test: add API tests`
- `refactor: simplify service logic`
- `chore: update dependencies`

Do not commit, push, or rewrite Git history unless the developer explicitly asks.

## AI Development Workflow

Before and while changing code:

1. Inspect the relevant files.
2. Understand the existing implementation.
3. Identify the smallest appropriate change.
4. Explain important assumptions when necessary.
5. Implement the change.
6. Run relevant tests or validation.
7. Review the final diff.
8. Avoid modifying unrelated files.

Only report work as done if it was actually performed and verified.

## Security

Never:

- commit API keys
- commit passwords
- commit tokens
- expose secrets
- hard-code credentials

Use environment variables for secrets. Keep `.env` files out of version control and provide a `.env.example` with placeholder values when configuration is needed.

## Testing

Before considering a task complete:

- Run relevant tests.
- Check for errors.
- Verify the application still works.
- Inspect `git diff`.
- Ensure only intended files changed.

Do not write placeholder or fake tests just to make checks pass. If no tests exist for the area you changed, say so.

## Definition of Done

A task is complete only when all of the following are true:

- Verify the implementation after making a change.
- Run relevant tests or validation.
- Review the final `git diff`.
- Ensure no secrets are exposed or committed.
- Ensure only intended files were modified.
- Update documentation when project behavior changes.