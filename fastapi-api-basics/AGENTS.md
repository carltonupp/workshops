# AGENT INSTRUCTIONS

## General Guidelines

- Adhere to SOLID Principles where possible
- Ensure code is clean and easily readable, avoiding high cyclomatic complexity
- Utilise DDD where it makes sense
- All business logic should be unit tested
- Use command line tools where possible for scaffolding code
- Prefer open standards to vendor-specific files for agentic use (AGENTS.md, agent skills)

## Technology Choices

- Language: Python (latest stable, managed by `uv`)
- Package & environment management: uv (never pip, poetry or conda)
- Web Framework: FastAPI
- HTTP client: httpx (runtime and testing)
- Data layer: SQLModel backed by SQLite
- Testing: pytest with FastAPI's TestClient
- Linting & formatting: ruff

## Git Guidelines

- use semantic commit messages standard for commits
- branch names should be descriptive
- when starting a new session, a new branch should be created
