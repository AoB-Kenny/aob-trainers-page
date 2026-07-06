# Corner radii

Source: parent-brand (Daniel Alan) design standard, confirmed by the client.

The brand uses soft, consistent rounding — quiet and grounded, never sharp, never fully
pill-shaped except for tags. **Buttons are the anchor: they always use an 18px corner radius.**
Inputs and dropdowns match the buttons so form controls read as one family.

## Tokens

| Token | Value | Use |
|---|---|---|
| `--r-btn` | **18px** | **Buttons — the brand standard.** Primary/solid CTAs, secondary buttons, any filled action. |
| `--r-input` | 18px | Dropdowns, selects, text inputs. Matches the button radius. |
| `--r-card` | 18px | Cards and larger surfaces. |
| `--r-tab` | 9px | Nav tabs / text-link chips — kept crisper, since these are not filled buttons. |
| `--r-pill` | 999px | Fully rounded — reserved for tags/pills only. |

## Notes

- **18px is the button rule.** When in doubt for an interactive, filled control, use 18px.
- Match inputs and dropdowns to buttons (18px) so controls feel unified.
- Do not fully round buttons — the pill shape (`999px`) is reserved for tags.
- Nav tabs stay tighter (9px) so the header reads crisp rather than bubbly.
- Reference these tokens by name in components, the same way color is referenced from
  [`colors.md`](./colors.md) and type from [`typo.md`](./typo.md).
