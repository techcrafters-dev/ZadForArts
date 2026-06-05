# Zad for Arts — زاد الفنون · Design System

A brand & UI design system for **Zad for Arts (زاد الفنون)**, a non-profit
performing-arts organization in Jordan supporting **theater, music, and dance**.
This system powers the organization's bilingual (Arabic / English) website and
related cultural communications.

> **Vibe in one line:** A bright, gallery-clean cultural institution — premium,
> emotionally resonant, purple-led, always on white.

---

## 1. Company & Product Context

**Zad for Arts** (literally "provisions / nourishment of the arts") is a Jordanian
non-profit that nurtures the performing arts community — producing and platforming
**theater, music, and dance**. The public face of the organization is its
**bilingual website**, which is the primary product this design system serves.

**Website surfaces (information architecture):**
- **Hero** — emotive opening statement of mission
- **Who We Are** — about / mission / story
- **Programs** — the three pillars: **Theater · Music · Dance**
- **Events** — upcoming performances, workshops, showcases
- **Support Us / Join Our Friends** — donation & membership / community

**Audience:** artists, audiences, cultural patrons, donors, and the broader
Jordanian and Arabic-speaking arts community. Bilingual Arabic-first with full
RTL support, plus English.

### Sources used to build this system
- **Provided brand brief** (palette, typography intent, IA, tone) — the
  authoritative source for this system.
- **Logo files:** `ZAD_Logo_(Feb_18_2025)-01-white.png`,
  `ZAD_Logo_(Feb_18_2025)-02-black.png` (in `assets/`).
- **Provided font:** Cairo variable font (`fonts/Cairo-Variable.ttf`).
- **GitHub repo:** `techcrafters-dev/ZadForArts`
  (https://github.com/techcrafters-dev/ZadForArts) — *"Digital assets, pages, and
  design resources for Zad for Arts."* **At the time of building this system the
  repository was empty (no commits / no files reachable).** Once the team pushes
  the real site code and assets, a future pass should pull components,
  copywriting, and real imagery directly from this repo to raise fidelity. The
  reader is encouraged to explore it for source-of-truth material as it fills in.

> ⚠️ **Caveats / substitutions** (see also bottom of file):
> - No production code or live screens were available, so the **website UI kit is
>   built from the described IA and brand brief**, not reverse-engineered from
>   shipped code. Treat it as a faithful brand-accurate proposal, not a 1:1 mirror.
> - The **typography is Cairo only** (the provided variable font), used for both
>   Arabic and English, display through body. No serif. Headlines are heavy Cairo
>   weights (700–800); body is Cairo 400.
> - The logo contains a small **teal diamond** accent (the "O" in *FOR*) not named
>   in the brief's palette. It's captured here as a rare flourish (`--teal`).

---

## 2. Content Fundamentals — how Zad writes

**Tone:** premium, cultural, warm, and emotionally resonant — the register of an
art institution, not a startup. Sentences are evocative but never flowery to the
point of vagueness. Confidence without corporate stiffness.

**Voice & person:**
- Speaks as **"we"** (the organization, a collective) — *"We make space for the
  performing arts to thrive."*
- Addresses the reader as **"you"** when inviting action — *"Join our friends,"
  "Support the artists you love."*
- Arabic copy is **Arabic-first and idiomatic**, not a literal translation of the
  English. The name itself, *زاد الفنون*, carries the metaphor of nourishment —
  lean into that imagery.

**Casing & formatting:**
- **Headlines:** sentence case or title case in heavy Cairo — never ALL CAPS for
  long headlines. Short eyebrow/section labels use **UPPERCASE** with wide
  letter-spacing (e.g. `WHO WE ARE`, `PROGRAMS`).
- **Buttons/links:** concise, verb-led — *"Discover the programs," "Become a
  friend," "See what's on."* Sentence case.
- **No emoji.** This is a cultural institution; expression comes from typography,
  color, and imagery — not emoji or exclamation-spam.

**Copy examples (in-brand):**
- Hero: *"Where Jordan's performing arts find their voice."*
- Who We Are: *"Zad for Arts nourishes the people, ideas, and stages behind
  theater, music, and dance."*
- Programs eyebrow: *"THREE STAGES, ONE COMMUNITY"*
- Support CTA: *"Your support keeps the lights on and the curtain rising."*

**Do / Don't:**
- ✅ Evocative, human, specific to the arts and to Jordan.
- ✅ Bilingual parity — every key message lands in both languages.
- ❌ Hype words, jargon, growth-speak, emoji, exclamation overload.

---

## 3. Visual Foundations

**Background — always white.** No dark sections, no dark mode. The aesthetic is
**gallery-bright**: generous white space lets art and type breathe. The only
non-white "fields" are an occasional faint **cream wash** (`--cream-50/100`) or a
deliberate **full-color block** (purple or red) used as a punctuation moment.

**Color & ratio.** The palette mirrors the logo's proportions:
**purple (dominant) › red (moderate) › cream (sparing) › black (text) on white.**
- **Purple `#8400A9`** is the signature — primary buttons, links, key headlines,
  accent rules, active states.
- **Red `#FF0000`** is energy — used moderately for emphasis, a secondary CTA, a
  single highlighted word, or a category tag. Never the dominant field.
- **Cream `#FFF0C3`** warms things sparingly — soft section backgrounds, cards,
  callouts. Pairs with deep-purple text.
- **Black/near-black `#111`** for body copy and headings; **true black** for the
  logo. **Teal** appears only as the logo flourish — use almost never.

**Typography.** **Cairo only** — one family for both Arabic and English, from large
display headlines down to body. Type tension comes from **weight and scale**, not
from mixing families: headlines run heavy (Cairo 700–800) and confident, body stays
calm and legible (Cairo 400). Body is comfortable at 17px with generous
line-height (1.65, and 1.9 for Arabic). Cairo carries the full Arabic glyph set, so
RTL and LTR share identical type styling.

**Spacing & layout.** 8-pt spacing scale. A `1200px` max content width with `24px`
gutters. Sections are airy — vertical rhythm uses the large `--s-8/9/10` steps
(64–128px) between sections. Layouts are **calm, grid-aligned, editorial** — think
cultural-magazine, not dense dashboard. RTL mirrors the entire grid for Arabic.

**Imagery.** Photography of performances, rehearsals, and artists —
**warm, human, candid**, full-color (stage light tends warm). Used **full-bleed**
in heroes and in clean rectangular/rounded frames in cards. No heavy filters, no
forced duotones (though a subtle purple wash on a hero photo is on-brand). When a
real photo isn't available, use a labeled placeholder — never a generated image.

**Decorative motif — the diamond.** The logo's tilted **diamond/rhombus** dots
(red, purple, teal, black) are the brand's signature shape. Use small rotated
squares as bullets, list markers, decorative accents, and section dividers. This
is the one piece of "ornament" the brand earns. **Bullet / list markers use cream**
(`--cream #FFF0C3`) — best on color or photographic backgrounds where it glows
(e.g. hero eyebrows); on plain white, fall back to purple or red for contrast.
Section dividers use red; outline accents use a purple-stroked diamond.

**Borders & cards.** Hairline borders (`--line #E7E3EC`). Cards are white (or
cream) with a **soft, low, warm-tinted shadow** (`--shadow-md`, purple-tinted) and
a **medium radius (`12–18px`)** — never heavy/blobby rounding, never hard
brutalist corners. Optional thin purple top-rule or a diamond marker for category.

**Corner radii.** Buttons & inputs `8–12px`; cards `12–18px`; pills/tags `999px`
for category chips. Consistent, gentle, never fully square or fully circular
except chips/avatars.

**Shadows / elevation.** Soft and warm, tinted with deep purple (`rgba(42,0,53,…)`)
rather than neutral grey — keeps the bright palette cohesive. Three steps:
`sm` (rest), `md` (cards), `lg` (overlays/menus), plus a `purple` glow for primary
buttons on hover.

**Motion.** Restrained and graceful. Fades and gentle rises (`8–16px` translate),
`240ms` with an ease-out curve (`cubic-bezier(0.16,1,0.3,1)`). No bounces, no
springy overshoot, no infinite looping decoration. Hover = subtle lift + color
deepen; press = slight shrink (`scale .98`) and a darker shade.

**Hover / press states.**
- Primary (purple) button: hover → deepen to `--purple-600` + soft purple glow +
  1px rise; press → `--purple-700`, `scale .98`.
- Secondary button: **cream fill** (`--cream`) with deep-purple text; hover →
  deepen to `--cream-300` + soft shadow + 1px rise.
- Ghost: hover → purple text + faint purple-50 fill.
- Nav links: a **red underline grows from center** on hover with a 2px lift; the
  **active tab keeps a persistent red underline**.
- Links: purple, underline-on-hover (or a growing underline).
- Cards: hover → shadow `md → lg` + 2px rise.

**Transparency & blur.** Used lightly — a translucent white sticky header with a
small `backdrop-filter: blur` on scroll; a subtle purple scrim over full-bleed
hero photos for text legibility (a "protection" gradient from transparent to
~`rgba(42,0,53,.45)` at the bottom). No glassmorphism everywhere.

**Focus states.** Visible purple focus ring (`--focus-ring`) for accessibility —
this is a public, bilingual, inclusive institution.

---

## 4. Iconography

**Approach:** minimal, line-based, and quiet — icons support, never decorate.
- **No bespoke icon font or SVG sprite was available** in the (empty) repo, so this
  system standardizes on **Lucide** (https://lucide.dev) loaded from CDN — a clean,
  consistent **1.75–2px stroke, rounded-join** outline set that matches the brand's
  elegant-but-friendly tone. *(Substitution — flag for review; swap to the team's
  real icon set if one exists.)*
- Stroke icons are drawn in `currentColor` so they inherit `--fg2` / `--primary`.
- Typical sizes: `18–20px` inline, `24px` standalone, `28–32px` feature.
- **The diamond/rhombus** from the logo doubles as the brand's signature
  "icon" — used as bullets, markers, and dividers. **Bullet / list markers are
  cream**; dividers red; accents purple. Prefer the diamond over generic dots.
- **No emoji.** **No unicode-glyph icons.** Category cues come from Lucide icons +
  color, not pictographs.

**Logos** live in `assets/`:
- `zad-logo-black.png` — primary, for the default white background.
- `zad-logo-white.png` — reverse (white wordmark + colored diamonds), for the rare
  full-color (purple/red) or photographic block. Updated Feb-2025 lockup.
Keep clear space around the logo of at least the height of the "Z"; never recolor
or distort it.

---

## 5. Index / Manifest

Root files:
- **`README.md`** — this file (context, content, visual foundations, iconography).
- **`colors_and_type.css`** — all color + type CSS variables and semantic classes.
  Import this in any artifact built for the brand.
- **`SKILL.md`** — Agent-Skill front-matter wrapper so this system can be used as a
  downloadable Claude skill.
- **`fonts/`** — `Cairo-Variable.ttf` (provided body/UI/Arabic face).
- **`assets/`** — logos (and any brand imagery / icons copied in).
- **`preview/`** — small HTML specimen cards that populate the Design System tab
  (colors, type, spacing, components, brand).
- **`ui_kits/website/`** — the bilingual website UI kit:
  `index.html` (interactive demo) + JSX components + its own `README.md`.

> No slide template was provided, so no `slides/` kit was created.

---

## 6. Caveats & open questions (please help me iterate)

1. **Empty source repo** — confirm where the real site code/assets live so the UI
   kit can be raised to true 1:1 fidelity.
2. **Typography is Cairo-only** now (per brand direction). Confirm this is the
   intended single-family system, or share a display face if you want contrast.
3. **Teal accent** — keep it as a rare flourish, drop it entirely, or promote it?
4. **Real photography** — please share performance/artist photos to replace
   placeholders.
5. **Icon set** — confirm Lucide is acceptable or share your own icons.
