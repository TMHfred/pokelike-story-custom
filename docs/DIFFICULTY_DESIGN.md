# Difficulty System / 難度設定草案

*All percentages below are proposed design targets, not observed Pokelike settings.*

| Preset | Enemy outgoing damage | Enemy maximum HP | XP reward | Recovery |
|---|---:|---:|---:|---|
| Baseline | 100% | 100% | 100% | Unchanged |
| Easy | 80% | 90% | 150% | Full heal after gym |
| Relaxed | 65% | 75% | 200% | Heal 30% of max HP after won battle |
| Custom | 50–150% | 50–150% | 100–300% | User choice |

Implementation rules:
1. Keep source species stats immutable; apply multipliers to derived battle numbers only.
2. Define rounding and minimum damage/HP behavior; add deterministic tests.
3. Document handling of fixed damage, HP-based damage, reflected damage, healing and boss mechanics separately.
4. If game progression uses direct level-up rewards rather than numerical XP, design separate reward knobs; do not blindly multiply number of levels.
5. Snapshot difficulty in each run save, with a clearly described policy for mid-run changes.
6. Prevent accidental save corruption and distinguish local saves from any outside services.
7. Baseline should be labeled “reference candidate” until measured and validated.
