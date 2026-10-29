# Story-mode Feature Audit (working matrix)

Status labels: **candidate** (appears in reference), **unverified** (needs evidence), **to design** (planned locally). No code or behavior has been validated in this repository.

| Area | Expected functionality | Current evidence/status | Audit task |
|---|---|---|---|
| Regions | Region-specific Story campaigns | Unverified for exact current official version | Confirm each region/version |
| Routes | Branching maps, nodes, trainers, wild encounters, recovery, items, exchanges, random events | Candidate from reference descriptions | Record node rules, probabilities, eligibility |
| Gym/League | Gym leaders, Elite Four, champion teams | Candidate | Capture versioned enemy rosters and mechanics without copying protected datasets |
| Species | Stats, type chart, evolution branches | Candidate | Verify licensing/source of any reusable datasets |
| Moves | Physical/special, power, status, priority, move tier | Unverified | Enumerate required semantics and test cases |
| Abilities | Passive triggers and status interactions | Unverified | Establish trigger lifecycle |
| Equipment | Held items and their restrictions | Unverified | Verify effect stacks, ordering, caps |
| Battle | Automatic actions, damage modifiers, immunity, statuses | Unverified across versions | Separate battle engine tests from UI |
| Progress | Level, XP, party changes, evolution | Candidate | Validate progression and persistence |
| Save | Start/resume/export/import | To design independently | Create own schema/versioning |
| Difficulty | Baseline/easy/relaxed/custom | To design | Define precise mathematical behavior |
| Localization | Traditional Chinese | To design | Establish strings and responsive layouts |

## Candidate external references — rights NOT established
- https://pokelike.xyz/
- https://github.com/pcasaspere/pokelike_v2

## Required evidence for each confirmed feature
Source URL/file + revision/date; exact behavior; confidence; cases that contradict; whether legally reusable. Avoid “100% identical” assertions without side-by-side runtime verification.
