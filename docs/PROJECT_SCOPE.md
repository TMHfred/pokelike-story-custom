# Project Scope / 專案範圍

## Intended result
An independent Story-mode browser game with selectable difficulty and Traditional Chinese UI, designed around the kinds of route choices, team progression, auto-battles, gyms, and league challenges the user enjoys.

## User-requested parity targets (subject to rights and verification)
- Region story campaigns, starters, map branches, trainer/wild encounters, events, gyms, Elite Four and Champions
- Species stats, types, evolutions, moves, abilities, items, held equipment
- Automatic battle, level progression, capture, party management
- Run continuation and local-save backup/restore
- Easy / Relaxed / Custom difficulty in addition to a verified baseline

## Non-goals for initial delivery
- Battle Tower, endless, daily/weekly challenges, competitive online modes
- Connecting to official Pokelike services or editing official saves
- Rehosting unauthorized copyrighted source or art

## Phases
0. Rights/source review and detailed gap audit (no code).
1. One-region vertical slice using a clean-room engine and authorized assets.
2. Difficulty integration and deterministic test harness.
3. Additional regions and complete Story features.
4. Mobile UI, localization, save migration and full regression tests.

## Acceptance checks
- Can start, save, reload, follow branches, encounter events, battle, level, evolve, equip and finish a region.
- Separate seeded tests cover damage, types, statuses, ability/item triggers, win/loss, route connectivity.
- Switching difficulty changes only specified parameters and does not mutate species reference data.
- No third-party materials without permission, no access to official accounts and no deployment without review.
