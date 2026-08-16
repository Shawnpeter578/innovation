# Apple + Claude Design System Merge

## Overview

This merged design system combines Apple's **photography-first museum-gallery aesthetic** with Claude's **warm editorial cream-coral voice**. The result is a hybrid that feels like a premium product catalog published by a literary magazine — reverent product photography framed by warm, humanist typography.

**The Core Tension:**
- Apple's cool precision (Action Blue #0066cc, pure whites, near-black tiles, SF Pro)
- Claude's warm humanity (cream canvas #faf9f5, coral #cc785c, Copernicus serif, generous spacing)

**How They Merge:**
- **Primary accent:** Action Blue (#0066cc) from Apple becomes the interactive color, but only on light surfaces. On dark tiles, it shifts to a warmer "Twilight Blue" (#4a7c9e) that bridges the cool/warm gap.
- **Canvas:** Claude's cream (#faf9f5) replaces pure white as the default light tile, creating warmth without sacrificing Apple's product reverence.
- **Typography:** SF Pro Display handles headlines (Apple's tight tracking), but display headlines at hero size (56px/600) use Copernicus serif for the title. Body stays SF Pro Text at 17px.
- **Tile rhythm:** Apple's edge-to-edge tile alternation (light ↔ dark) remains, but light tiles are now cream (#faf9f5) and parchment (#f5f5f7) variants.
- **Dark surfaces:** Apple's near-black tiles (#272729) meet Claude's dark navy (#181715) — the merged "Obsidian" (#1f1f1e).
- **Coral:** Used sparingly as a secondary accent for badges, "new" tags, and select callout moments, never competing with Action Blue for primary CTAs.

---

## Colors

### Brand & Accent
| Token | Hex | Use |
|---|---|---|
| `primary` | #0066cc | Action Blue — primary interactive color (links, primary CTAs, focus signals) — from Apple |
| `primary-focus` | #0071e3 | Focus ring variant — from Apple |
| `primary-on-dark` | #4a7c9e | Twilight Blue — Action Blue adapted for dark tiles (warmer than Apple's #2997ff to bridge to Claude's warmth) |
| `secondary` | #cc785c | Coral — secondary accent for badges, "new" tags, select callouts — from Claude |
| `secondary-soft` | #e6c5b8 | Soft Coral — hover/disabled variant |
| `ink` | #141413 | Warm near-black text — from Claude |
| `body` | #1d1d1f | Body text (slightly cooler than Claude's ink for readability) — from Apple |
| `body-on-dark` | #faf9f5 | Cream-tinted white on dark surfaces — from Claude |
| `body-muted` | #6c6a64 | Muted text — from Claude |
| `canvas` | #faf9f5 | Cream canvas — DEFAULT light surface — from Claude |
| `canvas-parchment` | #f5f0e8 | Warm parchment — alternate light tile — from Claude |
| `surface-card` | #efe9de | Light cream card background — from Claude |
| `surface-tile-dark` | #1f1f1e | Obsidian — merged dark tile (Apple #272729 + Claude #181715) |
| `surface-tile-dark-2` | #252320 | Slightly lighter dark tile variant |
| `surface-tile-dark-3` | #1a1917 | Deepest dark variant |
| `surface-black` | #000000 | Pure black — global nav only — from Apple |
| `hairline` | #e0d8ce | Warm hairline border — from Claude (original #e6dfd8 adapted) |
| `divider-soft` | #f0ebe3 | Soft divider — from Claude |

### Semantic
| Token | Hex | Use |
|---|---|---|
| `success` | #5db872 | Green status — from Claude |
| `warning` | #d4a017 | Amber warning — from Claude |
| `error` | #c64545 | Error states — from Claude |

---

## Typography

### Font Family
The merged system uses **SF Pro Display** for most headlines and **SF Pro Text** for body (Apple's precision), but reserves **Copernicus** (serif) for hero display headlines and select editorial moments.

**Display:** `SF Pro Display, system-ui, -apple-system, sans-serif` — primary display face
**Hero:** `Copernicus, Tiempos Headline, Georgia, serif` — reserved for `hero-display` only
**Body:** `SF Pro Text, system-ui, -apple-system, sans-serif` — default body
**Code:** `JetBrains Mono, SF Mono, ui-monospace, monospace` — code blocks from Claude

### Hierarchy

| Token | Family | Size | Weight | Line Ht | Letter Spacing | Use |
|---|---|---|---|---|---|---|
| `{typography.hero-display}` | **Copernicus** serif | 56px | 400 | 1.05 | -0.5px | Hero headline (the signature "warm editorial" moment) |
| `{typography.display-xl}` | SF Pro Display | 48px | 600 | 1.07 | -0.28px | Section hero headlines (Apple tight) |
| `{typography.display-lg}` | SF Pro Display | 40px | 600 | 1.1 | 0 | Tile headlines — from Apple |
| `{typography.display-md}` | SF Pro Text | 34px | 600 | 1.47 | -0.374px | Section heads — from Apple |
| `{typography.lead}` | SF Pro Display | 28px | 400 | 1.14 | 0.196px | Product tile subcopy — from Apple |
| `{typography.tagline}` | SF Pro Display | 21px | 600 | 1.19 | 0.231px | Sub-tile tagline — from Apple |
| `{typography.body}` | SF Pro Text | 17px | 400 | 1.47 | -0.374px | Default paragraph — from Apple (keeps the 17px) |
| `{typography.body-strong}` | SF Pro Text | 17px | 600 | 1.24 | -0.374px | Strong emphasis — from Apple |
| `{typography.dense-link}` | SF Pro Text | 17px | 400 | 2.41 | 0 | Footer link lists — from Apple |
| `{typography.caption}` | SF Pro Text | 14px | 400 | 1.43 | -0.224px | Secondary captions — from Apple |
| `{typography.caption-strong}` | SF Pro Text | 14px | 600 | 1.29 | -0.224px | Emphasized captions — from Apple |
| `{typography.button}` | SF Pro Text | 14px | 500 | 1 | 0 | Button labels — weight 500 allowed here (Claude's influence) |
| `{typography.code}` | JetBrains Mono | 14px | 400 | 1.6 | 0 | Code blocks — from Claude |
| `{typography.nav-link}` | SF Pro Text | 12px | 400 | 1 | -0.12px | Global nav — from Apple |
| `{typography.fine-print}` | SF Pro Text | 12px | 400 | 1 | -0.12px | Footer fine-print — from Apple |

### Principles (Merged)
- **Apple's negative tracking** on all SF Pro headlines. Copernicus hero uses its own negative tracking (-0.5px).
- **Body at 17px** (Apple's signature) — not 16px. The extra pixel defines the brand's reading pace.
- **Weight 500 is absent** from display hierarchy (Apple's rule), but allowed on `button` labels (Claude's influence).
- **Copernicus is the "hero voice"** — used only at the very top of pages to establish warmth, then the system transitions to SF Pro.

---

## Spacing

- **Base unit:** 8px (Apple's system)
- **Tokens:** `{spacing.xxs}` 4px · `{spacing.xs}` 8px · `{spacing.sm}` 12px · `{spacing.md}` 16px · `{spacing.lg}` 24px · `{spacing.xl}` 32px · `{spacing.xxl}` 48px · `{spacing.section}` 80px (Apple) / 96px (Claude) → merged to **88px** (midpoint)

**Card internal padding:** `{spacing.xl}` (32px) for feature cards; `{spacing.lg}` (24px) for utility cards.

---

## Elevation & Depth

| Level | Treatment | Use |
|---|---|---|
| Flat | No shadow, no border | Full-bleed tiles, global nav, footer |
| Soft hairline | 1px warm border `{colors.hairline}` | Utility cards (Apple's approach with Claude's color) |
| Backdrop blur | `backdrop-filter: blur(20px) saturate(180%)` | Sub-nav frosted (Apple) and sticky bars |
| Product shadow | `rgba(0,0,0,0.22) 3px 5px 30px` | Product renders resting on a surface — from Apple |
| Card shadow (new) | `0 1px 3px rgba(20,20,19,0.06)` | Subtle elevation for Claude-style feature cards |

**Philosophy:** Apple's single-shadow rule applies to product imagery. Claude's subtle card shadow is permitted only on cream feature cards (never on tiles).

---

## Shapes

| Token | Value | Use |
|---|---|---|
| `{rounded.none}` | 0px | Full-bleed product tiles — from Apple |
| `{rounded.xs}` | 4px | Tiny accents — from Claude |
| `{rounded.sm}` | 6px | Inline buttons — from Claude |
| `{rounded.md}` | 8px | Standard CTAs, inputs, tabs — from Claude |
| `{rounded.lg}` | 12px | Content cards, feature cards — from Claude |
| `{rounded.xl}` | 16px | Hero illustration container — from Claude |
| `{rounded.pill}` | 9999px | Primary CTAs, configurator chips — from Apple |
| `{rounded.full}` | 9999px | Circular icons — shared |

**Rule:** `{rounded.pill}` remains the Apple signature for primary CTAs and product interactions. `{rounded.md}` (8px) is used for secondary buttons and inputs (Claude's influence).

---

## Components

### Top Navigation

**`global-nav`** — Apple's ultra-thin black nav bar. Background `{colors.surface-black}` (#000000), height 44px, text `{colors.body-on-dark}` in `{typography.nav-link}` (12px/400). Right-aligned cluster: Search, Bag icons.

**`sub-nav-frosted`** — Surface-specific nav. Background `{colors.canvas-parchment}` at 80% opacity with backdrop-filter blur. Height 52px. Category name in `{typography.tagline}` (21px/600). Inline links in `{typography.button}` (14px/500), ending in `{component.button-primary}`.

### Buttons

**`button-primary`** — Apple Action Blue pill. Background `{colors.primary}` (#0066cc), text `{colors.body-on-dark}` (#faf9f5 — cream-tinted white), `{typography.button}` (14px/500), `{rounded.pill}`, padding 11px × 22px. Active: `transform: scale(0.95)`. Focus: 2px `{colors.primary-focus}` outline.

**`button-secondary-pill`** — Ghost pill. Transparent background, `{colors.primary}` text, 1px `{colors.primary}` border, `{rounded.pill}`, same padding.

**`button-secondary`** — Cream button with hairline. Background `{colors.canvas}`, text `{colors.ink}`, `{rounded.md}` (8px), padding 12px × 20px. Used for secondary actions on cream surfaces.

**`button-dark-utility`** — Apple utility. Background `{colors.ink}`, text `{colors.body-on-dark}`, `{rounded.sm}` (6px — from Claude), padding 8px × 15px.

**`button-store-hero`** — Larger primary CTA. Same Action Blue, `{typography.button}` at 18px/400 (Apple's weight 300 replaced with 400 for consistency), padding 14px × 28px.

**`button-icon-circular`** — 44px circular control. Background `rgba(210,210,215,0.64)`, icon in `{colors.ink}`, `{rounded.full}`.

**`text-link`** — Inline links in `{colors.primary}` (Action Blue). Underlined on hover.

**`text-link-on-dark`** — Inline links on dark tiles in `{colors.primary-on-dark}` (Twilight Blue #4a7c9e).

### Cards & Containers

**`product-tile-cream`** — Full-bleed cream tile. Background `{colors.canvas}` (#faf9f5), text `{colors.ink}`, `{rounded.none}`, padding `{spacing.section}` (88px). Centered: product name in `{typography.display-lg}` (40px/600 SF Pro) → tagline in `{typography.lead}` → two pill CTAs → product render with system shadow.

**`product-tile-parchment`** — Same but `{colors.canvas-parchment}` (#f5f0e8 — warmer). Alternates with cream tiles.

**`product-tile-dark`** — Obsidian tile. Background `{colors.surface-tile-dark}` (#1f1f1e), text `{colors.body-on-dark}`, `{rounded.none}`, padding `{spacing.section}`. Same stack with `{component.text-link-on-dark}`.

**`feature-card`** — Claude-style cream feature card. Background `{colors.surface-card}` (#efe9de), `{rounded.lg}` (12px), padding `{spacing.xl}` (32px). Used in 3-up grids for editorial content. Carries a small icon, `{typography.display-md}` headline (SF Pro Text 34px/600 — Apple's style), and body description.

**`code-window-card`** — Claude's dark code editor card. Background `{colors.surface-tile-dark-2}` (#252320), `{rounded.lg}`, padding `{spacing.lg}` (24px). Internal code block in `{typography.code}` (JetBrains Mono). Signature for developer-focused pages.

**`store-utility-card`** — Apple store grid card. Background `{colors.canvas}`, 1px `{colors.hairline}` border, `{rounded.lg}` (12px — merged), padding `{spacing.lg}` (24px). Product image (1:1 crop), name in `{typography.body-strong}`, price, `{component.text-link}`.

**`configurator-option-chip`** — Apple pill. Background `{colors.canvas}`, `{rounded.pill}`, padding 12px × 16px. Thumbnail + label + price.

**`callout-card-coral`** — Claude's coral callout card. Background `{colors.secondary}` (#cc785c), text `{colors.body-on-dark}`, `{rounded.lg}` (12px), padding `{spacing.xxl}` (48px). Used sparingly for major CTAs.

**`floating-sticky-bar`** — Apple's sticky buy bar. Background `{colors.canvas-parchment}` at 80% with blur, height 64px. Left: running price. Right: `{component.button-primary}`.

**`environment-quote-card`** — Apple's photographic hero. Dark photographic backdrop with `{colors.surface-tile-dark}` fallback, centered white text, `{component.button-primary}` below.

**`hero-band`** — Claude's cream hero with 6-6 grid. Background `{colors.canvas}`, padding `{spacing.section}`. Left: `{typography.hero-display}` (Copernicus serif 56px), sub-head, buttons. Right: product mockup or illustration card.

### Inputs & Forms

**`search-input`** — Apple's pill input. Background `{colors.canvas}`, text `{colors.ink}`, `{typography.body}` (17px — Apple's 17px!), 1px `{colors.hairline}` border, `{rounded.pill}`, padding 12px × 20px, height 44px.

**`text-input`** — Claude's rectangular input. Background `{colors.canvas}`, `{rounded.md}` (8px), `{typography.body}` (17px — adapted), padding 10px × 14px, height 40px. Used in forms and sign-up flows.

### Tags & Badges

**`badge-pill`** — Apple pill for categories. Background `{colors.surface-card}`, text `{colors.ink}`, `{typography.caption}` (14px), `{rounded.pill}`, padding 4px × 12px.

**`badge-coral`** — Coral fill for "NEW", "BETA". Background `{colors.secondary}`, text `{colors.body-on-dark}`, `{typography.caption-strong}` (14px/600), `{rounded.pill}`, padding 4px × 12px.

### Footer

**`footer`** — Background `{colors.canvas-parchment}` (#f5f0e8), text `{colors.body-muted}` (#6c6a64). Link columns in `{typography.dense-link}` (17px/400/2.41 — Apple's relaxed leading). Column headings in `{typography.caption-strong}`. Legal in `{typography.fine-print}`. Padding 64px.

---

## Responsive Behavior

### Breakpoints
| Name | Width | Key Changes |
|---|---|---|
| Small phone | ≤ 419px | Single-column tiles; hero typography drops; Copernicus hero 56→32px |
| Phone | 420–640px | Single-column stack; product renders scale |
| Tablet portrait | 736–833px | Global nav collapses to hamburger |
| Tablet landscape | 834–1023px | 3-column utility grids become 2-column |
| Small desktop | 1024–1068px | Product tiles use 2/3 width |
| Desktop | 1069–1440px | Full layout; 4–5 column grids |
| Wide | ≥ 1441px | Content locks at 1440px |

### Touch Targets
- Minimum 44 × 44px (Apple's requirement).
- `{component.button-primary}` at ~44 × 100px.
- `{component.button-icon-circular}` at 44 × 44px.

---

## Do's and Don'ts

### Do
- Use `{colors.canvas}` (#faf9f5) as the default light tile — the warm cream is the merged brand's differentiator.
- Use `{colors.primary}` (Action Blue #0066cc) for all primary interactive elements — links, pill CTAs, focus signals.
- Reserve Copernicus serif for the `hero-display` only — establishes warmth, then transitions to SF Pro.
- Run body copy at `{typography.body}` (17px/400/1.47/-0.374px) — Apple's signature 17px.
- Alternate cream and dark tiles for full-bleed section rhythm. The color change IS the divider.
- Reserve `{rounded.pill}` for primary CTAs and product interactions (Apple's signature).
- Apply the single product-shadow only to product renders resting on a surface — never on cards or buttons.
- Use `{colors.secondary}` (coral #cc785c) sparingly for badges, "new" tags, and select callout moments.
- Use `{component.code-window-card}` to show actual product chrome on developer-focused pages.

### Don't
- Don't introduce a second accent color beyond Action Blue and Coral. Every "click me" signal is Action Blue.
- Don't set body copy at weight 500 — Apple's ladder is 300/400/600/700. Body is 400; strong is 600.
- Don't round full-bleed tiles — tiles are rectangular and edge-to-edge.
- Don't use Copernicus for body copy or for any headline below hero level — it's the signature hero voice only.
- Don't mix radii grammars — pills are `{rounded.pill}`, CTAs are `{rounded.md}` (8px), content cards are `{rounded.lg}` (12px).
- Don't use pure white as the default canvas — cream is the brand.
- Don't add shadows to cards or buttons — shadow is reserved for product imagery.
- Don't use `{colors.primary-on-dark}` (Twilight Blue) on light surfaces — it's the dark-tile-only variant.

---

## What's Preserved from Each System

### From Apple
- Action Blue (#0066cc) as the single primary interactive color
- SF Pro Display + SF Pro Text type system
- 17px body copy
- Edge-to-edge tile alternation (light ↔ dark)
- `{rounded.pill}` for primary CTAs
- Single product-shadow reserved for imagery
- `transform: scale(0.95)` as active state
- Tight negative letter-spacing on headlines
- Weight 500 absent from display hierarchy
- Global nav (pure black, 44px)
- Floating sticky bar
- Configurator chips
- Store utility cards

### From Claude
- Cream canvas (#faf9f5) as the default light tile
- Warm parchment variants (#f5f0e8, #efe9de)
- Copernicus serif for hero display
- Coral (#cc785c) as secondary accent
- Dark navy/Obsidian tiles (#1f1f1e)
- Warm ink (#141413) and muted text (#6c6a64)
- Code window cards (JetBrains Mono)
- `{rounded.md}` (8px) for CTAs and inputs
- `{rounded.lg}` (12px) for content cards
- Feature cards with 32px internal padding
- Coral callout cards
- Weight 500 allowed on button labels

---

## Usage Notes for AI Agents

When generating components from this merged system:

1. **Canvas default:** Always start with `{colors.canvas}` (#faf9f5) — the cream tint IS the brand.
2. **Primary CTA:** Use `{component.button-primary}` — Action Blue pill.
3. **Hero headline:** Use `{typography.hero-display}` — Copernicus serif 56px/400/-0.5px. This is the one place where serif appears.
4. **All other headlines:** Use SF Pro Display with Apple's negative tracking.
5. **Body:** SF Pro Text at 17px/400/1.47/-0.374px — Apple's signature.
6. **Tile rhythm:** Alternating cream ↔ obsidian. The color change IS the divider.
7. **Badges:** Coral for "NEW", "BETA". Pills otherwise.
8. **Code:** Use `{component.code-window-card}` on dark surfaces with JetBrains Mono.
9. **Spacing:** Section padding at 88px (midpoint between Apple's 80px and Claude's 96px).
10. **Shadows:** Only on product imagery. Exception: feature cards may use `0 1px 3px rgba(20,20,19,0.06)` for subtle elevation.
