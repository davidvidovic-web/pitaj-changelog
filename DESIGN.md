---
name: Pitaj.io Novosti
description: A programme guide for release notes: strict grid, one sans family, 3px ink rules, a sticky release numeral.
colors:
  paper: "#f6f6f4"
  paper-sunk: "#ecece9"
  ink: "#0b0b0f"
  ink-soft: "#35353b"
  muted: "#5a5a62"
  hairline: "rgba(11, 11, 15, 0.2)"
  programme-blue: "#2563eb"
  signal-green: "#047857"
typography:
  display:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "clamp(42px, 6.2vw, 76px)"
    fontWeight: 900
    lineHeight: 1
    letterSpacing: "-0.035em"
  numeral:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "clamp(88px, 9vw, 128px)"
    fontWeight: 900
    lineHeight: 0.8
    letterSpacing: "-0.05em"
  headline:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "clamp(28px, 3.2vw, 40px)"
    fontWeight: 900
    lineHeight: 1.1
    letterSpacing: "-0.03em"
  title:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "19px"
    fontWeight: 700
    lineHeight: 1.25
    letterSpacing: "-0.01em"
  body:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.65
  label:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "11px"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "0.08em"
  code:
    fontFamily: "JetBrains Mono, ui-monospace, monospace"
    fontSize: "0.86em"
    fontWeight: 500
rounded:
  none: "0px"
  circle: "50%"
spacing:
  gutter: "48px"
  gutter-tablet: "24px"
  gutter-phone: "16px"
  rail: "208px"
  issue-mark: "172px"
  tile: "44px"
  row-pad: "22px"
components:
  rule-heavy:
    height: "3px"
    backgroundColor: "{colors.ink}"
  tile-blue:
    backgroundColor: "{colors.programme-blue}"
    textColor: "{colors.paper}"
    rounded: "{rounded.none}"
    size: "44px"
  tile-ink:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper}"
    rounded: "{rounded.none}"
    size: "44px"
  tile-green:
    backgroundColor: "{colors.signal-green}"
    textColor: "{colors.paper}"
    rounded: "{rounded.none}"
    size: "44px"
  tile-circle:
    rounded: "{rounded.circle}"
    size: "44px"
  numeral:
    typography: "{typography.numeral}"
    textColor: "{colors.ink}"
  numeral-latest:
    typography: "{typography.numeral}"
    textColor: "{colors.programme-blue}"
  rail-link:
    typography: "{typography.body}"
    textColor: "{colors.muted}"
    padding: "11px 0"
  rail-link-current:
    textColor: "{colors.ink}"
  code-inline:
    backgroundColor: "{colors.paper-sunk}"
    textColor: "{colors.ink}"
    typography: "{typography.code}"
    padding: "1px 5px"
---

# Design System: Pitaj.io Novosti

## Overview

**Creative North Star: "The Programme Guide"**

Every release is one issue of a printed programme: a strict two-level grid, a rail that lists the issues, and one huge release numeral that stays put while its issue scrolls. The world is Program Sarajevo '84 meeting Pitaj.io: neutral paper, the logo's near-black ink, a single programme blue, and a signal green reserved for reliability and privacy. It reads as an institution's schedule, not as a SaaS changelog.

Structure is made of rules, not boxes. A 3px ink rule opens each issue, the masthead and the colophon; 1px hairlines separate rows. Sections are rows (pictogram tile, heading, bullet list), never cards. One sans family (Archivo, with its width axis for narrow labels) carries all roles; a mono face appears only for code. Light and dark follow the OS (`prefers-color-scheme`), with the same roles remapped.

The build rejects rounded cards, pills, shadows and gradients. Circles are the one round form, and only on conversation-type pictogram tiles.

**Key Characteristics:**
- Flat: no shadows, no gradients, no rounded containers.
- 3px ink rules for hierarchy, 1px hairlines for rows.
- One family, tabular numerals everywhere.
- Blue is the single programme colour; green is for infra and privacy only.
- Tile shape (circle vs square) and text carry state and category; colour only reinforces.
- Sticky release numeral as signature.

## Colors

A restrained paper-and-ink palette with one blue and one green; ink does most of the work.

### Primary
- **Programme Blue** (#2563eb light, #8fb0ff dark): the single programme colour. Latest-issue numeral, bullet squares, "Novo" flag square, current rail date, focus ring, in-content links, selection, default tile fill.

### Secondary
- **Signal Green** (#047857 light, #5fd1a4 dark): reliability and privacy. Privacy note icon and tiles for infra and privacy sections only.

### Neutral
- **Paper** (#f6f6f4 light, #0e0e11 dark): page background.
- **Paper Sunk** (#ecece9 light, #17171b dark): inline code and code blocks.
- **Ink** (#0b0b0f light, #f4f4f2 dark): headings, numerals, rules, ink tiles, logo block.
- **Ink Soft** (#35353b light, #d2d2d6 dark): body text.
- **Muted** (#5a5a62 light, #a0a0a9 dark): metadata, inactive rail entries, footer.
- **Hairline** (rgba(11,11,15,0.2) light, rgba(244,244,242,0.22) dark): row dividers, link underlines at rest.

### Named Rules
**The One Programme Colour Rule.** Blue is the only accent. Green appears only on reliability and privacy. Do not add a third hue.

**The Shape Before Hue Rule.** Category and state are told by tile shape (circle for conversation, square for the rest), a "Novo" word and a square marker, and bold weight on the current rail entry. Colour is never the only signal.

## Typography

**Display Font:** Archivo (variable, wdth 62..125, wght 100..900; fallback system-ui, sans-serif)
**Body Font:** Archivo
**Label/Mono Font:** JetBrains Mono (400/500), code only

**Character:** One heavy grotesque family, tight-tracked at weight 900 for numerals and titles, with the width axis (75-85%) condensing small caps labels and nav links. Tabular numerals are on at the body level.

### Hierarchy
- **Display** (900, clamp(42px, 6.2vw, 76px), 1.0, -0.035em): page title, max 18ch.
- **Numeral** (900, clamp(88px, 9vw, 128px), 0.8, -0.05em; 80px under 960px): release number, sticky, blue when latest.
- **Headline** (900, clamp(28px, 3.2vw, 40px), 1.1, -0.03em): release title.
- **Title** (700, 19px, 1.25, -0.01em): section heading beside its tile; pager titles at 20px.
- **Body** (400, 17px, 1.65): base. Release lead 19px; page lead 20px; list items 16.5px; measure 68ch.
- **Label** (700, 11-13px, 0.08-0.12em, uppercase, width 75% on the rail heading): "Novo" flag, rail heading.
- **Code** (JetBrains Mono 500, 0.86em inline, 14px blocks).

### Named Rules
**The One Family Rule.** Everything is Archivo; hierarchy comes from weight (400/500/700/900), size and width, never a second text face.

## Layout

A page is 1280px max with 48px gutters (24px under 960px, 16px under 520px). The index is a two-column grid: a 208px sticky rail (24px from top) and a fluid main column, 48px apart. Each issue is a nested grid: a 172px mark column (sticky numeral and meta) and the content, 40px apart. Content rows are three columns: 68px tile, 220px heading, fluid list; the release title and lead span all columns. Rows get 22px vertical padding, separated by hairlines; lists cap at 68ch.

Under 960px the rail becomes a horizontal scrolling strip (dates and "Novo" hidden), the mark becomes a numeral-plus-meta flex row, and content rows collapse to a 56px tile and fluid column with the list full width. Pager stacks to one column.

## Elevation & Depth

Flat by design. No shadows, no gradients. Depth is hierarchy of rules: 3px ink rules mark major breaks, hairlines mark rows, and a tonal step (Paper Sunk) marks code.

### Named Rules
**The Rules Not Boxes Rule.** Separate with a rule or whitespace; never with a shadow, border box or fill panel.

## Shapes

Square and rectilinear. Radius is 0 everywhere. The single exception is the circle (50%) on conversation-type pictogram tiles (chat, bot, omnichannel, tickets, brain), which is a category signal, not decoration. Bullets are 6px squares; the "Novo" marker is a 7px square. Pictograms are Lucide line icons at 22px, stroke 2, inside a 44px tile.

## Components

### Pictogram Tile
- 44px square (or circle for conversation sections), solid fill, icon at 22px.
- Tones: blue (default), ink (infrastructure-like: crawler, sync, cdn, code, docs, wordpress, building), green (infra, privacy). Fallback icon is Sparkles.
- Decorative (aria-hidden); the heading carries the meaning.

### Release Issue
- Opens with a 3px ink rule. Mark column: sticky numeral (top 24px), then meta: version (700, 16px, ink), date (14px, muted), optional "Novo" flag, and an "Open" link with a 1px ink underline and a 14px arrow that turns blue on hover.
- Content: headline, lead, then section rows.

### Release Rail
- Heading "Program izdanja" (uppercase label) with a zero-padded count in muted. Entries are version plus short date (dd.mm.), 1px hairline between.
- Default muted; hover ink; current entry ink and bold with a blue date, set by scroll position (IntersectionObserver, `aria-current`). Newest carries "Novo" with a blue square.

### Navigation (Masthead)
- Logo block (ink square, paper P, 3px corner), wordmark "Pitaj" 900 with blue ".io", then a hairline-separated "Novosti" in muted. Links 15px, weight 500, width 85%, ink, underline on hover. Sits on a 3px ink rule; links wrap below the brand under 520px.

### Pager and Colophon
- Pager: two columns under a 3px ink rule, 20px bold titles that turn blue on hover, muted caption; next is right-aligned (left on mobile).
- Colophon: 3px ink rule, 14px muted text, ink links.

### Links and Focus
- Links inherit colour with a hairline underline that becomes solid on hover; in-content links are blue. Focus is a 3px blue outline offset 3px. A skip link appears fixed top-left on focus. Smooth scroll is disabled under reduced motion. No other motion is used.

## Do's and Don'ts

### Do:
- **Do** open each major block with a 3px ink rule and separate rows with 1px hairlines.
- **Do** keep blue as the only accent; use green only for infra and privacy.
- **Do** make sections rows of tile, heading and list, with tile shape as the category signal.
- **Do** use Archivo for everything and keep tabular numerals on.
- **Do** keep text lines to 68ch and the page to 1280px.
- **Do** swap to the dark values through the same custom properties, not new colours.

### Don't:
- **Don't** use rounded cards, pills, shadows or gradients.
- **Don't** introduce a third accent hue or rely on colour alone to mark state.
- **Don't** add a second text typeface; mono is for code only.
- **Don't** add a hero or a "latest" tile that sets the newest release apart from the feed; the numeral in blue is the only mark.
- **Don't** put circles on anything but conversation-type pictogram tiles.
