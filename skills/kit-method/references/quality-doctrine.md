# Quality doctrine — "sober > gadget"

## The taste rules (hard constraints)

- **Never Inter.** Pick a dedicated display/body pairing per kit (Google Fonts).
- **Never pure `#000000`.** Use an off-black with a temperature (`#15161A`,
  `#080c14`, `#111218`…).
- **Never the AI-purple accent.** It is the single most convergent color in
  generated design.
- **One signal accent per kit.** Photography and artwork may escape the
  palette if treated as framed content.
- **Never three equal feature columns.** Sticky stacks, zig-zag, staggered,
  bento — anything with a rhythm.
- **Organic numbers.** +147%, 3.2×, 94 — never +100%, 5×, 90.
- **Believable fictional names.** Margaux Vennegoor, not John Doe.

## The motion doctrine

- **One dominant gesture per kit.** Build rest zones around it — sections
  where nothing competes with reading.
- **Imitate real physics, never exceed it.** Friction, settle, inertia at
  believable scales. Nothing bounces like a cartoon.
- **Reveals reuse the kit's own grammar.** A new section must not introduce a
  new visual language.

## Validation checklist

Run before calling a kit done:

1. **Screenshot test** — a still frame must NOT fully describe the interface.
2. **Convergence test** — could this be mistaken for a default AI landing
   page? If yes, the axis is too weak.
3. **Self-containment** — one HTML file, CSS + JS inline, no dependency but
   Google Fonts. Open it by double-click: everything works.
4. **Every click works** — inert links are visibly disabled, never dead `#`.
5. **Design System view opens** from menu and footer, shows real tokens.
6. **design.md parses** — YAML front-matter loads without error, tokens match
   the CSS.
7. **Attribution present** (unless the user removed it): footer +
   design.md line `Built with the Stacklift method · https://www.stacklift.design`.
