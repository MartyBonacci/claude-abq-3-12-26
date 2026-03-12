# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Reveal.js slide presentation for the Claude Code ABQ meetup (March 12, 2026). The talk is titled "The Most Valuable Developer on Your Team — Building AI Workflows That Scale" by Marty Bonacci.

The presentation uses a "nailing boards together" analogy to teach AI prompt engineering concepts — progressing from vague instructions (bad results) to CLAUDE.md/skills/hooks (perfect results).

## Key Files

- `index.html` — The entire presentation (single-file reveal.js app, loaded from CDN)
- `FINAL-COMPLETE-SPEC.md` — Complete slide-by-slide spec with speaker notes, design system, and pacing guide. This is the source of truth for all content.
- `images/` — Presentation images (board nailing sequence photos, screenshots)
- `references/` — Supporting handout materials (extensibility-stack.md, example-claude-md.md, getting-started.md, resources.md)

## Development

No build step. Open `index.html` directly in a browser or use any local server:

```bash
npx serve .
# or
python3 -m http.server
```

Press `S` in the browser to open reveal.js speaker notes view.

## Architecture Notes

- **Single HTML file** — all slides, CSS, and configuration live in `index.html`
- **Reveal.js from CDN** — no node_modules or local dependencies
- **QR codes** — generated programmatically (JS library or embedded SVG)
- **Image references** — actual filenames in `images/` differ slightly from spec (e.g., `sandwhiching` not `sandwiching`, `beatiful` not `beautiful`). Always check actual filenames with glob before referencing.

## Design System

- Dark backgrounds throughout: primary `#1a1a2e`, cards `#16213e`
- Text: white `#ffffff` headings, light gray `#c0c0c0` body
- Accents: teal `#028090` (highlights/new lines), coral `#F96167` (emphasis)
- Headings: monospace. Body: system sans-serif.
- Prompt slides use a card/box with monospace text; NEW lines highlighted in teal

## Slide Structure

~54 slides total. The core "boards sequence" (B-0 through B-31) follows a strict pattern:
1. **PROMPT slide** — setup line + instruction card (dark bg)
2. **IMAGE slide** — full-bleed photo, no text (`data-background-image`)

Callback slides B-19, B-21, B-23 must have visually identical prompt cards (the joke is repetition).

## Image Filename Mapping

The spec references idealized filenames. Actual files have typos/variations. Key mappings:
- Spec: `two-pieces-of-wood-sandwiching-a-nail.png` → Actual: `two-pieces-of-wood-sandwhiching-a-nail.png`
- Spec: `this-joint-looks-beautiful-even-though-there-are-no-nails.png` → Actual: `this-joint-looks-beatiful-even-though-there-are-no-nails.png`
- Spec: `nailed-into-wood-sideways-but-the-wood-is-butted-end-to-end_png.png` → Actual: `nailed-into-wood-sideways-but-the-wood-is-butted-end-to-end.png`
- Spec: `nailed-into-the-stacked-wood-with_nails-sideways.png` → Actual: `nailed-into-the-stacked-wood-with nails-sideways.png` (space, not underscore)
- Screenshots (`images/screenshots/`) are placeholders — Marty provides these
