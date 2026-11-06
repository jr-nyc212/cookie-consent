# PROGRESS — Cookie Consent

Updated: 2026-11-06 — Handoff before the assistant switches from Claude Code to GitHub
Copilot. Setup scope shipped 2026-10-27 (issue #1, PR #2). No lesson code written since.

## Start here

Read `CLAUDE.md` for the working rules, then jump to **Current milestone**.
Shipped work is in `HISTORY.md`. The lesson starter is `index.html`, `index.css`,
`index.js`; the Scrimba scrim is linked from `package.json`.

## North Star

A Scrimba solo project: a satirical "We ❤️ Your Data" cookie-consent modal that appears
over a landing page, collects a name and email, fakes an upload, then taunts the user.
It demonstrates DOM manipulation, form handling, `setTimeout`, and modal positioning,
published lesson by lesson through GitHub issues and PRs.

## Roadmap

- [>] M1 — Core: the modal behaves as in the scrim (positioned, timed, form, loading
  state, close and choice buttons).
- [ ] M2 — Accessibility and responsive pass: semantic headings, `alt` text, rem units,
  layout that works below 400px, contrast.
- [ ] M3 — Polish: portfolio README (`/scrimba-readme`), Netlify deploy.

## Current milestone — M1 Core

**Definition of done:** opening the Vite dev server shows the landing page, the modal
appears centred over it after a short delay, submitting a name and email shows a loading
state then a personalised message, and the close button becomes usable. Matches the scrim.

**Scopes (hill status)**

- setup — git repo, GitHub repo, Vite, head metadata (doctype, lang, charset, viewport,
  title) — done
- modal-css — the challenge comment in `index.css` under `.modal`: sit on top of the page,
  centre horizontally and vertically, then `display: none` — uphill
- modal-js — `index.js` is empty. Reveal the modal after a delay, add the name/email form,
  handle submit with a loading state then a thanks message, enable the close button,
  accept/decline buttons — uphill (exact steps follow the scrim's lesson order)

**Next unit of work:** modal-css. Start with `/github-flow` to open the issue and branch.

## Standing items

- Each lesson is published as issue → branch → commit → push → PR "Closes #N" → merge.
  `/github-flow` prints the commands for the step you are on.
- Verify visual changes with screenshots of the Vite site before and after.

## Backlog / Icebox

- Replace the boilerplate `docs/design/README.md` (it is copied from a different project
  and talks about posts and avatars).
- `img` in `index.html` has no `alt`; `h3` follows `h1` with no `h2` in between. Both
  belong to M2 unless a lesson touches them first.

## Blockers / risks

- No screenshot of the Scrimba design yet. `docs/design/` holds only starter assets.
  Screenshot the scrim's mini-browser into `docs/design/` before modal-css.

## Decisions & findings

- From 2026-11-08 the assistant is GitHub Copilot in VS Code. It reads `CLAUDE.md` and
  `.claude/skills/` natively, so the working rules and `/github-flow` carry over. The
  memory-sync and transcript-sync scripts in `ops-session-handoff` target Claude Code's
  local store and are inert under Copilot; the PROGRESS/HISTORY reconcile still applies.
