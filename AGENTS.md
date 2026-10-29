# Codex Agent Instructions

## Mission
Research and eventually build an independently controlled Story-mode browser game with adjustable difficulty, using Pokelike only as a functional reference where lawful.

## Hard constraints
- Do not copy/import official or third-party game source, data dumps, sprites, names, sounds, or art without documented rights/permission.
- Do not touch official accounts, cloud saves, leaderboards, or endpoints.
- Do not publish/deploy or make this repository public/private through automation.
- First task is **audit only**, not game development. No dependency installation or arbitrary execution of untrusted code before review.
- Work in small, reviewable changes, preferably feature branches and PRs. Do not overwrite main or force-push.
- Record each finding with source URL, observed revision/date, evidence and confidence level; distinguish implemented, partial, missing, unknown.
- Never represent unverified behavior as identical to official.
- Prefer clean-room implementation with original/authorized assets where reuse permission is absent.

## Technical direction (after audit)
- Web-first (desktop + iPhone Safari), Traditional Chinese support.
- Separate immutable data, battle engine, map/events, difficulty layer, UI and local save.
- Deterministic seeded tests for battle and route generation.
- Distinct storage namespace, schema version, export/import/rollback.
- Difficulty presets adjust enemy damage, max HP, earned XP or explicit level-up rewards, and post-battle healing. Avoid directly modifying canonical species stats.
- Ensure difficulty changes cannot corrupt existing saves.

## First deliverables
1. License/rights audit.
2. Candidate architecture and version gap matrix.
3. Story-mode feature inventory by region.
4. Risk log and implementable roadmap.
5. Explicit list of unknowns and required user input.
Stop after audit; no gameplay code or deployment until reviewed.
