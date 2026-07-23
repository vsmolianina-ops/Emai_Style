# EMAi Design System

Brand: **EMAi** (always uppercase EMA + lowercase "i") · tagline "caring by tech" · emai.group
Product: AI voice companion for seniors. Audience: seniors, their families, care providers (DE market). Mood: calm, caring, warm, technological yet human.

Machine-readable tokens: `design-system/tokens.json`. Full rules: `design-system/brand-core.md`. Human guide: `design-system/EMAi-Design-System-Foundations.html`.

## Colors

- Backgrounds: Cream `#F7F4EB` (primary), Cream Soft `#FBF9F3`, Cream Deep `#EFE9D9` (dividers/hover), White `#FFFFFF` (cards)
- Dark surface: Surface Dark `#5E6472` — backgrounds (titles, dividers); also reused as web/social digital body text color
- Print/PPT text: Text 100 `#000000` (H1–H2), Text 70 `#4D4D4D` (body, secondary) — text only, never backgrounds
- Web/social text: Digital Heading `#2D3142` (headings, also CTA hover fill), Digital Secondary `#7A8090` (captions/labels)
- Accent (the ONLY accent): Amber `#D69043`; hover Amber Soft `#E8B074`; pressed Amber Deep `#B87530`
- Borders: Line `#E2DDD0`. Grey Light `#CACBD3` — light logo variant/disabled only, not a background
- Hard rules: no blue/green/red accents. Big numbers (KPIs, sums, section numbers) always Amber (on light) or Cream (on dark/amber).

## Typography

Two role sets, chosen by carrier — never mixed on one deliverable. Headings always **Gantari**; numbers (prices/KPIs/eyebrow numbers) always **Inter** + Amber, in both sets.

- **Print/PPT:** Gantari Bold 700 (H1) / Semibold 600 (H2), tracking −0.02em; body/secondary **Inter** Regular 400/Medium 500, Text 100/Text 70. 4 levels max.
- **Web/social** (verified against the live site): Gantari Bold 700 (H1) / **Medium 500** (H2/H3); body/secondary **Geist** Regular 400, colored Digital Heading `#2D3142` / Surface Dark-as-text `#5E6472`. 4 levels max.

## Components

- Card: White, radius 24px, shadow `0 8px 32px rgba(45,49,66,.08)`, padding 28–36px. Print/PPT keep a 1px Line border; **web/social cards have no border** (shadow only — verified).
- CTA button: Surface Dark fill, White text 14px Inter Medium, radius 12px, height 42px. Web: **hover → Digital Heading fill** (verified).
- Secondary button: transparent, Line border, Text 70 (print/PPT) or Surface Dark-as-text (web/social)
- Icon circle: 64×64, Amber fill, Cream icon
- Web container: max 1280px; section spacing 64/80/96px (mobile/tablet/desktop)

## Logo (files in design-system/assets/logo/)

- `Logo_EMAI_main.svg` — primary, on Cream/White
- `Logo_Emai_main_light.svg` — on Surface Dark (grey) backgrounds
- `Logo_Emai_small_*.svg` — no-tagline versions for width < 120px
- Black/white versions — only on explicit request (mono print, restricted media)
- Amber dot over "i" never recolored; clear space ≥ height of "E"; min width 80px

## Icons (files in design-system/assets/icons/)

Bold rounded-outline style, ~7% stroke of icon size (min 2px), round caps/joins, no fills, 1–3 shapes. Recolor via fill: Text 70 or Amber. Optimal display 32–96px.

## Photography

Warm natural light, real seniors and families, homely calm mood. Never: stock clichés, cold blue light, oversaturation. Overlay for text on photo: rgba(0,0,0,.30).
