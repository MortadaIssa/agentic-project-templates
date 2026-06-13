# Backend Architecture

## Technology

- .NET Web API
- C#
- Entity Framework Core
- SQL Server
- Background Worker Service

## Recommended Structure

```text
src/backend/
├── ProjectName.Api/
│   ├── Controllers/
│   ├── Middleware/
│   └── Program.cs
├── ProjectName.Application/
│   ├── Feature1/
│   ├── Feature2/
├── ProjectName.Domain/
│   ├── Entities/
│   ├── Enums/
├── ProjectName.Infrastructure/
│   ├── Data/
│   ├── Repositories/
│   ├── Integrations/
│   └── Configuration/
```

## Backend Rules

- Controllers should be thin.
- Business logic should not be placed directly in controllers.
- Validation must exist on the backend.
- Use DTOs for API requests and responses.
- Do not expose database entities directly from APIs.
- Use transactions when saving business data and related Outbox records together.
- Use clear error responses.
- Log technical errors without exposing sensitive data.

## Example Backend Flow

Creating a entity should follow this flow:

1. API receives `CreateEntityRequest`.
2. Backend validates required fields.
3. Backend checks uniqueness rules.
4. Backend creates the entity.
5. API returns the created Entity response.

## Error Handling

Use consistent error responses:

```json
{
  "code": "Entity_ALREADY_EXISTS",
  "message": "A entity with the same name already exists."
}
```

## Build Command

```bash
dotnet build
```
