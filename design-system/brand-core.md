# EMAi Brand Core (SSOT) · v1.0 · 2026-07

Brand name: always **EMAi** (uppercase EMA, lowercase "i"). Tagline: "caring by tech".
Site: emai.group. Audience: seniors and their families, care providers (DE market).

## Colors

| Token | HEX | CMYK | Role |
|---|---|---|---|
| Cream | #F7F4EB | 0 1 5 3 | primary background |
| Cream Soft | #FBF9F3 | 0 1 3 2 | nested blocks |
| Cream Deep | #EFE9D9 | 3 5 12 6 | dividers, hover, placeholders |
| White | #FFFFFF | 0 0 0 0 | cards, sections |
| Surface Dark | #5E6472 | 62 51 38 12 | dark section backgrounds ONLY — never text |
| Text 100 | #000000 | 0 0 0 100 | H1–H2 headings — TEXT ONLY |
| Text 70 | #4D4D4D | 0 0 0 70 | body/secondary text — TEXT ONLY |
| Grey Light | #CACBD3 | 20 16 11 0 | light logo variant, disabled — NOT a background |
| Amber ★ | #D69043 | 15 48 86 1 | the only accent: prices, icons, links, active states |
| Amber Soft | #E8B074 | 8 34 58 0 | hover, secondary accent |
| Amber Deep | #B87530 | 24 57 92 8 | pressed state |
| Line | #E2DDD0 | 11 11 18 1 | borders, rules |

Rules: accent is ONLY Amber (no blue/green/red ever). Blacks are text-only, never backgrounds. Dark fills = Surface Dark only. **Big numbers (KPIs, section numbers, sums) are always Amber or Cream**: light background → Amber; amber/dark background → Cream.

Combinations: Cream/White bg → Text 100 headings + Text 70 body + Amber accents. Surface Dark bg → White text + Amber accents. Amber bg → Cream/White text.

## Typography

Fonts: **Gantari** (headings) + **Inter** (body/UI). Google Fonts. Fallback: DM Sans / Plus Jakarta Sans.
4 levels (×1.5 scale step, never more levels on one layout):

| Level | Font/weight | Tracking | Line-height | Color |
|---|---|---|---|---|
| H1 | Gantari Bold 700 | −0.02em | 1.1 | Text 100 |
| H2 | Gantari Semibold 600 | −0.02em | 1.15 | Text 100 |
| Body | Inter Regular 400 | 0 | 1.6–1.7 | Text 70 |
| Secondary | Inter Medium 500 | +0.02em | 1.5 | Text 70 (smaller size, not another color) |

Prices/KPIs: Inter Bold 700, Amber (or Cream on dark/amber).

## Logo — real assets (ALWAYS use these SVGs, never redraw)

Folder: connected project folder `Emai_design_system/Emai_Logo/` (Vita's PC: `C:\Work\EMAI\Emai_design_system\Emai_Logo\`). All viewBox 182.46×85.37. `main` = with tagline "caring by tech"; `small` = wordmark only (use when width < 120px or the tagline would be unreadable).

| File | Use on |
|---|---|
| Logo_EMAI_main.svg | primary: Cream/White backgrounds (grey letters + amber dot) |
| Logo_Emai_main_light.svg | grey (Surface Dark) backgrounds — default dark-surface variant |
| Logo_Emai_small_light.svg | grey (Surface Dark), small sizes / where tagline unreadable |
| Logo_EMAI_main_black.svg, Logo_EMAI_main_white.svg | ONLY on explicit request — special cases, never by default |
| Logo_Emai_small_*.svg | wordmark without tagline, width < 120px (same color logic) |

On Amber backgrounds: use the white variant only as an approved special case (e.g. PPT contact slide); otherwise avoid placing the logo on Amber.

Rules: dot over "i" stays #D69043 (except white/black variants as drawn). Clear space ≥ height of "E". Min width: 80px / 22mm (main), 48px (small). Never: recolor, stretch, shadow, busy-photo background.

## Icons — real assets

Folder: `Emai_design_system/Emai_icon/` (13 SVG, viewBox ~383×383, bold rounded-outline style). Available: B2C, b2b, Bell, Calendar, Creation_doc, Facebook, Forwarding_Heart, Grafik, Instagram, Management, Strilka_dveri, telefon, warnung. ALWAYS use these first. Color: Text 70 or Amber (recolor via fill). Checkmarks — Amber.

**Stroke scales with size (optical scaling):** smaller icon → relatively thicker stroke. Base rule ≈7% of icon size, min 2px: 16–24px→2px · 32px→2.5–3px · 48–54px→3.5–4px (card standard) · 64px→4.5–5px · 96px+→6–7px. The existing set has baked-in stroke — optimal at 32–96px display; never use below 24px (use a simplified variant or none).

**Creating a missing icon:** match the set. Spec: canvas 384×384, stroke 28 units (~7.3%), round caps and joins, outline style (no fills), 1–3 shape elements, 24-unit safe margin, monochrome single path color. Save SVG to `Emai_icon/` with an English name. Ready generator prompt: `core/icon-prompt.md`. After generating: vectorize/clean if needed, verify side-by-side with 2–3 existing icons before use.

## Photography

Warm natural light, real seniors/families, homely calm mood. Forbidden: stock clichés, cold blue light, oversaturated colors. Text-over-photo overlay: rgba(0,0,0,.30). Ratios: 1:1 or 4:3.

## Components (base)

CTA button: Surface Dark fill, White 14px Inter Medium, radius 12px. Secondary: transparent, Line border.
Card: White, Line border 1px, radius 24px, shadow 0 8px 32px rgba(45,49,66,.08), padding 28–36px.
Inner spacing (edge margin → gutter → block padding) — see the carrier file.

## Tone of voice

Calm, caring, technological yet human. No aggressive marketing, no jargon. Simplicity (older audience).

## QA checklist (before delivering any layout)

- [ ] Background Cream/White (dark only where the carrier allows, Surface Dark)
- [ ] Headings Gantari + Text 100; body Inter + Text 70; ≤4 text levels
- [ ] Accents and big numbers — Amber/Cream only
- [ ] Brand written as "EMAi"; logo with clear space
- [ ] Icons line-style 1.75px; photos warm
- [ ] Spacing matches the carrier table
