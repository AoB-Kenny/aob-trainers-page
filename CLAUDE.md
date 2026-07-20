# Art of Breath — Trainers Website

## What this project is

**Art of Breath** is a breathwork-teacher training program. The company trains people to become
breathwork trainers, who then go on to train others. Until now the sole main teacher has been
**Daniel Alan**; the program is now expanding to a wider roster of trainers.

This repository is the **website for and about these new trainers**. When finished it will have
three parts:

1. **Introduction** to the Art of Breath project as a whole.
2. **Trainers overview & sorting** — a browsable, sortable directory of all trainers. *(Current focus.)*
3. **Graduates** — a list of everyone who has successfully graduated the program.

### Current focus

The **trainers overview and sorting** view. Start here.

## Brand & design system

> **ALWAYS invoke the `frontend-design` skill before any design work** — new UI, layout, visual
> direction, or reshaping existing UI. No exceptions. Run it *before* writing markup or CSS so the
> aesthetic direction is deliberate rather than templated, and derive colors/type/layout from it
> together with the brand docs below.

Art of Breath is a sub-brand of **Daniel Alan** (the parent brand). The visual language inherits
much of the parent's tone — warm, quiet, grounded neutrals; "let viewers feel before they think."

| File | What it holds |
|------|---------------|
| `colors.md` | Full color system. **Primary** palette (the four AoB brand neutrals) + **secondary** palette (inherited from Daniel Alan), each with 10-step scales, plus text roles. Single source of truth for color. |
| `fonts.md` | Font families, weights, web font stacks. Athelas/Playfair Display (headings), Raleway (body). |
| `typo.md` | Type scale (H1–H6, paragraphs), desktop + mobile, line-height & tracking tokens. References color by role name from `colors.md`. |
| `radii.md` | Corner-radius tokens. **Buttons use an 18px radius (brand standard)**; inputs/dropdowns match; tags stay fully rounded; nav tabs kept crisper. |
| `Art of Breath Logo Variants 2025/` | All logos (SVG + PNG), one per color variant: rooted-earth, ash-fog, weathered-bone, charcoal-smoke, white. Both an icon mark and a wordmark lockup exist per color. |

### Color notes

- **Primary palette** = the four Art of Breath brand neutrals, extracted from the logo variants:
  Rooted Earth `#AA9983`, Ash Fog `#7C705C`, Weathered Bone `#C1B9A7`, Charcoal Smoke `#383530`.
  Their meanings in `colors.md` are provisional (derived to match the parent brand's tone) —
  refine with the client if canonical descriptions exist.
- **Secondary palette** = inherited from the Daniel Alan branding bible: Ember, Wood, Dust,
  Charcoal, Moss, Ochre.
- **10-step scales**: step 50 is the canonical brand hex; 00–40 tint toward warm off-white,
  60–100 shade toward warm near-black. The exact procedure (anchors + per-step fractions) is
  documented in `colors.md` so it can be reapplied to any new color.
- Reference colors by **role/token name**, never raw hex, in components. `colors.md` is the
  single source of truth.
- Charcoal Smoke replaces pure black. Keep contrast soft — quiet, not loud.

### Type notes

- Serif heading over sans subheading; do not mix the two roles. Let type breathe.
- Web: **Playfair Display** (headings) + **Raleway** (body) are the licensable substitutes for the
  proprietary Apple faces Athelas/Galvji.

### Copy notes

- **No em-dashes.** Never use `—` (em-dash) in copy. Use a comma, a colon, or a separate sentence
  instead. (The parent-brand copy guide calls this "no em-dash-prosa"; it is a hard rule here.)
- **German first**, Du-form, **no gendering** (generic masculine: "Trainer", not "Trainer:innen").
- AoB voice is **broader and plainer** than the personal Daniel Alan brand, and speaks about Art of
  Breath in the **third person** to a "du" reader (no "wir"/"uns" narrative voice). Daniel Alan stays a
  background credibility anchor. See the working copy in `copy/` and `content/` for reference only.
