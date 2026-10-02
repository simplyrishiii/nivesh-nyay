# Architecture Blueprint

```text
Browser
  |
  v
Frontend UI
  |
  +--> Static/reference data
  |
  +--> Service layer
          |
          +--> External APIs
          +--> Authoritative public data
          +--> Optional backend
                    |
                    +--> Validation
                    +--> Caching
                    +--> Logging
```

## Frontend

Use reusable components and route-level pages. Keep presentation logic separate from data-access logic.

## Service layer

External requests should be wrapped in small adapters. Each adapter should validate response data, handle timeouts/errors and expose a stable internal interface.

## Data

Static educational content can live in version-controlled JSON/Markdown files. Dynamic financial data should not be hard-coded into the UI.

## Security

- Never commit API keys or credentials.
- Use environment variables for secrets.
- Validate user input at trust boundaries.
- Sanitize externally supplied content before rendering it as HTML.
- Apply rate limits when a backend/API layer is introduced.

## Deployment

The existing public prototype uses Netlify. The same frontend architecture can also be deployed to Vercel or another static/edge hosting provider.
