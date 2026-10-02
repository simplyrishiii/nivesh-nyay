# Nivesh Nyay

Nivesh Nyay is a web-based investor-awareness and financial-information project.

**Live prototype:** https://niveshnyay.netlify.app/

> This repository currently contains a documentation and implementation boilerplate. It is intentionally not presented as a reconstruction of the original deployed source code.

## Project goals

- Make investor-oriented information easier to understand.
- Organize educational resources and financial concepts clearly.
- Provide a foundation for structured decision-support features.
- Keep financial education separate from personalised financial advice.
- Provide a maintainable foundation for future frontend/API development.

## Suggested structure

```text
nivesh-nyay/
├── docs/              # Product, UX, architecture and API documentation
├── public/             # Static assets
├── src/
│   ├── components/    # Reusable UI components
│   ├── pages/         # Application pages/routes
│   ├── data/          # Reference/static datasets
│   ├── services/      # API and external-service adapters
│   └── utils/         # Shared utilities
├── tests/             # Unit and end-to-end tests
├── .env.example       # Non-secret environment-variable template
└── README.md
```

## Recommended implementation stack

- React + Vite or Next.js
- TypeScript
- Tailwind CSS or another accessible component system
- REST/JSON APIs for external data
- Vitest/Jest for unit tests
- Playwright for end-to-end tests
- Netlify or Vercel for deployment

## Important

The public deployment does not provide the original repository's complete source tree. The files in this repository should therefore be treated as a practical project scaffold and documentation layer, not as a claim that every implementation detail matches the original application.

Financial information can change. Verify important information against authoritative sources before relying on it for an investment decision.
