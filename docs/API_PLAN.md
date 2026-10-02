# API Integration Plan

The application should treat external data providers as replaceable integrations.

## Recommended pattern

```text
UI -> service function -> provider adapter -> API
                         |
                         +-> validation
                         +-> normalization
                         +-> cache/error handling
```

## Rules

- Keep provider-specific URLs and response formats out of UI components.
- Normalize responses into application-owned types.
- Cache data where freshness requirements permit.
- Display the timestamp/source for dynamic information.
- Fail gracefully when an external provider is unavailable.
- Do not expose private credentials in browser code.

## Example service boundaries

```text
services/
├── marketData.ts
├── education.ts
├── disclosures.ts
└── resources.ts
```

These are proposed boundaries, not claims about the implementation of the deployed prototype.
