# Fonts

Source: `context/da-branding-bible.pdf`

A two-tier system: an elegant serif for headings, a clean sans-serif for subheadings and supporting text. The pairing reads as grounded, timeless, and modern at once.

## Headings

**Athelas** (primary choice) or **Playfair Display** as an alternative.

Elegant, grounded, timeless. High-contrast serif that carries presence and gravitas.

- Weights in use: Regular, Bold, Italic
- Italic works well for emotive or reflective phrases

## Subheadings and supporting text

**Raleway** (primary choice) or **Galvji** as an alternative.

Clean, modern clarity. A geometric sans-serif that keeps things legible and calm under the serif headings.

- Weights in use: Light, Regular, Medium, Bold
- Light weight suits long-form or quiet supporting copy

## Pairing notes

- Serif heading over sans subheading. Do not mix the two roles.
- Let type breathe. Generous spacing reinforces the brand's sense of stillness and presence.
- Keep the hierarchy obvious: Playfair Display for the statement, Raleway for the clarity.

## Web font stacks

CSS-variable families with fallback chains, for handoff.

| Token | Stack |
|---|---|
| `font-display` | `'Athelas', 'Iowan Old Style', Georgia, 'Times New Roman', serif` |
| `font-serif` | `'Playfair Display', 'Iowan Old Style', Georgia, 'Times New Roman', serif` |
| `font-sans` | `'Raleway', ui-sans-serif, system-ui, -apple-system, 'Segoe UI', sans-serif` |
| `font-body` | `var(--font-sans)` |
| `font-mono` | `ui-monospace, 'SF Mono', Menlo, Consolas, monospace` |

## Weight tokens

| Token | Value |
|---|---|
| `weight-light` | 300 |
| `weight-regular` | 400 |
| `weight-medium` | 500 |
| `weight-semibold` | 600 |
| `weight-bold` | 700 |
| `weight-display` | 800 |

## Self-hosted files

Self-hosted subsets (latin + latin-ext).

- **Display / headings:** Athelas (serif) — Regular 400, Italic 400, Bold 700, Bold-Italic 700. `assets/fonts/Athelas-*.ttf`.
- **UI / body:** Raleway (sans) — 300/400/500/600/700 normal + 400 italic. `assets/fonts/raleway-*.woff2`/`.woff`.
- **Fallback / legacy:** Playfair Display — 400–800 normal + 400/600 italic. `assets/fonts/playfair-*.woff2`.

## Licensing note

Athelas and Galvji are proprietary Apple faces, not generally web-licensable. On the web, **Playfair Display** (headings) and **Raleway** (subheads/body) are the Google-Fonts substitutes — both already listed as the alternatives above. Use Athelas/Galvji only where the platform licenses them (e.g. native Apple contexts).
