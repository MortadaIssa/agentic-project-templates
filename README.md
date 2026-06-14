# [Replace this text with the title of the project]

## Overview

[Write here a brief description about the project].

## Business Purpose

[What main problems this project solves].

## Technology Stack

- Frontend: React with TypeScript
- Backend: .NET Web API
- Database: SQL Server
- Background Processing: .NET Worker Service
- Authentication: JWT-based authentication

## Documentation Map

| Area | File |
|---|---|
| Requirements index | `docs/requirements/index.md` |
| Requirement Example | `docs/requirements/requirement-example.md` |
| Architecture overview | `docs/architecture/overview.md` |
| Backend architecture | `docs/architecture/backend.md` |
| Frontend architecture | `docs/architecture/frontend.md` |
| Agent instructions | `AGENTS.md` |

## Local Development

Backend:

```bash
cd src/backend
dotnet build
```

Frontend:

```bash
cd src/frontend
npm install
npm run dev
```

## Important Notes

- Detailed requirements are maintained under `docs/requirements/`.
- Technical decisions are maintained under `docs/architecture/`.
- AI agents must follow `AGENTS.md` before making code changes.
