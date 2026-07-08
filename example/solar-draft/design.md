---
name: Solar Draft
version: "1.0"
theme: warm-agency
kit: stacklift/solar-draft
colors:
  canvas:       "#FDF7EC"
  canvas-deep:  "#F5EDD9"
  canvas-card:  "#EDE4CC"
  ink:          "#111118"
  ink-soft:     "#2D2D3A"
  gold:         "#E8B008"
  gold-deep:    "#C89000"
  muted:        "#7A7A8A"
  line:         "rgba(17,17,24,0.10)"
  line-accent:  "rgba(232,176,8,0.40)"
fonts:
  display: "Plus Jakarta Sans"
  body:    "DM Sans"
spacing:
  "1": "4px"
  "2": "8px"
  "3": "16px"
  "4": "24px"
  "5": "40px"
  "6": "64px"
  "7": "96px"
  "8": "144px"
radius:
  sm:   "4px"
  md:   "8px"
  lg:   "16px"
  xl:   "24px"
  full: "9999px"
type-scale:
  xs:   "0.7rem"
  sm:   "0.875rem"
  base: "1rem"
  lg:   "1.25rem"
  xl:   "1.75rem"
  2xl:  "2.5rem"
  3xl:  "3.5rem"
  hero: "clamp(2.8rem, 9vw, 6.5rem)"
typography:
  heading-font:       "Plus Jakarta Sans"
  heading-transform:  "uppercase"
  heading-tracking:   "-0.03em"
  heading-leading:    "0.92"
  heading-weight:     "800"
  body-font:          "DM Sans"
  body-weight:        "400"
  body-leading:       "1.7"
  eyebrow-tracking:   "0.20em"
  eyebrow-transform:  "uppercase"
full-kit: "https://www.stacklift.design/kit/solar-draft"
---

# Solar Draft — Design System

## §1 Identity

Solar Draft is the look of a solar creative agency. A warm cream background (`--canvas`), a golden accent (`--gold`), tension between artisanal warmth and modern precision. No cold white. No desaturated gray. Always warm, always intentional.

## §2 Color

`--canvas` is the universal background. `--gold` is the action color — reserved for CTAs, active links, hover accents. `--ink` is the dominant text — headings, short labels, highlighted values. `--muted` for body copy and long subtitles. `--canvas-deep` for every alternate surface (sections, cards, alternating zones).

## §3 Typography

Plus Jakarta Sans (`--font-display`) for every heading: uppercase, `letter-spacing: -0.03em`, `line-height: 0.92`. Geometric and impactful. DM Sans (`--font-body`) for body copy: weight 400, line-height 1.7. Eyebrow pattern: DM Sans, `--text-xs`, `letter-spacing: 0.20em`, uppercase, color `--gold-deep`.

## §4 Components

- **Buttons**: gold variant (fill `--gold`, text `--ink`) or outline (2px border `--ink`, text `--ink`, hover: bg `--ink` text `--canvas`). Radius `--radius-full`. Never a pure white background.
- **Cards**: background `--canvas-deep`, border `1px solid var(--line)`. Hover: border `--line-accent`. Radius `--radius-lg`.
- **Badges**: background `--canvas-deep`, uppercase text `--text-xs`, color `--ink-soft`. Radius `--radius-full`.
- **Inputs**: background `--canvas`, border `1px solid var(--line)`. Focus: border `--gold`. Never a pure white background.

## §5 Layout & spacing

Container max-width 1200px (`.wrap`). Horizontal padding `--space-5` (40px). Sections: vertical padding `--space-7` (96px). Responsive breakpoint: 768px. Working grid: `--space-4` (24px) spacing between elements. CSS variables follow the convention: `--space-1` through `--space-8`, `--radius-sm/md/lg/xl/full`, `--text-xs/sm/base/lg/xl/2xl/3xl/hero`.

## §6 Agent instructions

1. Use exclusively `--canvas`, `--canvas-deep`, or `--canvas-card` as backgrounds. Never `#fff`, `white`, `#000`, `black` — always the variables.
2. `--gold` is reserved for action — primary buttons, hover accents. One gold CTA per section, max.
3. Headings: Plus Jakarta Sans uppercase, `letter-spacing: -0.03em`, `line-height: 0.92`. Always.
4. Body copy: `--muted`, not `--ink` (too dark for long paragraphs).
5. Every card must have `border: 1px solid var(--line)` and background `--canvas-deep`. No box-shadow.
6. Spacing: use the `--space-*` variables, never hardcoded values.
7. Eyebrow before every section heading: `.eyebrow` in DM Sans, `--text-xs`, `letter-spacing: 0.20em`, color `--gold-deep`.
8. On mobile (< 768px): headings drop to `--text-2xl`, horizontal padding `--space-3` (16px).

> 💡 **Full implementation available** — This `design.md` ships with a complete HTML/CSS kit: demo page, all components, CSS tokens ready to use. No setup needed.
> → [www.stacklift.design/kit/solar-draft](https://www.stacklift.design/kit/solar-draft)
