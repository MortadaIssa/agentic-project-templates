# Sample Requirements

## Objective

[Brief Description here]

## Actors

| Actor | Description |
|---|---|
| Admin User | Manages the configuration |
| X user | Create, update, delete entities |


## Functional Requirements

| ID | Requirement |
|---|---|
| EXP-001 | The user can do xyz. |
| EXP-002 | The system should do xzy. |
| EXP-003 | The system generates a entity serial number. |
| EXP-004 | The user can export all entties as Excel. |

## Entity Statuses

| Status | Description |
|---|---|
| Draft | Entity generated but not finalized |
| In Progress | Entity is under processing |
| Completed | For successfull records |

## Business Rules

- Entity cannot be added unless xyz are provided.


## Validations

| Field | Validation |
|---|---|
| Field1 | Required, must be unique |
| Field2 | Required |
| Field3 | Optional, should be in email format |

## API Expectations

| Operation        | Expected Endpoint           |
| ---------------- | --------------------------- |
| List Entities    | `GET /api/entities`         |
| Get Entity by ID | `GET /api/entities/{id}`    |
| Create Entity    | `POST /api/entities`        |
| Update Entity    | `PUT /api/entities/{id}`    |
| Delete Entity    | `DELETE /api/entities/{id}` |

## Out of Scope

- [Anything that you expect that the agent might include in scope and you explicitly want to exclude it for now].

## Acceptance Criteria

- [Always explain to an LLM and let it help you with writing the acceptance criteria].
