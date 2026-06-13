# Data Model

## Main Entities

| Entity | Purpose |
|---|---|
| EntityA | Stores entity A information |
| EntityB | Stores Entity B |
| OutboxMessage | Stores pending and processed integration events |

## Main Relationships

```text
EntityA   1 ---- *      EntityB
EntityC   1 ---- 0..1   EntityD
```

## Entity Notes

### Entity

Important fields:

- Id
- EntityCode
- Name
- Email
- Phone
- TaxNumber
- Status
- ExternalErpCode
- CreatedAtUtc
- CreatedBy
- ModifiedAtUtc
- ModifiedBy

### OutboxMessage

Important fields:

- Id
- EventType
- AggregateType
- AggregateId
- Payload
- Status
- RetryCount
- MaxRetryCount
- NextRetryAtUtc
- LastError
- IdempotencyKey
- ExternalReference
- CreatedAtUtc
- ProcessedAtUtc
