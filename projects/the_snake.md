# projects/the_snake.md

# The Snake (Python/Pygame) — Case study (project work)

**Repo:** https://github.com/jurassicon/the_snake

## Context
Classic “Snake”: grid movement, eating apples, growth, and Game Over on self-collision.  
Additional: wrap-around (leaving the field → appearing on the opposite side) and a Game Over sound.

## My role
- Built the training project and performed **manual testing** of mechanics and state transitions.
- Prepared core-loop checks and small checklists.
- Reported bugs in GitHub Issues (steps, expected/actual, severity/priority, video).

## What I tested
### Smoke (2–5 min)
- Game starts without errors
- Snake movement works
- Arrow-key controls work
- Apple spawns
- Eating apple increases length
- Self-collision triggers Game Over (text/sound)

### Functional
- Controls work in all states (normal play, after respawn, after eating)
- Wrap-around works on all 4 borders
- “Eat” happens only when head coordinates match apple coordinates
- Apple never spawns on the snake (head/body)

### Exploratory
- Input spam (chaotic arrow presses)
- Edge checks near borders
- Long sessions (10–15 minutes)

## Evidence (issues)
- #18 [False Game Over after chaotic arrow input (Snake length 3)](https://github.com/jurassicon/the_snake/issues/18)
- #19 [Apple sometimes spawns directly in front of the snake’s head after respawn](https://github.com/jurassicon/the_snake/issues/19)
