# RABA Field Lab — Publication Style Guide

**Status:** operational presentation guide / public-surface consistency rule / non-canonical

## Purpose

This file preserves the presentation style for RABA Field Lab public research pages so future entries remain visually and structurally consistent.

It governs presentation only. It does not change research status, RABA architecture, publication authority, canon, validation, adoption, endorsement, compliance, certification, or Human Owner authority.

## Design direction

Use the **Editorial Research Notebook** style.

The site should feel like a calm, serious research notebook rather than a corporate landing page, startup product site, academic PDF, or technology showcase.

Priorities:

1. readability;
2. visible research progression;
3. restrained originality;
4. low maintenance;
5. continuity across pages;
6. clear epistemic and governance status.

## Visual language

Use:

- warm paper-like background rather than pure white;
- dark charcoal text rather than harsh black;
- serif body typography for long-form reading;
- clean sans-serif headings;
- restrained blue-grey accent;
- generous vertical spacing;
- a moderately wide but still controlled reading column;
- thin section dividers;
- calm highlighted blocks for research questions;
- compact code-style labels for research states and course states;
- a faint, reusable **Soft Research Signals in the Margins** motif on sufficiently wide desktop screens.

The margin motif should suggest process, transitions, automation, evidence flow, or decision paths through soft nodes, rounded traces, light arcs, and quiet guide-lines. It is decorative context only and must never carry evidence, status, or meaning that is absent from the text.

Avoid:

- sharp angular or spike-like background motifs;
- dense diagonal crossings;
- bright technology/cyber aesthetics;
- excessive colour;
- decorative gradients as a dominant visual effect;
- animation unless separately approved;
- heavy card layouts;
- marketing-style hero sections;
- visual effects that compete with the research content;
- dense background imagery behind the reading column;
- external font dependencies unless separately justified and approved.

## Header and title discipline

Keep the page entry visually simple.

For ordinary Pages content:

- show one site identity in the header;
- show one primary reading title in the page content;
- suppress theme-generated duplicate navigation/title output when it merely repeats the same page name;
- do not create multiple visible copies of `RABA Field Lab` at the top of the same page.

## Current implementation source

The active visual implementation is:

`docs/assets/main.scss`

Future public pages should inherit this stylesheet rather than reproduce local styling page by page.

Do not create page-specific CSS unless a real presentation need cannot be met by the shared stylesheet.

## Writing and page rhythm

Public research pages should use short, readable blocks.

Prefer:

- one idea per paragraph;
- short paragraphs;
- meaningful section headings;
- one strong research question at a time;
- visible distinction between evidence, interpretation, failed hypothesis, surviving question, and current course;
- blockquotes for central research questions or decision tensions;
- inline code formatting for controlled states such as `CONTINUE / REUSE`, `REUSE / STOP`, `NO MATERIAL RESIDUAL FOUND`, or equivalent research-state labels.

Do not turn pages into long unbroken academic prose.

## Research-story structure

When appropriate, reader-facing investigations should follow this progression:

`Question → Challenge → Existing approaches → What failed → What survived → Current result → Next test`

A negative or null result is a valid public research result.

Do not manufacture novelty or a RABA-specific mechanism when existing approaches are sufficient.

## Status discipline

Reader-friendly presentation must never strengthen the evidence.

Always distinguish, where relevant:

- documented evidence;
- interpretation;
- working hypothesis;
- publicly unresolved question;
- negative/null result;
- research course state;
- non-canonical status.

Publication on GitHub Pages does not imply canon, validation, adoption, endorsement, partnership, compliance, certification, commercial readiness, or architectural approval.

## Human Owner authority

AI may assist with research, comparison, evidence mapping, structuring, drafting, language, editing, and presentation.

Final decisions about public content, research direction, status promotion, architecture, canonicalization, and substantive public positioning remain with the Human Owner.

## Continuity rule for future Pages work

Before creating or materially restyling a new RABA Field Lab public page:

1. read this file;
2. reuse the shared stylesheet in `docs/assets/main.scss`;
3. preserve the Editorial Research Notebook design language;
4. preserve the Soft Research Signals in the Margins motif unless it interferes with readability or the Human Owner approves a change;
5. avoid adding a competing visual system;
6. keep changes minimal and reusable;
7. if a proposed page requires a different visual language, STOP and request Human Owner approval before introducing it.

## Change rule

This style guide may evolve, but not silently.

Material changes to the shared visual language should be treated as a bounded public-surface change and require Human Owner approval.
