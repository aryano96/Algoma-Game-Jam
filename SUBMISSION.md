# Submission checklist: ThunderHacks 2026 Algoma Game Jam ("Four Seasons")

**Deadline: Friday, October 16, 12:00 PM.**

## Deliverables in the brief

| # | Deliverable | Status |
|---|---|---|
| 1 | Playable build, demonstrated live and playable by judges | Done: `index.html`, which runs offline in any browser. Play link: https://raw.githack.com/aryano96/Algoma-Game-Jam/main/index.html (backup: https://claude.ai/artifact/FnPmHve9MJkY951WdRUGky). |
| 2 | Pitch of up to 5 minutes, then 3 minutes of questions | Script ready in `PITCH.md`. **Your team needs to rehearse it.** |
| 3 | Link to the code or project repository | Done: https://github.com/aryano96/Algoma-Game-Jam (paste this link into the submission form). |
| 4 | List of third-party assets, tools and libraries, with credit | Done: see "Third-party assets, tools and libraries" in `README.md` (no third-party assets are used). |
| 5 | Submit by Fri Oct 16, 12:00 PM | **You need to do this:** submit on the event's portal with team names. |

## Solution requirements

| Requirement | How Perennial meets it |
|---|---|
| 01 Playable loop | Clear goal (survive 3 winters), lose condition (health reaches 0 from heat, cold, wolves or hunger), score (tree rings), and a full start-to-finish flow with title, play, pause, win and lose screens, plus an endless mode. |
| 02 Theme in mechanics | Each season has its own rules: planting only in spring, heat and watering in summer, wind and harvest in fall, dark, cold, fire and wolves in winter. |
| 03 Consistent art and audio | One flat "paper diorama" style drawn in code. Each season has its own palette and generated music in one shared instrument family. |
| 04 Runs on site | A single self-contained HTML file with no network, install or build step. Playtested in headless Chromium with zero console errors. A bot completed 9 full games. |

## Bonus considerations

| Bonus | Covered by |
|---|---|
| 1. All four seasons play differently | See the season table in `README.md` |
| 2. Season changes are gameplay | Sprouts become trees, fruit rots, the ice cracks and dumps you in, dusk falls, a countdown ticks |
| 3. Art and audio made during the event | All of it is drawn and synthesized in code |
| 4. Accessibility | Remappable controls, colour-blind palette, 3 difficulties, hint levels, reduce motion, volume sliders, gamepad and touch |
| 5. Tutorial without text | First year teaches through picture bubbles, arrows, keycaps and picture rule banners |

## Rubric self-check (100)

- **Theme (25):** the seasons are the rules, not a backdrop.
- **Gameplay and fun (30):** a 2 to 3 minute year, a tense first winter, and a clear "one more year" pull.
- **Art and audio (20):** one style, four palettes, generated per-season music.
- **Playable build (15):** one file that runs offline.
- **Originality (10):** the tree is shade, then food, then fuel, and the winter choice decides your next year. The sun jar lets you bottle summer and spend it in winter.

## Before judging

1. Open `index.html` in Chrome on the demo laptop. Press F11 for full screen and turn the volume up.
2. Leave difficulty on **Normal** and hints on **First year** so judges get the wordless tutorial.
3. If a judge struggles, open Options and switch to **Gentle**. The settings save in the browser.
