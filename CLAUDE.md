# CLAUDE.md

This file provides guidance for AI assistants working on the **emailcode** repository.

## Project Overview

This is a newly initialized repository. The project name suggests functionality related to email-based verification codes or authentication. As the project evolves, update this file to reflect the actual implementation.

## Repository Status

- **State**: Fresh repository — no source code, dependencies, or configuration yet
- **Remote**: `samueleserratorepms-max/emailcode`

## Development Guidelines

### Getting Started

When initializing this project, establish:

1. A `package.json` (or equivalent manifest for the chosen language/runtime)
2. A source directory structure (e.g., `src/`)
3. A test directory (e.g., `tests/` or `__tests__/`)
4. Linting and formatting configuration

### Conventions to Follow

- **Commits**: Use clear, descriptive commit messages. Prefer conventional commit format (e.g., `feat:`, `fix:`, `docs:`, `test:`, `chore:`)
- **Branching**: Development branches follow the pattern `claude/<description>`
- **Code style**: Configure a linter and formatter early; enforce consistency from the first file
- **Testing**: Write tests alongside new functionality; do not merge untested code
- **Security**: Never commit secrets, API keys, or credentials. Use environment variables and `.env` files (excluded via `.gitignore`)

### Commands

_No build/test/lint commands configured yet. Update this section as tooling is added._

<!-- Example (uncomment and adapt when applicable):
```
npm install          # Install dependencies
npm run build        # Build the project
npm test             # Run tests
npm run lint         # Run linter
npm run lint:fix     # Auto-fix lint issues
```
-->

## Architecture

_No architecture defined yet. Document the following as the project takes shape:_

- Entry points and main modules
- Key abstractions and data flow
- External service integrations (email providers, SMTP, etc.)
- Database or storage layer (if any)
- API surface (endpoints, CLI commands, library exports)

## Key Files

| Path | Purpose |
|------|---------|
| `CLAUDE.md` | AI assistant guidance (this file) |

_Add entries as files are created._

## Maintenance

Keep this file up to date as the project evolves:

- Add new commands when tooling is configured
- Document architecture decisions
- List key files and their purposes
- Note any non-obvious conventions or gotchas
