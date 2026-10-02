# Testing Strategy

## Unit tests

Test calculators, formatters, validation functions and data transformations independently.

## Component tests

Verify loading, empty, error and success states for reusable UI components.

## End-to-end tests

Recommended critical flows:

1. Landing page loads.
2. Navigation reaches major sections.
3. Search/filter interactions work.
4. Interactive calculators produce deterministic results for known inputs.
5. External-data failures show a useful fallback state.

## Quality gates

Before deployment:

- Type-check
- Lint
- Unit tests
- Production build
- Basic accessibility audit
- End-to-end smoke test
