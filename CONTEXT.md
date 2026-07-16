# Ponca Language App

Ponca language learning / preservation app. React + Vite frontend; Capacitor wrapping for iOS and Android.

## Status

Migrated from `Projects/Ponca_Language_App/` to `Projects/coding/ponca_language_app/` on 2026-05-14 as part of the `coding/` arm creation. Internal structure (the actual codebase) was preserved as-is — only the path changed. The app does NOT yet follow the standard `planning/ + src/ + docs/ + ops/` template; the existing layout (`src/`, `dist/`, `public/`, `android/`, `ios/`, etc.) is the working app structure. Future refactors can pull planning material into `planning/` and `docs/` subfolders incrementally as those needs surface.

## Tech Stack

- Frontend: React (JSX) + Vite
- Mobile: Capacitor (iOS + Android wrappers)
- Source files: `ponca-language-app.jsx`, `stress-disambiguator.jsx`
- Build output: `dist/`, `ponca-app-dist.zip`
- Reference content: `Dictionary of the Ponca People - Louis Headman & Sean O'Neill.epub`, `HTML Ponca Dictionary.html`, `ponca_qc_check.xlsx`, `Ponca Logo.png`

## Commands

Verify against `package.json` scripts before relying on these — they reflect last-known state at migration time:

| Action | Command |
|---|---|
| Dev server | `npm run dev` (Vite) |
| Build | `npm run build` |
| iOS sync | `npx cap sync ios` |
| Android sync | `npx cap sync android` |

## Current State

Pre-migration state preserved. No code or asset changes were made during the migration. Open work items live with the project itself (no formal tracker yet — to be documented as work resumes).

## Note on Structure

This app pre-dates the `coding/` arm's standard layout. Rather than force a refactor at migration time, the existing structure is preserved (lower risk; the working app keeps working). As future work surfaces a need (real PRD, decision log, deployment scripts), `planning/`, `docs/`, and `ops/` folders can be added incrementally. See `../CONTEXT.md` for the standard arm-level shape.

## Git

The app retains its own `.git/` directory. It is independently tracked from the Projects MWP git history (if any). Path change from the migration is transparent to git — all internal references are relative.
