## Title

[macOS] Two-finger trackpad scroll triggers unintended click near cursor on
Players list screen

### Description

On the Players list screen (team/co-op UI), doing a **two-finger scroll on the
trackpad** can trigger an **unwanted click/action** even when I scroll **away
from the list items**. The action happens **left of the mouse cursor**, as if
the click position is shifted. This can open player profiles or select items by
mistake.

---

### Environment

- **Build/Version:** Township 33.0.0 (App Store)
- **Platform:** macOS Sequoia 15.6 (24G84)
- **Device:** MacBook Pro 13", 2560×1600, 8GB RAM, Apple Silicon M2 Pro
- **Input:** Built-in trackpad, **two-finger scroll**
    - Trackpad -> Tap to click: ON/OFF tested — **no change**
    - Accessibility -> Pointer Control -> Trackpad Options -> Enable dragging:
      ON/OFF tested — **no change**
    - Mouse is working properly. Tested on Apple Magic Mouse 2.

---

### Steps to Reproduce

1. Launch Township.
2. Open the **team/co-op screen** and go to the **Players list**.
3. Move the mouse cursor to the right side (away from the list items).
4. Use **two fingers** on the trackpad to scroll (no click/tap).
5. Watch the left side near the list and the cursor area.

**Repro Rate:** 100%(always)

---

### Results

- **Expected Result:**
  Two-finger scrolling should only scroll the list. It should **not** select
  items or open player profiles unless I click.
- **Actual Result:**
  Two-finger scrolling can trigger an **unintended click/action** near the
  cursor, often **left of the cursor position**, causing wrong selection or
  opening a profile.

---

### 🟡 Impact

- **Severity:** Minor
- **Priority:** Medium

---

### Notes & Hypothesis

This looks like wrong handling of **two-finger trackpad events** on macOS (
scroll/gesture treated as click/drag) and/or **input coordinate offset** (
action happens left of cursor).
**Possible related issue:** similar trackpad bug on Match-3 board (two-finger
movement triggers actions without click).

**Suggested Fixes (optional):**

- [ ] Do not trigger any click/select actions from scroll events.
- [ ] Make sure click/selection uses correct cursor coordinates.
- [ ] Separate scroll gestures from gameplay/UI actions.

---

### Attachments

- Video with visible click indicator (circle): [add link here]
