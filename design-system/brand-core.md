# EMAi Brand Core (SSOT) · v1.0 · 2026-07

Brand name: always **EMAi** (uppercase EMA, lowercase "i"). Tagline: "caring by tech".
Site: emai.group. Audience: seniors and their families, care providers (DE market).

**Link to the live site's code:** the actual technical source for Digital text roles/colors is `src/styles/global.css` (`@theme` block) in the emai-site repo. This file mirrors it in prose. If global.css changes, update the Digital roles here (and `tokens.json`) together — don't let them drift. `EMAi-Visual-Style-Guide.md` is a retired duplicate of this same information.

## Colors

| Token | HEX | CMYK | Role |
|---|---|---|---|
| Cream | #F7F4EB | 0 1 5 3 | primary background |
| Cream Soft | #FBF9F3 | 0 1 3 2 | nested blocks |
| Cream Deep | #EFE9D9 | 3 5 12 6 | dividers, hover, placeholders |
| White | #FFFFFF | 0 0 0 0 | cards, sections |
| Surface Dark | #5E6472 | 62 51 38 12 | dark section backgrounds; also reused as **Digital Body** text color on web/social only — see Digital text roles below |
| Text 100 | #000000 | 0 0 0 100 | H1–H2 headings — TEXT ONLY (print/PPT roles) |
| Text 70 | #4D4D4D | 0 0 0 70 | body/secondary text — TEXT ONLY (print/PPT roles) |
| Digital Heading | #2D3142 | 68 58 43 22 | web/social heading color — TEXT ONLY, replaces Text 100 for those two carriers. Also the CTA button's **hover** fill (default fill is Surface Dark) |
| Digital Secondary | #7A8090 | 44 34 22 4 | web/social captions/labels/secondary text — lighter than Surface Dark-as-text, e.g. "/device", "/month" |
| Grey Light | #CACBD3 | 20 16 11 0 | light logo variant, disabled — NOT a background |
| Amber ★ | #D69043 | 15 48 86 1 | the only accent: prices, icons, links, active states |
| Amber Soft | #E8B074 | 8 34 58 0 | hover, secondary accent |
| Amber Deep | #B87530 | 24 57 92 8 | pressed state |
| Line | #E2DDD0 | 11 11 18 1 | borders, rules |

Rules: accent is ONLY Amber (no blue/green/red ever). Blacks are text-only, never backgrounds. Dark fills = Surface Dark only. **Big numbers (KPIs, section numbers, sums) are always Amber or Cream**: light background → Amber; amber/dark background → Cream.

Combinations: Cream/White bg → Text 100 headings + Text 70 body + Amber accents. Surface Dark bg → White text + Amber accents. Amber bg → Cream/White text.

## Typography

Fonts across the whole brand: **Gantari** (all headings, every carrier) + **Inter** (numbers everywhere: prices/KPIs, eyebrow numbering, buttons) + **Geist** (digital body text only — web/social). Google Fonts (Gantari, Inter) + Geist. Fallback: DM Sans / Plus Jakarta Sans.

Two text-role sets exist, chosen by carrier — never mix them on the same deliverable. 4 levels max per layout in either set (×1.5 scale step).

**Print text roles** (print, PPT):

| Level | Font/weight | Tracking | Line-height | Color |
|---|---|---|---|---|
| H1 | Gantari Bold 700 | −0.02em | 1.1 | Text 100 |
| H2 | Gantari Semibold 600 | −0.02em | 1.15 | Text 100 |
| Body | Inter Regular 400 | 0 | 1.6–1.7 | Text 70 |
| Secondary | Inter Medium 500 | +0.02em | 1.5 | Text 70 (smaller size, not another color) |

**Digital text roles** (web, social — verified against the live site):

| Level | Font/weight | Tracking | Line-height | Color |
|---|---|---|---|---|
| H1 | Gantari Bold 700 | −0.02em | 1.1 | White (hero on dark/photo) or Digital Heading |
| H2/H3 | Gantari **Medium 500** | −0.02em | 1.15 | Digital Heading (#2D3142) |
| Body | **Geist** Regular 400 | 0 | 1.6–1.7 | Surface Dark reused as text (#5E6472) |
| Secondary/UI/nav | Geist Regular 400 | 0 | 1.5 | Surface Dark reused as text (#5E6472) |

Prices/KPIs/eyebrow numbers (both role sets): Inter Bold 700 (or Medium 500 for eyebrow numbers like "01"), Amber (or Cream on dark/amber).

## Logo — real assets (ALWAYS use these SVGs, never redraw)

Folder: `design-system/assets/logo/`. All viewBox 182.46×85.37. `main` = with tagline "caring by tech"; `small` = wordmark only (use when width < 120px or the tagline would be unreadable).

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

Folder: `design-system/assets/icons/` (13 SVG, viewBox ~383×383, bold rounded-outline style). Available: B2C, b2b, Bell, Calendar, Creation_doc, Facebook, Forwarding_Heart, Grafik, Instagram, Management, Strilka_dveri, telefon, warnung. ALWAYS use these first. Color: Text 70 or Amber (recolor via fill). Checkmarks — Amber.

**Stroke scales with size (optical scaling):** smaller icon → relatively thicker stroke. Base rule ≈7% of icon size, min 2px: 16–24px→2px · 32px→2.5–3px · 48–54px→3.5–4px (card standard) · 64px→4.5–5px · 96px+→6–7px. The existing set has baked-in stroke — optimal at 32–96px display; never use below 24px (use a simplified variant or none).

## Photography

Warm natural light, real seniors/families, homely calm mood. Forbidden: stock clichés, cold blue light, oversaturated colors. Text-over-photo overlay: rgba(0,0,0,.30). Ratios: 1:1 or 4:3.

## Components (base)

CTA button: Surface Dark fill, White 14px Inter Medium, radius 12px (web: hover → Digital Heading). Secondary: transparent, Line border.
Card: White, Line border 1px, radius 24px, shadow 0 8px 32px rgba(45,49,66,.08), padding 28–36px. (Web/social carriers: no border, shadow only — see web.md.)
Inner spacing (edge margin → gutter → block padding) — see the carrier file.

## Tone of voice

Calm, caring, technological yet human. No aggressive marketing, no jargon. Simplicity (older audience).

## QA checklist (before delivering any layout)

- [ ] Background Cream/White (dark only where the carrier allows, Surface Dark)
- [ ] Headings Gantari + correct role color (Text 100 for print, Digital Heading for web/social); body in the matching role font/color; ≤4 text levels
- [ ] Accents and big numbers — Amber/Cream only
- [ ] Brand written as "EMAi"; logo with clear space
- [ ] Icons line-style 1.75px; photos warm
- [ ] Spacing matches the carrier table
