---
version: alpha
name: Groq
website: "https://groq.com"
description: >-
  Groq's 2026 marketing system is a hardware-inference brand built on a cream canvas (#f3f3ee) with charcoal ink (#2d2f33), a single hot-orange voltage at #f43e01 reserved for CTAs and overlines, Space Grotesk display weight 300 at 46px with -0.92px tracking, and a parallel IBM Plex Mono lane running uppercase eyebrows at 12px / 1.2px letter-spacing — the orange pill button, the mono overline, and the deep-charcoal product render are the three load-bearing moves.

seo:
  title: "Groq Design System for React — #f43e01 orange, Space Grotesk 300, 18 components"
  metaDescription: "Groq's LPU inference design system as a DESIGN.md file. #f43e01 orange, Space Grotesk weight 300, IBM Plex Mono overlines, 22 colors, 18 components. For React, Next.js, and AI tools."
  highlights:
    - "Single-pill voltage — #f43e01 orange used as the only filled CTA (1000px radius), every secondary action is a transparent text link"
    - "Display at weight 300 — Space Grotesk runs 46px / 32px / 28px at fontWeight 300 with negative tracking, refusing the heavy grotesque convention of the AI-infra category"
    - "Mono overline lane — IBM Plex Mono at 12px / 500 / 1.2px letter-spacing carries every uppercase eyebrow above the headline, giving the page a chip-spec cadence"
    - "Pill-or-rectangle, nothing between — radii cluster at 1000px (15 uses) for pills and 10px (11 uses) for outer cards, with 5px / 3px reserved for inline code chips"
    - "Fluorescent reserve palette — purple #d377fd, green #10e68d, yellow #fdeb20 ship in CSS variables but render zero times on the home surface, kept for code-snippet syntax and dashboard chrome"
  tags:
    - "AI & LLM Platforms"
    - "Hardware & Robotics"
  lastUpdated: "2026-05-13"
  author:
    name: "Dov Azencot"
    url: "https://x.com/dovazencot"
  opening: |
    Groq sells inference on a custom LPU chip, and the marketing surface refuses every AI-infrastructure visual cliche. There is no purple-to-blue gradient mesh, no animated globe, no glassmorphic console screenshot. The canvas is a warm bone (#f3f3ee) — not white, not gray — sitting under charcoal ink (#2d2f33) that handles every paragraph, nav link, and rule. The only chromatic event on the page is a single Groq orange (#f43e01) doing three jobs: it fills the primary pill CTA at 1000px radius, paints the uppercase mono overline above each section headline, and underlines hovered link text. Everything else — the McLaren F1 hero card, the rack-mounted LPU photograph, the OpenAI-compatibility code well — renders in black, cream, or charcoal.

    This page packages the captured system as a single DESIGN.md file written to the Google Labs spec. Inside the frontmatter: 22 color tokens covering the bone canvas, the charcoal ink ladder, the orange voltage with its pressed variant, and a five-stop fluorescent reserve (purple, green, yellow, blue, pink) that ships in CSS variables but never appears on the home surface. There are 12 typography tokens split across two families — Space Grotesk for every display tier and body line, IBM Plex Mono for overlines and inline code — plus 4 radii, 8 spacing values from 4px to 80px, and 18 components covering the pill primary CTA, the bordered secondary, the dark code well at #2d2f33, the McLaren-style media card, and the bottom "Build Fast" full-bleed orange band.

    Feed the file to Claude, Cursor, or GitHub Copilot and the agent will write React and Tailwind that match Groq's discipline: cream canvas, weight-300 display, mono overlines, scarce orange. The result is not a generic AI-infra dark theme — it's an inference-hardware product brochure that trusts a single voltage hex to carry every call to action across the page. Read it as a reference if you are building any developer-facing platform where the brand needs to feel both technical and warmly editorial, and where the convention to default to dark canvases and saturated gradients is exactly what you want to avoid.
  related:
    - href: "/design"
      title: "Browse all design systems"
      description: "The full directory of DESIGN.md files on shadcn.io, with live mockups for each."
    - href: "https://groq.com"
      title: "Groq — official site"
      description: "The marketing site this DESIGN.md was extracted from — fast, low-cost inference on the LPU."
    - href: "https://github.com/google-labs-code/design.md"
      title: "The DESIGN.md specification"
      description: "Google Labs' open spec for machine-readable design system files — the format this page is built on."
  questions:
    - id: "primary-color"
      title: "What is Groq's primary brand color?"
      answer: "Groq's brand voltage is #f43e01 — a hot orange shipped as --color-orange-brand and exposed under eight aliases including --color-text-accent, --color-icon, --color-focus-btn, and --color-overline. The token appears 42 times on the home surface: 10 background fills (primary CTAs, the bottom Build Fast band), 16 text uses (uppercase mono overlines, hovered link color), and 16 border uses (focus rings, icon strokes). A pressed variant #c23101 carries link-hover state. Every other section is charcoal and bone — orange is the single chromatic event."
    - id: "typography"
      title: "What typography does Groq use, and what's the weight strategy?"
      answer: "Groq runs two families with no third option. Space Grotesk handles every display tier and every body line, from the 46px h2 hero headline down to 15px nav links and paragraph copy. IBM Plex Mono handles only two roles — 12px uppercase overlines at fontWeight 500 with 1.2px letter-spacing, and 14px code-snippet body. The weight strategy is the load-bearing decision: every display size (46px, 36px, 32px, 28px) renders at fontWeight 300 with negative letter-spacing (-0.92px / -0.72px / -0.64px / -0.56px), while body and UI hold at fontWeight 400. There are zero weight-600 or weight-700 occurrences on the home page."
    - id: "shape-language"
      title: "Why are buttons fully rounded but cards aren't?"
      answer: "The radius scale clusters at exactly two values. The 1000px full pill (`--bdrs-l`) appears 15 times — every interactive control: the orange primary CTA, the transparent-bordered secondary, the nav pill, the small badges over hero media. The 10px rectangular radius (`--bdrs-outer`) appears 11 times — every content surface: the McLaren video card, the dark code well, the data-table panel. A 5px inner radius (`--bdrs-inner`) handles inline code chips, and 3px is reserved for thumbnails. The split is structural: anything you tap is a pill, anything that holds content is a soft rectangle."
    - id: "fluorescent-palette"
      title: "What are the fluorescent purple, green, yellow, blue, pink tokens for?"
      answer: "Groq ships a five-stop fluorescent reserve in CSS variables — purple #d377fd, green #10e68d, yellow #fdeb20, blue #5fc0ff, pink #f392dd, each with a light tint — but every one of them renders zero times on the home surface. The strongest signal is `--color-code-snippet-highlight: #d377fd`: the purple is reserved for syntax highlighting inside dark code wells on developer-doc pages. The green carries dashboard chart accents on the GroqCloud inference-share bar (visible in the home survey chart). Treat the fluorescent stops as documented runway for inner-product surfaces, not as marketing palette extensions — promoting any of them to a hero CTA breaks the single-voltage rule."
    - id: "overline-pattern"
      title: "Why does every section start with a tiny orange uppercase line?"
      answer: "The IBM Plex Mono overline is the page's structural rhythm. Every section above the headline carries a 12px uppercase eyebrow at fontWeight 500 with 1.2px letter-spacing, colored in the brand orange (#f43e01) via `--color-overline`. It runs 17 times on the home page. The pattern reads as chip-spec metadata — borrowed from datasheet typography rather than marketing — and reinforces the inference-hardware positioning. Without the overline the page would lose its measured cadence; with it, every section feels like a labeled row in a technical reference document."
    - id: "use-in-project"
      title: "Can I use this DESIGN.md to build a developer-facing platform with shadcn/ui?"
      answer: "Yes — the file is built for AI coding tools that read structured tokens. Drop it into Claude, Cursor, or Windsurf alongside your component request and the agent will reproduce Groq's discipline: bone canvas, scarce orange, weight-300 display, mono overlines, pill CTAs at 1000px radius, content cards at 10px. Every color, type style, radius, and spacing value is quoted as a literal hex or px string ready for Tailwind config, CSS variables, or shadcn/ui registry tokens. Pair it with `/blocks` for hero, pricing, and CTA sections that already match the typographic restraint Groq uses."

colors:
  primary: "#f43e01"
  primary-pressed: "#c23101"
  primary-light: "#ffd1a3"
  ink: "#2d2f33"
  ink-soft: "#69695d"
  ink-muted: "#9c9c90"
  hairline: "#cecebf"
  canvas: "#f3f3ee"
  surface: "#ffffff"
  surface-elevated: "#e8e8de"
  surface-dark: "#2d2f33"
  on-dark: "#ffffff"
  black: "#000000"
  navy-deep: "#2c364a"
  navy-mid: "#3e4c69"
  fluor-purple: "#d377fd"
  fluor-green: "#10e68d"
  fluor-yellow: "#fdeb20"
  fluor-blue: "#5fc0ff"
  fluor-pink: "#f392dd"
  yellow-warn: "#f6ab45"
  swiper-blue: "#007aff"

typography:
  display-xl:
    fontFamily: "Space Grotesk, Space Grotesk Fallback, system-ui, sans-serif"
    fontSize: 46px
    fontWeight: 300
    lineHeight: 1.3
    letterSpacing: "-0.92px"
  display-lg:
    fontFamily: "Space Grotesk, Space Grotesk Fallback, system-ui, sans-serif"
    fontSize: 36px
    fontWeight: 300
    lineHeight: 1.3
    letterSpacing: "-0.72px"
  display-md:
    fontFamily: "Space Grotesk, Space Grotesk Fallback, system-ui, sans-serif"
    fontSize: 32px
    fontWeight: 300
    lineHeight: 1.3
    letterSpacing: "-0.64px"
  display-sm:
    fontFamily: "Space Grotesk, Space Grotesk Fallback, system-ui, sans-serif"
    fontSize: 28px
    fontWeight: 300
    lineHeight: 1.3
    letterSpacing: "-0.56px"
  heading-md:
    fontFamily: "Space Grotesk, Space Grotesk Fallback, system-ui, sans-serif"
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: "-0.48px"
  heading-sm:
    fontFamily: "Space Grotesk, Space Grotesk Fallback, system-ui, sans-serif"
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: "-0.38px"
  body-lg:
    fontFamily: "Space Grotesk, Space Grotesk Fallback, system-ui, sans-serif"
    fontSize: 21px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0
  body-md:
    fontFamily: "Space Grotesk, Space Grotesk Fallback, system-ui, sans-serif"
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: 0
  body-sm:
    fontFamily: "Space Grotesk, Space Grotesk Fallback, system-ui, sans-serif"
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: 0
  overline:
    fontFamily: "IBM Plex Mono, IBM Plex Mono Fallback, ui-monospace, monospace"
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: "1.2px"
  code-block:
    fontFamily: "IBM Plex Mono, IBM Plex Mono Fallback, ui-monospace, monospace"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.3
    letterSpacing: 0
  caption:
    fontFamily: "Space Grotesk, Space Grotesk Fallback, system-ui, sans-serif"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.57
    letterSpacing: 0

rounded:
  none: "0px"
  xs: "3px"
  sm: "5px"
  md: "10px"
  full: "1000px"

spacing:
  xxs: "4px"
  xs: "8px"
  sm: "12px"
  md: "16px"
  base: "24px"
  lg: "32px"
  xl: "48px"
  section: "80px"

components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-dark}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: "10px 16px"
    border: "0"
  button-primary-hover:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    border: "1px {colors.primary}"
  button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: "10px 16px"
    border: "1px {colors.hairline}"
  button-tertiary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: "10px 16px"
  top-nav:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.body-sm}"
    height: 88px
    padding: "0px 48px"
  nav-link:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    padding: "8px 12px"
  overline:
    backgroundColor: "transparent"
    textColor: "{colors.primary}"
    typography: "{typography.overline}"
  hero-headline:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.display-xl}"
  body-paragraph:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
  media-card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.md}"
    padding: "0"
  section-band-light:
    backgroundColor: "{colors.surface-elevated}"
    textColor: "{colors.ink}"
    padding: "80px 48px"
  section-band-dark:
    backgroundColor: "{colors.surface-dark}"
    textColor: "{colors.on-dark}"
    padding: "80px 48px"
    rounded: "{rounded.md}"
  code-well:
    backgroundColor: "{colors.surface-dark}"
    textColor: "{colors.on-dark}"
    typography: "{typography.code-block}"
    rounded: "{rounded.md}"
    padding: "24px 32px"
  code-highlight:
    backgroundColor: "transparent"
    textColor: "{colors.fluor-purple}"
    typography: "{typography.code-block}"
  data-row:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.body-sm}"
    padding: "16px 0px"
    border: "0"
  cta-banner-orange:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-dark}"
    typography: "{typography.display-md}"
    rounded: "{rounded.md}"
    padding: "80px 48px"
  footer:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.body-sm}"
    padding: "80px 48px"
---

## Overview

Groq's web chrome is hardware-spec restraint wearing a marketing skin — a bone-cream canvas, a single hot-orange voltage, and a typographic system that holds every display headline at weight 300 while pretending the rest of the AI-infrastructure category isn't shouting at weight 700. Where most LPU and GPU vendors anchor their pages on a saturated indigo-to-violet mesh and a glassmorphic console screenshot, Groq holds the entire page on `#f3f3ee` warm bone with charcoal `#2d2f33` ink and the McLaren F1 livery as the only piece of brand atmosphere. The orange — `#f43e01` — appears 42 times across the page and never more than once per viewport.

**Stamped voltage**: the orange is treated as a stamp, not as a palette. It fills exactly one shape — the pill primary CTA at 1000px radius — and stains exactly one role of text — the uppercase mono overline above each section. It never gradients, never tints, never carries a secondary action. Every transparent-border button and every nav link is charcoal on bone.

**Weight as restraint**: the entire display ladder runs at fontWeight 300 — 46px hero, 36px section, 32px sub-section, 28px callout — with negative letter-spacing scaling from -0.92px down to -0.56px. There is not a single weight-600 or weight-700 glyph on the home surface. This is not the convention of the infrastructure category; it is the convention of editorial print.

**Key Characteristics:**
- Single brand voltage (`#f43e01`) used as the only filled CTA color, never as a secondary or as a tint.
- Two-family typographic split — Space Grotesk for everything visual, IBM Plex Mono for overlines and code.
- 1000px pill controls sitting inside 10px rectangular content cards — no in-between radii on the page.
- Bone canvas (`#f3f3ee`) instead of white; charcoal ink (`#2d2f33`) instead of true black.
- Five-stop fluorescent reserve palette shipped in CSS variables but unused on the marketing surface.
- IBM Plex Mono overlines at 12px / fontWeight 500 / 1.2px letter-spacing on every section.
- Dark code well at `#2d2f33` with white type and purple `#d377fd` syntax highlighting.
- Full-bleed orange "Build Fast" CTA band at the page foot — the only large orange surface.

## Colors

### Brand & Accent

- **Groq Orange (`#f43e01`)** — frequency 42. Used as text (16), bg (10), border (16). The single brand voltage; lives in `--color-orange-brand`, `--color-text-accent`, `--color-icon`, `--color-focus-btn`, `--color-overline`. Reserved for the primary pill CTA, the uppercase mono overline above every section, the "Build Fast" footer band, and the focus outline.
- **Pressed Orange (`#c23101`)** — frequency 2. Used as text (1), border (1). Lives in `--color-orange-dark` and `--color-text-link-hover`. The only color shift in the entire page is the link-hover state; even pressed-state CTAs reuse the base orange.
- **Orange Light (`#ffd1a3`)** — frequency 0 on the home surface. Ships in `--color-orange-light` for inline status chips on dashboard surfaces.

### Surface & Background

- **Bone Canvas (`#f3f3ee`)** — frequency 5. Used as bg (5). Lives in `--color-utility-200`, `--color-utility-95-yellow`, `--color-bg`. The dominant page background; warmer than gray-100, cooler than parchment, and the temperature signal that the brand is a hardware company rather than a SaaS dashboard.
- **Soft Elevated (`#e8e8de`)** — frequency 8. Used as bg (6), gradient (2). Lives in `--color-utility-300`, `--color-utility-91-yellow`, `--color-bg-section-91`. Section-band fill behind the GroqCloud chart and the McLaren feature row — half a step darker than canvas without crossing into gray.
- **Surface White (`#ffffff`)** — frequency 111. Used as bg (3), text (54), border (54). The white is for inverted text on dark surfaces and for the rare elevated media card; the page itself is never pure white.
- **Charcoal Surface (`#2d2f33`)** — frequency 650 (the dominant color). Used as text (324), bg (4), border (322). Not black, not gray — a near-neutral charcoal with a hint of cool blue (oklch hue 264). Carries every paragraph, every nav link, every hairline, and inverts to fill the code well and dark product band.

### Text & Rules

- **Ink Soft (`#69695d`)** — frequency 18. Used as text (9), border (9). Lives in `--color-tabs-icon-btn-text`, `--color-text-secondary`. Inactive nav and tab labels, secondary metadata.
- **Ink Muted (`#9c9c90`)** — frequency 4. Used as text (2), border (2). Lives in `--color-code-snippet-text-comment`, `--color-utility-61-yellow`. Code-comment color inside the dark well, footer microcopy.
- **Hairline (`#cecebf`)** — frequency 8. Used as text (4), border (4). Lives in `--color-utility-81-yellow`. Section dividers and the secondary-button stroke.
- **Charcoal Ink (`#2d2f33`)** — see Surface section; this hex serves as both the inverted dark fill and the default text color on light surfaces.

### Fluorescent Reserve

- **Fluorescent Purple (`#d377fd`)** — frequency 0 on home. Lives in `--color-code-snippet-highlight`. Reserved for syntax highlighting inside dark code wells on doc pages.
- **Fluorescent Green (`#10e68d`)** — frequency 0 on home. The GroqCloud chart bar uses this on the inference-share row.
- **Fluorescent Yellow (`#fdeb20`)**, **Blue (`#5fc0ff`)**, **Pink (`#f392dd`)** — frequency 0 each. Documented runway for product surfaces; never deployed on the marketing canvas.

### Semantic

- **Yellow Warn (`#f6ab45`)** — `--color-yellow`. Reserved for status warnings.
- **Navy Deep (`#2c364a`)** / **Navy Mid (`#3e4c69`)** — `--color-utility-29-blue` / `--color-utility-41-blue`. Internal tool palette for tabular surfaces, not used on the home page.

## Typography

### Font Family

- **Display & UI**: `Space Grotesk` with `Space Grotesk Fallback`, then `system-ui`, `Helvetica Neue`, `Helvetica`, `Arial`. Lives in `--ff-display`, `--ff-text`, `--ff-sans`.
- **Mono**: `IBM Plex Mono` with `IBM Plex Mono Fallback`, then `ui-monospace`, `Cascadia Code`, `Source Code Pro`, `Menlo`, `Consolas`. Lives in `--ff-mono`, `--ff-ibm-plex-mono`.
- There is no third family. Headlines, body, captions, button labels — all Space Grotesk. Overlines, code wells, inline commands — all IBM Plex Mono.

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing | Notes |
|---|---|---:|---:|---:|---:|---|
| Display XL | Space Grotesk | 46px | 300 | 1.30 | -0.92px | Section h2 hero headlines. |
| Display LG | Space Grotesk | 36px | 300 | 1.30 | -0.72px | Secondary section headlines. |
| Display MD | Space Grotesk | 32px | 300 | 1.30 | -0.64px | Hero h1 on solution sub-pages. |
| Display SM | Space Grotesk | 28px | 300 | 1.30 | -0.56px | h3 callouts. |
| Heading MD | Space Grotesk | 24px | 400 | 1.30 | -0.48px | Pull-quote body. |
| Heading SM | Space Grotesk | 19px | 400 | 1.30 | -0.38px | Card titles inside dark bands. |
| Body LG | Space Grotesk | 21px | 400 | 1.40 | 0 | Hero subtext paragraphs. |
| Body MD | Space Grotesk | 17px | 400 | 1.40 | 0 | Section body. |
| Body SM | Space Grotesk | 15px | 400 | 1.30 | 0 | Default UI text, nav, buttons. |
| Overline | IBM Plex Mono | 12px | 500 | 1.40 | 1.2px | Uppercase eyebrow above every section. |
| Code Block | IBM Plex Mono | 14px | 400 | 1.30 | 0 | Inside the dark code well. |
| Caption | Space Grotesk | 14px | 400 | 1.57 | 0 | Footer microcopy, dates, metadata. |

### Principles

- Hold every display tier at weight 300 with negative letter-spacing; resist promoting to weight 500 or 600 even when the headline carries the page.
- Use the IBM Plex Mono overline as the structural rhythm marker — every section above the fold and below carries one.
- Keep mono usage to two roles only: uppercase overlines (12px) and code wells (14px). Do not let mono leak into body copy or buttons.
- The base UI size is 15px, not 16px — match Space Grotesk's slightly larger x-height by sitting one step below.

## Layout

### Spacing System

The captured scale runs 4px, 8px, 12px, 16px, 24px, 32px, 48px, and 80px. The dominant spacing value on the page is 32px (18 uses), followed by 16px (12 uses), and the outer section padding is 48px (`--space-outer: 3.43rem`). Hero band vertical padding sits at 80px (`--space-section-top: 5.71rem`), giving every section a generous breath above and below the headline.

### Grid & Container

- Global nav uses a three-zone layout: logo center, menu links left and right of logo, sign-in CTA far right at 88px height.
- Hero alternates between centered single-column text (above the McLaren video card) and split two-column compositions (left media card + right body copy).
- Section bands run full-bleed; content sits inside a 12-column grid with 32px gutters and a 1024px max-width container.
- The OpenAI-compatibility section uses a single full-width dark code well rather than a split syntax/explanation layout.
- The featured-articles strip renders as a three-row rule-separated list with date column left, title column center, source-mark right.

### Whitespace Philosophy

Groq uses vertical empty space as a pacing signal between hardware claim, customer proof, code proof, and CTA. The home page is roughly 4500px tall and every section is separated by at least 80px of bone canvas. Dense content arrives only inside the dark code well and the footer link grid.

## Elevation & Depth

Groq is mostly flat with a measured shadow ladder defined in CSS variables. Depth comes from surface inversion (cream → charcoal), corner radius (10px content cards), and one drop-shadow tier reserved for the floating nav.

| Level | Token | Treatment | Use |
|---|---|---|---|
| 0 | `--elevation-0` | none | Default surfaces, body sections |
| 1 | `--elevation-1` | drop-shadow(0.5px 1px 1px rgba(0,0,0,0.3)) | Inline chips and the McLaren badge over the F1 photo |
| 2 | `--elevation-2` | layered drop-shadows at 2/4/6px | Floating media cards on cream canvas |
| 3 | `--elevation-3` | layered drop-shadows at 2/4/8/16/32px | Modal-tier surfaces (not used on home) |
| 4 | `--elevation-4` | 0 4px 80px rgba(0,0,0,0.04) | Soft ambient lift on the bottom CTA band |

## Shapes

### Radius Scale

| Token | Value | Role |
|---|---:|---|
| `none` | `"0px"` | Full-bleed bands, section dividers |
| `xs` | `"3px"` | Thumbnail rounding inside code wells |
| `sm` | `"5px"` | Inline code chips (`--bdrs-inner`) |
| `md` | `"10px"` | Every content card — McLaren media, code well, data table (`--bdrs-outer`, 11 uses) |
| `full` | `"1000px"` | Every interactive control — primary CTA, secondary button, nav pill (`--bdrs-l`, 15 uses) |

### Image Treatment

Imagery on the home surface is two things only: the McLaren F1 video card at 10px radius (the only photographic warmth on the page) and the LPU rack-mount render at the same radius. There are no decorative illustrations, no abstract 3D shapes, no avatar circles. Every other piece of "imagery" is a code snippet inside the dark well.

## Components

### **`button-primary`**

Filled orange pill at 1000px radius with white 15px Space Grotesk label, 10px / 16px padding, zero border. The single chromatic CTA — appears in the hero ("Get Started"), above each section break, and at the foot of the "Build Fast" banner.

### **`button-primary-hover`**

Inverts to white fill with a 1px orange border and orange label. The only color-shifting CTA state in the captured spec.

### **`button-secondary`**

Transparent fill, 1px hairline border (`#cecebf`), charcoal label. Same 1000px pill geometry as primary, used for "Read Article" and "View Details" in section bands.

### **`button-tertiary`**

White fill, no border, charcoal label. Sits inside the dark code-well section as the "Copy" affordance.

### **`top-nav`**

Cream-canvas nav band, 88px tall, 48px horizontal padding, logo centered with links splitting left/right around it and the "Get Started" pill anchored far right.

### **`nav-link`**

Charcoal 15px Space Grotesk on transparent background, 8px / 12px padding, 1000px hit-target radius. No underline, no separator marks — links rely on hover state for affordance.

### **`overline`**

Uppercase IBM Plex Mono 12px / fontWeight 500 / 1.2px letter-spacing, colored Groq orange. Appears 17 times — once at the top of every distinct section.

### **`hero-headline`**

Space Grotesk 46px / fontWeight 300 / -0.92px tracking. Carries the strongest typographic identity on the page — the absence of weight is what reads as confidence.

### **`body-paragraph`**

Space Grotesk 17px / fontWeight 400 / lineHeight 1.4 on charcoal. The workhorse paragraph style across hero subtext and section copy.

### **`media-card`**

White surface, 10px radius, zero padding (content is full-bleed image or video). The McLaren video card, the LPU rack render, and the customer testimonial photos all use this geometry.

### **`section-band-light`**

Soft elevated fill (`#e8e8de`) running full-bleed with 80px / 48px padding. Used for the GroqCloud bar-chart section and the featured-articles strip.

### **`section-band-dark`**

Charcoal surface (`#2d2f33`) at 10px outer radius (when contained) with white type and 80px / 48px padding. Carries the McLaren racing video band.

### **`code-well`**

Charcoal `#2d2f33` background, white IBM Plex Mono 14px type, fluorescent purple `#d377fd` syntax highlighting, 10px radius, 24px / 32px padding. The OpenAI-compatibility section is a single full-width code well.

### **`code-highlight`**

Inline mono span colored fluorescent purple — the only fluorescent token that renders on the home page, and only inside the code well.

### **`data-row`**

Rule-separated row on canvas with charcoal Space Grotesk 15px text and 16px vertical padding. Used in the featured-articles three-row list.

### **`cta-banner-orange`**

Full-bleed Groq orange (`#f43e01`) band at the page foot, 80px / 48px padding, 10px outer radius when contained, white 32px display type centered above a white-fill secondary CTA. The only large orange surface on the page.

### **`footer`**

Cream canvas continuing from the page body, 80px / 48px padding, four-column link grid in charcoal 15px Space Grotesk. No background change — the footer reads as the natural continuation of the page rather than a sealed band.

## Do's and Don'ts

### Do

- Hold every display tier at fontWeight 300 with negative letter-spacing; resist the AI-infra default of weight 600+.
- Use `#f43e01` as the only filled accent color and reserve it for primary CTAs and uppercase overlines.
- Open every section with a 12px IBM Plex Mono overline at 1.2px letter-spacing.
- Use 1000px radius on interactive controls and 10px on content cards — never a value in between.
- Render the canvas as `#f3f3ee` bone, not `#ffffff` white.

### Don't

- Don't promote the fluorescent purple (`#d377fd`) to a marketing surface — it's reserved for code-snippet highlights (`--color-code-snippet-highlight`) and renders zero times on the home page. Use Groq orange (`#f43e01`) for any non-code accent.
- Don't render display headlines at weight 500 or above — the captured ladder is strictly weight 300, and bumping to 500 reads as a third-party page mistakenly using the Groq palette.
- Don't use the `#69695d` ink-soft for body paragraphs — it's the inactive-tab and footer-metadata token (18 uses, half text half border). Default paragraph color is `#2d2f33` charcoal.
- Don't add a secondary filled-color button (blue, green, dark). The captured spec defines exactly two button surfaces: filled orange and transparent-border charcoal.
- Don't apply 5px (`--bdrs-inner`) radius to anything larger than an inline code chip — the inner radius is a 4-use token reserved for character-scale containers, not card-scale geometry.
- Don't replace the IBM Plex Mono overline with a Space Grotesk small-caps treatment — the mono lane is the page's structural rhythm marker and renders 17 times across the home page.

## Known Gaps

- Active and pressed component states are captured only for `button-primary-hover` (white fill, orange border) and the `link-hover` color shift to `#c23101`. Focus rings extracted via `--color-focus-outline: #f43e01` but per-component focus visuals are not broken out as variants.
- The logged-in GroqCloud console, the inference dashboard, and the API-key management surfaces live behind authentication and were not part of the home-page capture. The five-stop fluorescent reserve (purple, green, yellow, blue, pink) is documented as runway for those surfaces.
- Mobile screenshots were not regenerated in this capture; mobile behavior is inferred from the existing `--max-nav-media-query: (max-width: 67.5em)` breakpoint and the `--grid-col-width` calc — the 12-column grid collapses to a single column below 1080px.

