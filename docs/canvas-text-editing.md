# Canvas Text Editing

The canvas editor should let creators edit the words and typography on screen directly, without opening a separate design tool or touching layout structure.

## User Goal

A creator should be able to select a lower-third, title card, caption block, or overlay label on the canvas, change its text and look, and see the result against a real episode moment while the layout and presets stay intact.

## Editable Text Objects

Text editing should apply to the podcast objects creators already recognize:

- lower-thirds with speaker name and handle
- title moments and title cards
- chapter and segment labels
- caption styling for the active caption track
- sponsor and disclosure labels
- custom overlay text the creator adds

Editing one object should never silently restyle the others. Changing a single guest lower-third should not rewrite every speaker's name treatment unless the creator chooses to apply it across the layout.

## Text And Typography Controls

Offer creator-facing type choices, not a full font engineering panel:

- edit the text content inline on the canvas
- pick from brand-kit fonts before arbitrary system fonts
- set size, weight, and emphasis
- choose color from the show brand kit with readable contrast
- set alignment and casing
- apply simple emphasis like highlight, underline, or accent color

Controls should describe outcomes in creator language and warn when a choice hurts readability rather than blocking it.

## Context Awareness

Text edits should stay connected to episode context so they survive reuse:

- lower-thirds keep inheriting names and handles from social context unless manually overridden
- title moments can pull from episode metadata and segment structure
- caption style changes preview against real spoken lines, not placeholder text
- a manual text override is remembered for that object but does not break automatic fill for the rest

Placement, layering, and safe-area fit stay owned by canvas layer controls and safe areas; this workflow owns the words and their type treatment.

## Reuse Requirements

Before saving text choices into a show template, confirm what should adapt next episode:

- which text is fixed wording and which is filled from context
- font, color, and emphasis that belong to the show identity
- caption style that should carry across episodes
- title and lower-third treatment that future guests should inherit

## Maintainer Acceptance Notes

Accept work that makes on-canvas text and typography feel direct, readable, brand-aware, and reusable across episodes. Close work that turns the canvas into a generic typesetting tool, detaches lower-thirds and titles from speaker and episode context, overrides automatic name and metadata fill by default, or duplicates layout positioning and safe-area checks that already have their own specs.
