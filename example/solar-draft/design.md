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

## §1 Identité

Solar Draft est l'esthétique d'une agence créative solaire. Fond crème chaleureux (`--canvas`), accent or doré (`--gold`), tension entre chaleur artisanale et précision moderne. Pas de blanc froid. Pas de gris désaturé. Toujours chaud, toujours intentionnel.

## §2 Rôles couleurs

`--canvas` est le fond universel. `--gold` est l'action — réservé aux CTAs, liens actifs, accents hover. `--ink` est le texte dominant — titres, labels courts, valeurs en évidence. `--muted` pour le corps de texte et les sous-titres longs. `--canvas-deep` pour toutes les surfaces alternatives (sections, cards, zones alternées).

## §3 Typographie

Plus Jakarta Sans (`--font-display`) pour tous les titres : uppercase, `letter-spacing: -0.03em`, `line-height: 0.92`. Géométrique et impactant. DM Sans (`--font-body`) pour le corps : poids 400, line-height 1.7. Pattern eyebrow : DM Sans, `--text-xs`, `letter-spacing: 0.20em`, uppercase, couleur `--gold-deep`.

## §4 Composants

- **Boutons** : variant gold (fill `--gold`, texte `--ink`) ou outline (border 2px `--ink`, texte `--ink`, hover: bg `--ink` texte `--canvas`). Radius `--radius-full`. Jamais de fond blanc pur.
- **Cards** : fond `--canvas-deep`, border `1px solid var(--line)`. Hover : border `--line-accent`. Radius `--radius-lg`.
- **Badges** : fond `--canvas-deep`, texte uppercase `--text-xs`, couleur `--ink-soft`. Radius `--radius-full`.
- **Inputs** : fond `--canvas`, border `1px solid var(--line)`. Focus : border `--gold`. Jamais de fond blanc pur.

## §5 Layout

Container max-width 1200px (`.wrap`). Padding horizontal `--space-5` (40px). Sections : padding vertical `--space-7` (96px). Breakpoint responsive : 768px. Grille de travail : espacement `--space-4` (24px) entre éléments. Les variables CSS suivent la convention : `--space-1` à `--space-8`, `--radius-sm/md/lg/xl/full`, `--text-xs/sm/base/lg/xl/2xl/3xl/hero`.

## §6 Instructions agent

1. Utilise exclusivement `--canvas`, `--canvas-deep`, ou `--canvas-card` comme fonds. Jamais `#fff`, `white`, `#000`, `black` — toujours les variables.
2. `--gold` est réservé à l'action — boutons primaires, accents de survol. Un seul CTA gold par section.
3. Titres : Plus Jakarta Sans uppercase, `letter-spacing: -0.03em`, `line-height: 0.92`. Toujours.
4. Corps de texte : `--muted`, pas `--ink` (trop sombre pour les paragraphes longs).
5. Chaque card doit avoir `border: 1px solid var(--line)` et fond `--canvas-deep`. Pas de box-shadow.
6. Espacements : utilise les variables `--space-*`, jamais de valeurs hardcodées.
7. Eyebrow avant chaque titre de section : `.eyebrow` en DM Sans, `--text-xs`, `letter-spacing: 0.20em`, couleur `--gold-deep`.
8. Sur mobile (< 768px) : titres passent en `--text-2xl`, padding horizontal `--space-3` (16px).

> 💡 **Full implementation available** — This `design.md` ships with a complete HTML/CSS kit: demo page, all components, CSS tokens ready to use. No setup needed.
> → [www.stacklift.design/kit/solar-draft](https://www.stacklift.design/kit/solar-draft)
