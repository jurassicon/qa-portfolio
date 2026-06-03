# QA Portfolio — Iurii Cherkasov

<p align='center'>
  <img
    src='https://github.com/user-attachments/assets/d163acbf-6bd6-4c8b-839c-c7200ba3f70e'
    alt='teenage mutant ninja turtles'
    width='640'
  >
</p>

Manual QA portfolio focused on game testing: gameplay mechanics, input handling,
edge cases, state transitions, and clear reproducible bug reports.

---

## Featured: Commercial Game Testing

### Township / macOS

Real bug reports filed against Township (Playrix, App Store) on macOS.

**1. [macOS] Match-3 board: two-finger trackpad move triggers unwanted tile actions**

- Report: [artifacts/playrix_bug_reports/township_trackpad_bug.md](artifacts/playrix_bug_reports/township_trackpad_bug.md)
- Severity: **Major** | Priority: **Medium**
- Evidence: video + screenshots ([Google Drive folder](https://drive.google.com/drive/folders/1lftEX8dvyhtiedwHCbNfNVEJBhI5lSJK?usp=sharing))
- Input bug can waste limited Moves during gameplay.

**2. [macOS] Players list: two-finger trackpad scroll triggers unintended click near cursor**

- Report: [artifacts/playrix_bug_reports/township_players_list_trackpad_bug.md](artifacts/playrix_bug_reports/township_players_list_trackpad_bug.md)
- Severity: **Minor** | Priority: **Medium**
- Evidence: video with click indicator ([Google Drive](https://drive.google.com/file/d/1cLJ5B4wVXIlpXBhykcRPwVWGCEyNJbmA/view?usp=sharing))
- UI input bug can open wrong player profiles or select wrong items.

---

## Additional Game QA Practice

### The Snake — Python/Pygame

Self-built training project from Yandex Practicum, tested manually as a game QA case.
Focus: gameplay logic, state transitions, input stress, edge cases.

- Case: [projects/the_snake.md](projects/the_snake.md)
- Repo: https://github.com/jurassicon/the_snake
- Issues:
  - [#18 False Game Over after chaotic arrow input (Snake length 3)](https://github.com/jurassicon/the_snake/issues/18)
  - [#19 Apple sometimes spawns directly in front of the snake's head after respawn](https://github.com/jurassicon/the_snake/issues/19)

### Battle Arena — Python console game

Self-built training project from Yandex Practicum student hackathon practice, tested manually as a QA case.
Focus: combat logic, randomness, tournament flow, logs, edge cases.

- Case: [projects/battle_arena.md](projects/battle_arena.md)
- Repo: https://github.com/jurassicon/Battle_Arena_OOP
- Issues:
  - [#1 Misleading HP value in battle log due to rounding](https://github.com/jurassicon/Battle_Arena_OOP/issues/1)
  - [#2 Tournament flow prints "В списке недостаточно элементов - 1" at the end of the final fight](https://github.com/jurassicon/Battle_Arena_OOP/issues/2)

---

## Artifacts

- [Bug reports index](artifacts/bug_reports.md)
- [Checklists](artifacts/checklists.md)
- [Bug report template](templates/bug_report_template.md)

---

## Skills Demonstrated

- Manual testing
- Functional testing
- Smoke testing
- Regression thinking
- Exploratory testing
- Gameplay logic testing
- Input stress testing
- Edge-case analysis
- Bug reporting with steps, expected/actual result, severity/priority, and evidence
