---
version: 1
slug: "src-pages-index-astro"
primary_target: "src/pages/index.astro"
related_targets: ["src/pages/releases/[slug].astro"]
---

# Changelog surface (index and release pages)

## Scope
Read mode. Index feed of all releases plus one page per release. Reader: a customer running agents on Pitaj.io who wants to see what is new in seconds. Must not feel like marketing; must stay recognisably Pitaj.io; scanning must not get slower than today.

## Direction contract

THESIS: Every release is one issue of a programme guide: a strict 12-column grid where the release number is the page's anchor and sections are rows with a pictogram, not cards. Refuses the SaaS changelog default (rounded cards, pills, hero with a "latest" tile).

OWN-WORLD: Sarajevo '84 programme guide meets Pitaj.io. Neutral paper, near-black ink (the logo's #0b0b0f), Pitaj blue as the single programme colour, a signal green for reliability. One sans family (Archivo, width axis for narrow labels), tabular numerals, 3px ink rules and hairlines. Square and circle pictogram tiles drawn from Lucide. No shadows, no gradients, no rounded cards.

STORY: The reader sees the newest release number and title first, finds the section they care about by pictogram and heading, and reads short rows. Older releases are reachable from a rail that lists number and date.

FIRST VIEWPORT: Masthead with logo and links over a 3px ink rule. Left rail (cols 1-3): "Program izdanja" list, version and date, newest marked. Main (cols 4-12): page title and one-line description, privacy note as small running text, then the newest issue: huge sticky release number in blue at left, title, lead sentence, then section rows (pictogram tile, heading, bullet list).

FORM: Programme guide, assigned by the roll (candidate 7), seed:f78a9aeec70b22b7. Signature move: the sticky release numeral, held while its issue scrolls. Raises: state is carried by tile shape and text, not hue alone (from cutting-bench); tabular numerals for dates and counts (from ikeda-datamatics).

FINISH: unreviewed and undocumented is unfinished; this build ends with the finish review, the verdict, DESIGN.md, and every shipping raster carrying its provenance
