# Plan: profile (duketopceo) → 10/10

**Date:** 2026-09-21 · **Status:** proposed · **Depth:** lightweight
**Origin:** repo scorecard pass — docs & onboarding 5, OSS citizenship 6.

## Problem frame

The profile README is the front door to 63 repos: it already has good plugin tables, but
link rot is the silent killer — repos get archived, renamed, or superseded, and the
tables don't say what's alive. A visitor can't tell in 30 seconds what to try first.

## Scope

**In:** link audit, a "start here" section, a quarterly refresh checklist.
**Out:** redesigns, auto-generated stats widgets that can break (keep it hand-maintained).

## Implementation units

### U1 — Link + status audit
**Files:** `README.md`
- Walk every repo link: drop archived/superseded entries or mark them clearly;
  confirm install commands (`omarchy plugin add …`) still work.
- Add a **Start here** section at the top: 3 repos for a first-time visitor
  (suggested: Argus, orchestral, kurultai — adjust to taste).
**Test scenarios:** n/a — review criterion: every link resolves, every command copy-pastes.

### U2 — Refresh checklist
**Files:** `docs/plans/2026-09-21-001-profile-polish-plan.md` (this file)
- Recurring: re-run U1 quarterly; pin/unpin repos to match what you're actually pushing.
**Test scenarios:** n/a.

## Key decisions

- Hand-maintained over auto-generated: stats cards rot and third-party badge services
  go down; a short, accurate README beats a flashy, stale one.
- The profile sells **three** things, not sixty-three.

## Assumptions / open questions

- Which 3 repos lead? Proposed above; owner's call.
