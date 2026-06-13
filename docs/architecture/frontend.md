# Frontend Architecture

## Technology

- React
- TypeScript
- Vite
- React Router
- API client layer for backend communication

## Recommended Structure

```text
src/frontend/
├── src/
│   ├── app/
│   ├── api/
│   ├── components/
│   ├── features/
│   │   ├── feature1/
│   │   ├── feature2/
│   ├── layouts/
│   ├── routes/
│   ├── shared/
│   └── main.tsx
```

## Frontend Rules

- Keep pages focused on screen composition.
- Keep reusable UI elements inside `components/` or `shared/`.
- Keep feature-specific code inside `features/{feature-name}/`.
- Do not duplicate API URLs across many files.
- Use a central API client.
- Show loading, empty, success, and error states.
- Apply frontend validation for user experience.
- Do not rely only on frontend validation; backend validation remains mandatory.
- Do not store sensitive tokens in unsafe locations unless the architecture explicitly allows it.

## Example Customer Feature Structure

```text
features/feature1/
├── api/
│   └── Feature1Api.ts
├── components/
│   ├── Feature1Form.tsx
│   └── Feature1StatusBadge.tsx
├── pages/
│   ├── Feature1ListPage.tsx
│   └── Feature1DetailsPage.tsx
└── types.ts
```

## UI Behavior Example

For the entities list page:

- Display entities in a paginated table.
- Provide search by x,y and z.
- Show active and inactive status clearly.
- Provide a button to create a new entity.
- Show a friendly empty state when no entity exist.
- Show validation messages near the related fields.

## Build Command

```bash
npm run build
```
