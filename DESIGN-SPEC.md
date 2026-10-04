# NiveshNyay Design Specification

Clean-room front-end reconstruction based on the publicly visible NiveshNyay experience.

## Visual system
- Warm parchment background, black ink, burnt-orange accent.
- Editorial serif headlines with compact system UI copy.
- Rounded cards, thin borders, restrained shadows.
- Responsive two-column desktop layout collapsing to mobile.

## Components
Navigation, hero, four-step progress, grievance form, privacy note, evidence checklist, editable complaint draft, case tracker, local case log, awareness roadmap, red-flag quiz, official resource cards and sign-in modal.

## Data
Demo cases use localStorage under niveshnyay_cases_v1. Production should use secure authenticated server-side persistence and avoid unnecessary storage of PANs, passwords, OTPs and full account numbers.