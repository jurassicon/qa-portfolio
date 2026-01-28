# Battle Arena (console, Python) — Case study (pet project)

**Repo:** https://github.com/jurassicon/Battle_Arena_OOP

## Context
A console duel simulator: fighters of different classes, items, turn-based battles with logs, critical hit chance, a tournament, and a final fight between winners.

## My role
- Built the pet project and performed **manual testing** of logic and edge cases.
- Tested probabilistic mechanics (randomness/crits), calculation correctness, and log readability.
- Verified the tournament flow and the final game state.

## What I tested
### Functional
- Fighter creation and battle start without errors
- Correct damage/defense calculation, HP reduction, battle ends at HP <= 0
- Critical hit conditions and real impact on damage
- Tournament: winners selection → final fight → clean completion

### Exploratory / Balance
- Multiple runs to validate fight pace and outcome variability
- Log output checks at “border” HP values (rounding/precision issues)

## Evidence (issues)
- #1 [Misleading HP value in battle log due to rounding](https://github.com/jurassicon/Battle_Arena_OOP/issues/1)
- #2 [Tournament flow prints “В списке недостаточно элементов - 1” at the end of the final fight](https://github.com/jurassicon/Battle_Arena_OOP/issues/2)
