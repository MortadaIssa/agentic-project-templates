# Architecture Overview

## Solution Summary

The Customer Operations Platform is a web application composed of:

- React frontend.
- .NET Web API backend.
- SQL Server database.
- Background worker for asynchronous processing.
- External ERP integration using the Outbox pattern.

## Architecture Principles

- Keep business rules in the backend.
- Do not trust calculations from the frontend.
- Use database transactions for operations that must be saved consistently.
- Use asynchronous integration for external systems that may fail or be unavailable.
- Keep integration logic isolated from core business logic.
- Avoid introducing new libraries or frameworks without a clear need.
- Prefer simple architecture first, then evolve when requirements justify it.

## Main Technical Decisions

| Decision | Reason |
|---|---|
| React with TypeScript | Maintainable frontend with type safety |
| .NET Web API | Strong backend platform for enterprise applications |
| SQL Server | Relational data model with transactional consistency |
| Outbox Pattern | Reliable external integration with retry and traceability |
| Background Worker | Processes integration records without blocking users |
