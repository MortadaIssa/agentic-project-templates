# Security Architecture

## Authentication

The system uses authenticated access for internal users.

The exact authentication provider may evolve, but backend APIs must require authenticated access unless an endpoint is explicitly public.

## Authorization

Authorization must be enforced in the backend.

Frontend route protection is required for user experience, but it is not sufficient by itself.

## Role-Based Access

| Feature | Admin | X Role | Y Role | Z Role |
|---|---:|---:|---:|---:|
| Users | Manage | NULL | NULL | NULL |
| Entity A | Manage | View, Edit | View | View, Edit, Delete |
| Entity B | Manage | View | View | View, Edit |

## Secrets Management

- Do not commit real secrets to the repository.
- Use local user secrets, environment variables, or secure secret stores depending on the environment.
- Keep `.env.example` or configuration templates with dummy values only.
- AI agents should work with dummy configuration values.
- Real credentials must be handled by developers or DevOps through approved secure channels.

## Logging

Do not log:

- Passwords.
- Access tokens.
- Refresh tokens.
- API keys.
- Full connection strings.
- Sensitive personal data unless explicitly approved and protected.

## Input Validation

- Validate all input on the backend.
- Treat frontend validation as a user experience improvement only.
- Return clear validation messages without exposing internal technical details.
