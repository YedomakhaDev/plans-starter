# Design tokens

**Source of truth** for design and code. Change a value here first, then in Figma and in code.
WordPress: colors, fonts, and sizes → `theme.json` (Gutenberg palette and typography) + CSS variables.

Status: <!-- v0.1 — where it comes from, date -->

## Colors

| Token | HEX | Role |
|---|---|---|
| `bg` | | Main background |
| `surface` | | Section / card background |
| `text` | | Primary text |
| `text-secondary` | | Secondary text |
| `accent` | | CTAs, links, active states |
| `accent-hover` | | Accent hover |
| `border` | | Borders, dividers |

### Contrast (WCAG AA: 4.5:1 for normal text, 3:1 for large text)

| Pair | Contrast | OK? |
|---|---|---|
| `text` on `bg` | | |
| `text-secondary` on `bg` | | |
| button text on `accent` | | |

## Fonts

| Role | Font | Where |
|---|---|---|
| Headings | | |
| Body | | |
| Accent / metadata (optional) | | |

Load fonts locally in the theme (self-hosted): faster and no GDPR concerns.

## Type scale

| Token | Font | Size / line height (desktop) | Mobile |
|---|---|---|---|
| `h1` | | | |
| `h2` | | | |
| `h3` | | | |
| `lead` | | | |
| `body` | | | |
| `small` | | | |

## Sizes and spacing

| Token | Value |
|---|---|
| Container width | |
| Section padding top / bottom | |
| Grid gap | |
| Card padding | |

## Radii

| Element | Radius |
|---|---|
| Cards | |
| Buttons, fields | |
| Images | |

## Borders and effects

- <!-- border width, shadows (used / not used), animations -->
