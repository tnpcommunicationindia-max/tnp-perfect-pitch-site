# TNP Perfect Pitch — "Pitch Town" Brand & Content Brief
*Reference document for building the microsite. Upload this alongside the poster PNGs and the deck.*

---

## 1. Event facts

- **Event:** TNP Perfect Pitch — an internal Shark Tank–style pitch competition
- **Date:** 16 September 2026
- **Registration deadline:** TBD — placeholder only, do not invent a date
- **Team size:** 1–3 employees, cross-department teams encouraged, open to all TNP India employees
- **Idea/theme:** Completely open — any product, service, or business idea
- **Pitch time:** 5 minutes live, strictly timed, visible countdown
- **Q&A time:** 5–7 minutes of investor-style questioning on market, numbers, differentiation, execution
- **Prize pool:** 1st ₹30,000 · 2nd ₹15,000 · 3rd ₹5,000
- **Scoring:** Final Score = (Judge points ÷ 200 × 70) + (Investment received ÷ ₹4,00,000 total pool × 30). 70% presentation score (judges' scorecard), 30% investment score (gold coins physically placed in a jar). Highest score wins; tie-break is higher total investment.
- **Office scope:** not yet confirmed — Kochi only, or all three offices (Kochi/Bangalore/Delhi). Do not assume.

## 2. The world: "Pitch Town"

**Confirmed direction: bright daytime side-scroller**, not the earlier dark "Night Arcade" concept. TNP's dark brand equity is preserved through outline color and the lime-on-dark rule below, not through a dark sky.

**Sky:** deep cobalt-violet `#4B4FE6` at the top, fading to lavender `#7E8FFF` at the horizon.

**Hard rule — outlines:** every sprite, tile, and building uses `#080B12` (TNP's primary black) as its outline color. This is how TNP's core brand color stays structurally present throughout a bright-daylight world.

**Hard rule — lime placement:** `#39FF6A` (Electric Lime) must never sit directly on the purple sky — it goes muddy. Lime only ever appears on a `#080B12` (near-black) surface: buttons, HUD accents, CTAs. This single rule is what keeps the bright world recognisably TNP.

### Palette
| Color | Hex | Role |
|---|---|---|
| Sky deep | `#4B4FE6` | Sky top |
| Sky light | `#7E8FFF` | Sky horizon |
| TNP purple | `#878FFF` | Buildings, skyline, mid-ground |
| Teal | `#36E6E4` | Window glow, UI panels, secondary accents |
| Coral | `#FF6B6B` | Timers, urgency, deadline states |
| Coin gold | `#FFC93C` | Coins ONLY — never used elsewhere |
| Electric lime | `#39FF6A` | CTAs and buttons, always on `#080B12` only |
| Cream | `#F5F2EC` | Body text, character highlights |
| Void black | `#080B12` | All outlines, all button/panel backgrounds behind lime text |

**Progression device (optional, not yet built):** the world can darken toward dusk as the site approaches the Final Bosses / registration scenes, giving a natural "raising stakes" arc without abandoning the bright opening. Not required for v1 — flag as a stretch goal.

## 3. Typography

- **Display/headlines only:** Press Start 2P (Google Fonts) — never for body copy
- **HUD/labels/timers:** VT323 (Google Fonts)
- **Body copy:** TNP's existing sans-serif, unchanged, always plain case, never pixel font
- **Rule:** pixel type for headlines, plain sans for anything longer than a few words. This is the single most important readability rule in the whole system.

## 4. Characters

**PIP** (the player) — lime green cap over green hair, purple vest and backpack, coral orange trousers, cream face. Three-heads-tall 8-bit sprite proportions.

**P2** — teal cap over dark hair, coral orange jacket, cream trousers.

**P3** — purple beanie, gold yellow jacket, teal trousers.

**The Final Bosses** — four generic, fictional, non-humanoid creature designs, all appearing together in `bg-final-bosses.png`. No individual names or titles beyond their position (no "Market Boss" / "Numbers Boss" naming), no real photographs or likenesses of actual judges under any circumstance. Purely illustrative, stylised, game-boss characters — treat them as a set, not as four separately named entities.

## 5. Naming system

| Real thing | Site language |
|---|---|
| Registration | Insert Name / Player Select |
| Team (1–3 people) | P1 · P1–P2 · P1–P2–P3 |
| The idea | Your Run |
| 5-minute pitch | Level 01 — The Pitch |
| Q&A | The Boss Fight |
| External judges | The Final Bosses (four creatures, shown as a set) |
| Prize pool | The Coin Pool |
| Coin jar | The Vault |
| Scoring | High Score Table |
| Registration deadline | Lobby Closing |

## 6. Voice

Two registers, never mixed in the same sentence:
- **HUD voice:** all caps, ≤6 words, imperative. `PRESS START TO PITCH.` `NO CONTINUES.`
- **Briefing voice:** normal professional English for actual rules, dates, eligibility. No gaming metaphor here — people need to understand it, not just enjoy it.

**Master line (confirmed):** `PRESS START TO PITCH`
**Recurring sub-line:** `Five minutes. No continues.`

## 7. Recurring visual devices

- **Dialogue box:** rounded rectangle, 2px stroke (lime or cream depending on background), transparent fill. Universal content container.
- **HUD bar:** thin strip at the top of scenes showing player state / date / status.
- **Brick strip:** alternating coral/gold brick tiles as a ground plane and section divider — the series' visual signature.
- **Coin sprite:** small gold circle, hard black outline, used for the Vault, celebration moments, and any "reward" beat.
- **Pixel cursor arrow:** chunky pointer, used sparingly as an annotation device.

## 8. Site assets (final — all generated, use these filenames exactly)

All backgrounds are 16:9, pure scenery with no baked-in text, logos, or UI — all copy is added separately in code.

| Filename | Contains | Used in scene |
|---|---|---|
| `bg-loading.png` | Empty morning street, glowing arcade cabinet | 0 — Loading |
| `bg-what-is-this.png` | Empty street corner, awning, coin jar, skyline | 1 — What is this? |
| `bg-how-to-play.png` | Four ascending brick platforms, flag, no characters | 2 — How to Play |
| `bg-gather-squad.png` | PIP + P2 + P3 together, coin stacks, jar | 3 — Gather Your Squad |
| `bg-final-bosses.png` | Four fictional creature bosses, dusk stage lighting | 4 — Final Bosses |
| `bg-how-you-win.png` | Large glass jar, partially filled, skyline | 5 — How You Win |
| `bg-register.png` | Calm street, glowing arcade cabinet, no characters | 6 — Register |
| `pip-walk-sheet.png` | PIP walk-cycle, 4 frames, transparent background | Persistent character layer, all scenes |
| `coin-spin-sheet.png` | Single coin spin cycle, 4 frames, transparent background | Vault animation, celebration beats |

**Note:** the PIP asset is assumed to be `pip-walk-sheet.png` (a 4-frame walk cycle) rather than a single static idle pose. If a static pose was generated instead, use a CSS sway/bounce animation rather than a stepped walk-cycle.

## 9. Legacy print assets (not used for the site build)

| Asset | Original purpose |
|---|---|
| Poster 01–05 (A4 print set) | Print/physical rollout only — different aspect ratio and has baked-in text, not suitable for site backgrounds |
| Deck (PowerPoint) | Reference for exact copy/numbers, especially the scoring explainer in "How You Win" |

Keep these in the Project for consistency reference, but the build should pull visuals from Section 8, not from the posters.

## 10. Confirmed technical/scope decisions

- **No Microsoft Forms embed of any kind.** The final scene contains a single button/link ("Register") that opens the Microsoft Form in a new tab. The form itself is being built separately and manually — do not attempt to build, design, or embed a form.
- **Mobile:** below 768px width, the site switches from horizontal scroll-hijacking to a normal vertical stacked layout, same content and art, top to bottom instead of left to right. This is a hard requirement, not optional polish.
- **Hosting:** the finished site must be plain HTML/CSS/JS with no build step and no framework, so it runs by opening `index.html` directly and can be dragged as a folder into Netlify Drop (app.netlify.com/drop) for free static hosting.
- **PIP's animation should loop continuously**, not be tied precisely to scroll position — precision scroll-to-frame binding is fragile across devices and input types.

## 11. Scene map

| # | Scene | Content |
|---|---|---|
| 0 | Loading | "LOADING TNP PERFECT PITCH..." pixel progress bar |
| 1 | What is this? | One-paragraph hook: Shark-Tank-style internal pitch competition, 16 September |
| 2 | How to Play | Four numbered steps: Build your squad → Load your idea → Level 01: The Pitch → The Boss Fight |
| 3 | Gather Your Squad | Team size 1–3, cross-department encouraged, eligibility |
| 4 | Final Bosses | What the Q&A actually covers — market, numbers, differentiation, execution. Four boss creatures shown together as a set, no likeness |
| 5 | How You Win | 70/30 scoring split, the Vault visual, prize amounts |
| 6 | Register | Single CTA button linking out to the Microsoft Form (new tab). No embed. |

## 12. Outstanding items — do not assume, ask if needed

- Exact registration deadline
- Whether this is Kochi-only or all three TNP offices
- The final Microsoft Form URL (will be supplied once built)
- Confirm whether `pip-walk-sheet.png` is a 4-frame walk-cycle or a single static pose (see note in Section 8) — ask before building the animation if this isn't clear from the file itself
