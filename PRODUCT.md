# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Astro 7 with MDX content collections and Sass (existing; the user confirmed it stays). Content lives in `src/content/releases/*.mdx`, one file per release, deployed as a static site (changelog.pitaj.io).

## Users

Customers who run AI agents on Pitaj.io: business owners and the operators who manage agents, conversations, widgets and the knowledge base. They open the changelog to see quickly what is new and whether it affects their own agent or workflow. (Confirmed as the primary reader. Integrators and prospects are secondary and not designed for first.)

## Product Purpose

The public release notes of the Pitaj.io platform (AI agents/chat widget for websites, with knowledge base crawler, procedures, widgets, product catalog, live operator takeover). The changelog tells customers what changed and shows the platform is actively developed. Success: a customer finds what is new in the latest release in seconds and can read any older release comfortably.

## Positioning

The official, first-party record of the platform's changes, written in Bosnian for the region's businesses. It sits alongside the main site (pitaj.io), the dashboard (app.pitaj.io) and the docs (docs.pitaj.io), and links to them.

## Operating Context

- One MDX file per release with frontmatter `title`, `description`, `versionNumber` (e.g. `v0.11-beta`), `date`; body is an H2 title, an intro sentence, then sections introduced by a `SectionHeader` component (icon + title) followed by bullet lists with bold lead-ins.
- Available section icons: ecommerce, mobile, globe, palette, bot, crawler, wordpress, chat, sync, omnichannel, cdn, docs, infra, tickets, star, brain, building, widget, code, analytics.
- Releases are numbered `v0.N-beta`; currently v0.5 to v0.11, newest first. The list will keep growing, so the structure must scale to many releases.
- Pages: an index that renders every release in a feed with a version navigation, and one page per release (`/releases/<slug>`).

## Capabilities and Constraints

- Language: Bosnian only (confirmed), `lang="bs"`. Keep diacritics correct.
- Stack: Astro + Sass (confirmed). Lucide icons via `@lucide/astro`.
- Existing release content (texts and section icons) is factual copy and is not rewritten by a visual redesign.
- The site carries a privacy notice that release notes contain no customer, company, client or visitor data. It was not marked binding in this round; it stays unless the user removes it, and its placement and form may change.
- Must work with a growing list of releases and with long MDX bodies.

## Brand Commitments

Same brand as pitaj.io and the dashboard: recognisably the same product (logo, tone, palette family), adapted for reading long release notes (confirmed). Existing assets: `public/logo.svg`, `public/favicon.svg`.

## Evidence on Hand

Seven real releases (v0.5-beta to v0.11-beta) in `src/content/releases/`. No screenshots, customer quotes or metrics are available; do not invent them.

## Product Principles

1. Newest first, scannable in seconds: a reader sees what changed before reading how.
2. Every release reads the same way, so comparing and skipping between releases is effortless.
3. Plain, honest release language: say what changed and what it means for the customer; no hype.
4. Recognisably Pitaj.io, but built for reading, not selling.

## Accessibility & Inclusion

No product-specific standard was established. Baseline: readable contrast in light and dark, keyboard navigation, skip link (exists), responsive down to phone width.
