# [macOS] Two-finger trackpad move triggers unwanted actions on Match-3 board without click

### Description

On the Match-3 level screen, the game sometimes treats a **two-finger
touch/move on the trackpad** as a board action (select/move/swap tiles)
**even without any click/tap**. It can also affect tiles **not under the cursor**
(e.g., cursor is in the bottom-right, but tiles on the left move). This
matters because it can **waste Moves** (limited turns).

---

### Environment

- **Build/Version:** Township 33.0.0 (App Store)
- **Platform:** macOS Sequoia 15.6 (24G84)
- **Device:** MacBook Pro 13", 2560×1600, 8GB RAM, Apple Silicon M2 Pro
- **In-game info:** Town level 13, Match-3 level 24
- **Input:** Built-in trackpad, **two-finger touch/move**
    - Trackpad → Tap to click: ON/OFF tested — **no change**
    - Accessibility → Pointer Control → Trackpad Options → Enable dragging:
      ON/OFF tested — **no change**

---

### Steps to Reproduce

1. Launch Township.
2. Open **Match-3 level screen (game board)**.
3. Move the cursor to the bottom-right area (away from the left side of the
   board).
4. **Do not click/tap** the trackpad.
5. Put **two fingers** on the trackpad and move them left/right/up/down.

**Repro Rate:** 100% (always)

---

### Results

- **Expected Result:**
  Two-finger movement without click/tap should only move the cursor or perform
  a system gesture (e.g., scroll). It should **not** move/swap tiles. Tile
  actions should happen only after a clear user action (click/tap + drag).
- **Actual Result:**
  Two-finger movement **without click/tap** can move/select/swap tiles. It can
  trigger **away from the cursor position**, causing **unwanted moves** and
  wasting **Moves**.

---

### Impact

- **Severity:** Major
- **Priority:** Medium

---

### Notes & Hypothesis

The game likely interprets **two-finger trackpad events** as board input
(drag/scroll) without requiring a click/tap. There may also be an issue with
**input coordinates** (board action not aligned with cursor position).

**Suggested Fixes (optional):**

- [ ] Ignore two-finger movement for board actions unless there is a click/tap.
- [ ] Allow tile actions only when input starts on the tile under the cursor.

---

### Evidence

- Video #1: [Google Drive folder](https://drive.google.com/file/d/1-owc_tU_KAcH4yY3TwPIY4RzHjLO9X0P/view?usp=sharing)
- Video #2: [Google Drive folder](https://drive.google.com/file/d/1CLBlsjnhE5zrKZbcpNq7zQF2f2j_iWNW/view?usp=sharing)
