# Typography

Source: manual rundown. Font definitions in [`fonts.md`](./fonts.md).

## Headings

Font: **Athelas** (primary) or **Playfair Display** (fallback).
Line height: auto. Style: Regular. Optional italic.

| Level | Size | Letter spacing |
|-------|------|----------------|
| H1 | 60px | 15% |
| H2 | 52px | 5% |
| H3 | 44px | 0% |
| H4 | 32px | 0% |
| H5 | 24px | 0% |
| H6 | 20px | 0% |

## Paragraphs

Font: **Raleway** (primary) or **Galvji** (fallback), per [`fonts.md`](./fonts.md). Optional italic.

| Variant | Size | Line height | Weight |
|---------|------|-------------|--------|
| Default | 16px | 150% | Regular |
| Small | 12px | 150% | Regular |
| Large | 20px | 150% | Medium |

## Mobile

Scaled-down values for small screens. Letter spacing, line height, font, and style carry over from the desktop specs above.

### Headings

| Level | Size |
|-------|------|
| H1 | 40px |
| H2 | 34px |
| H3 | 30px |
| H4 | 26px |
| H5 | 22px |
| H6 | 18px |

### Paragraphs

| Variant | Size | Line height | Weight |
|---------|------|-------------|--------|
| Default | 16px | 150% | Regular |
| Small | 12px | 150% | Regular |
| Large | 18px | 150% | Medium |

## Use cases

Reference color by role name from [`colors.md`](./colors.md) (e.g. `text-primary`), not raw hex.

<!-- Add specific use cases here (e.g. which level for hero, section titles, captions). -->

## Web tokens

Tokens for handoff. The H1–H6 and paragraph sizes above stay canonical; these add the values the size table doesn't cover.

### Line heights

| Token | Value | Use |
|---|---|---|
| `leading-tight` | 1.08 | large display / hero |
| `leading-snug` | 1.22 | headings |
| `leading-normal` | 1.5 | body (matches the 150% above) |
| `leading-relaxed` | 1.7 | long-form, calm reading rhythm |

### Letter spacing (tracking)

Named tokens for labels and display. Headings keep their positive spacing from the table above (H1 15%, H2 5%, rest 0%); these tokens cover the cases the table doesn't.

| Token | Value | Use |
|---|---|---|
| `tracking-tight` | -0.01em | large display, optional |
| `tracking-normal` | 0 | most headings (H3–H6) |
| `tracking-wide` | 0.04em | labels |
| `tracking-wider` | 0.12em | small-cap labels, eyebrows |
| `tracking-widest` | 0.28em | the `D A N I E L   A L A N` lockup |

### Display / hero (web only)

For oversized hero statements beyond H1 (60px). Athelas, weight bold, leading tight.

| Role | Size | Use |
|---|---|---|
| Display | ~68px | landing statements |
| Hero | ~85px | full-bleed hero |

### Label & eyebrow roles

| Role | Family | Weight | Other |
|---|---|---|---|
| Eyebrow | Raleway | semibold | uppercase, size 12px, tracking widest, color `text-muted` |
| Label | Raleway | semibold | tracking wide |
| Lockup | Raleway | semibold | uppercase, tracking widest (0.28em) — the `D A N I E L   A L A N` mark |
| Quote | Athelas | regular italic | size ~34px (H3), leading snug, color `text-primary` |
