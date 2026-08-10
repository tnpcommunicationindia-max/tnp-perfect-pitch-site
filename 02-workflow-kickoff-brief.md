# Workflow brief — paste this as your first message in the Project chat

Read the uploaded brand and content brief, the nine site asset PNGs (the `bg-*.png` backgrounds, `pip-walk-sheet.png`, and `coin-spin-sheet.png`), the legacy poster PNGs, and the deck fully before doing anything else. Confirm you've reviewed all of them before proceeding. The `bg-*.png` files are what you build the scenes from — the poster PNGs are print reference only, not site material.

We are building a horizontal-scroll pixel-art microsite for "TNP Perfect Pitch," inspired by band5051.com's structure (full-bleed parallax scenes, a scroll-driven journey, a persistent character). All content, copy, palette, naming, and scoping decisions are in the brand brief — follow it exactly. Do not invent facts, dates, or copy that aren't in the brief.

## Hard rules for this build

1. **Plain HTML/CSS/JS only.** No React, no build tools, no npm dependencies. The site must run by opening `index.html` directly in a browser and must be draggable as a folder straight into Netlify Drop.
2. **No Microsoft Forms embedding of any kind.** The final scene is a single button/link that opens the Microsoft Form in a new tab. Do not design, mock up, or attempt to embed a form.
3. **Mobile fallback is mandatory.** Below 768px width, switch from horizontal scroll-hijacking to a normal vertical stacked layout — same content and art, top to bottom. Build and verify this alongside the desktop version, not as an afterthought.
4. **PIP's animation loops continuously**, independent of scroll speed or position. `pip-walk-sheet.png` is a 4-frame walk-cycle sprite sheet — cycle it with a CSS `steps()` animation on a fixed timer, not bound to scroll position. If this file turns out to be a single static pose instead, ask before building — don't guess which one it is.
5. **Use the uploaded image assets for anything that's genuine pixel art** — all seven `bg-*.png` backgrounds, PIP, the coin sprite, and the four boss creatures in `bg-final-bosses.png` (treat them as one set, not four separately named characters). Do not attempt to hand-draw detailed pixel art in CSS or SVG. Code is for structure, layout, scroll mechanics, and UI chrome (buttons, HUD bar, dialogue boxes) — not for illustration.

## Process rules — follow these strictly

- **Build in phases. Never build more than one phase per response.** The phases are: (1) the skeleton, (2) Scene 1, (3) Scene 2, (4) Scene 3, (5) Scene 4, (6) Scene 5, (7) Scene 6, (8) final assembly.
- **After completing each phase, stop and explicitly ask for approval before starting the next phase.** Do not proceed automatically. End your response with a direct question such as "Approved to move to the next phase, or would you like changes first?"
- **Before building each phase, ask any clarifying questions you need — do not assume.** In particular: if the brief doesn't specify whether an image asset exists for something you're about to build, ask whether one will be supplied or whether you should build a simplified code-only version instead. If a decision in the brief is marked "open" or "not yet decided," ask rather than picking one.
- **Reference the previous phase's actual output when building the next one** — match its CSS variables, HUD bar, and style system exactly rather than re-deriving colors or fonts from scratch.
- **Once a phase is approved, write it to real files** (not just the live preview) so it can be downloaded. Confirm the file paths you've created.

## Phase 1 — start here

Build only the skeleton: the CSS color variables from the brief's palette table, the pixel grid unit, the Press Start 2P and VT323 font imports, and the scroll-container mechanism (horizontal scroll-hijacking above 768px, vertical stacking below it). Include six placeholder boxes labeled for the six scenes, with no real content yet, so the scroll behavior itself can be reviewed and approved first.

Before you start this phase, ask me anything you're unsure of.
