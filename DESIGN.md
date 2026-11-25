---
name: Gabriel Belcastro portfolio
description: Airport wayfinding for a recruiter. Black signs in signal yellow point to the voice work, the systems and the contact.
colors:
  concourse-grey: "#E4E6E3"
  concourse-grey-deep: "#D7DAD6"
  ticket-paper: "#F4F5F3"
  sign-black: "#111214"
  sign-black-raised: "#1D1F23"
  sign-seam: "#33363C"
  signal-yellow: "#FFC629"
  signal-yellow-lit: "#FFD55C"
  body-graphite: "#2A2D31"
  caption-slate: "#565B62"
  rule-grey: "#AEB2AD"
  on-sign: "#ECEDEE"
  on-sign-muted: "#A9AEB5"
  wave-idle: "#6E737B"
typography:
  display:
    fontFamily: "Barlow Condensed, Arial Narrow, sans-serif"
    fontSize: "clamp(42px, 6.2vw, 88px)"
    fontWeight: 800
    lineHeight: 0.95
  headline:
    fontFamily: "Barlow Condensed, Arial Narrow, sans-serif"
    fontSize: "clamp(38px, 5vw, 64px)"
    fontWeight: 800
    lineHeight: 1
  title:
    fontFamily: "Barlow Condensed, Arial Narrow, sans-serif"
    fontSize: "clamp(28px, 2.8vw, 36px)"
    fontWeight: 800
    lineHeight: 1
  body:
    fontFamily: "Barlow, Segoe UI, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "Barlow Condensed, Arial Narrow, sans-serif"
    fontSize: "16px"
    fontWeight: 700
    letterSpacing: "0.05em"
rounded:
  control: "3px"
  panel: "6px"
spacing:
  gutter: "32px"
  gutter-phone: "16px"
  section: "112px"
  section-phone: "80px"
components:
  button-sign:
    backgroundColor: "{colors.signal-yellow}"
    textColor: "{colors.sign-black}"
    typography: "{typography.label}"
    rounded: "{rounded.control}"
    padding: "9px 16px"
  button-sign-hover:
    backgroundColor: "{colors.signal-yellow-lit}"
  button-line:
    textColor: "{colors.sign-black}"
    rounded: "{rounded.control}"
    padding: "8px 15px"
  button-line-hover:
    backgroundColor: "{colors.sign-black}"
    textColor: "{colors.signal-yellow}"
  call-sign:
    backgroundColor: "{colors.sign-black}"
    textColor: "{colors.on-sign}"
    rounded: "{rounded.panel}"
    padding: "32px 36px"
  tag-measured:
    backgroundColor: "{colors.signal-yellow}"
    textColor: "{colors.sign-black}"
    rounded: "{rounded.control}"
---

# Design System: Gabriel Belcastro portfolio

## Overview

The page is airport wayfinding for one visitor: a recruiter who must find the voice work, the systems and the contact in seconds. Black sign panels set in signal yellow do the directing; everything else sits on a pale concourse grey, flat, ruled and quiet. The world comes from Gabriel's own ground (airline operations and the calls made to them), one step removed from the obvious airline artifacts. Anti-references: the cream editorial page with a terracotta accent this replaced, and the dark developer portfolio with a split hero over equal cards.

## Colors

Committed strategy: signal yellow on sign black carries every sign (the band, the call sign, the contact close, the pictogram tiles); the concourse grey is the ground.

### Primary
- **Signal Yellow** (#FFC629): the color of direction. Primary actions, the played part of the waveform, the "measured on real calls" tag, pictograms on black, the whole contact close. Never body text on grey.

### Neutral
- **Sign Black** (#111214): sign panels, the top band, headings, the route line, ink.
- **Concourse Grey** (#E4E6E3): page ground. **Concourse Grey Deep** (#D7DAD6): row hover, the agent's lines in the transcript.
- **Ticket Paper** (#F4F5F3): tables and the transcript box, the only "lifted" surfaces on the ground.
- **Body Graphite** (#2A2D31): running text. **Caption Slate** (#565B62): captions and secondary lines (5.4:1 on the ground, 4.9:1 on a hovered row).
- **Rule Grey** (#AEB2AD): hairline rules between directory rows and tag borders.
- **On Sign** (#ECEDEE) and **On Sign Muted** (#A9AEB5): text on black panels.

### Named Rules
**The One Signal Rule.** Yellow means "go here" or "proven". It is never decoration and never a second accent's partner. In the content area play is the only yellow action; e-mail is yellow only in the band and the contact close.

## Typography

**Display font:** Barlow Condensed (fallback Arial Narrow)
**Body font:** Barlow (fallback Segoe UI)

One family in two widths, after highway and airport sign lettering. Condensed carries every sign, heading, label and button; the regular width carries reading.

### Hierarchy
- **Display** (800, clamp(42px, 6.2vw, 88px), 0.95): the one hero line.
- **Headline** (800, clamp(38px, 5vw, 64px), 1): section signs, always beside a pictogram tile.
- **Title** (700–800, 26–36px, 1–1.08): directory entries, route stops, the call title.
- **Body** (400, 17px / 16px on phones, 1.55): prose, held to about 62–66ch.
- **Label** (600–700, 16–19px, 0.05em, uppercase): status lines under titles and the tags. Never above a heading.

### Named Rules
**The No Kicker Rule.** No label sits above a heading; status and kind lines go under the title.

## Layout

Single column at 1200px max with a 32px gutter (16px on phones). Sections open 112px apart (80px on phones). The voice section splits 7:5 (route left, evidence right); directory rows run thumbnail 300px, text, action. Everything collapses to one column under 860–960px; nothing scrolls sideways at 390px.

## Elevation & Depth

Flat by default. Depth is tonal: black signs on grey, paper tables with a 2px ink border. The only shadow is under the hero call sign (`0 24px 48px -24px rgba(17,18,20,.55)`), to lift the demonstration off the ground.

## Shapes

Small, sign-like corners: 3px on controls and tags, 4–6px on panels and frames. Circles only for the play button and the numbered route stops. Rules do the grouping: 4px ink under group heads, 1px rule grey between rows.

## Components

### Buttons
- **Shape:** 3px corners.
- **Sign (primary):** signal yellow, sign black text, condensed 700, 9px 16px; hover lifts to #FFD55C.
- **Line (secondary):** 2px ink border on the ground; hover fills black with yellow text.
- **Dark (on yellow):** black with yellow text, used in the contact close.

### Navigation
The top band is the overhead sign: name with a yellow GB tile, directional links separated by seams with down arrows, the language switch, and a yellow e-mail sign (mailto). Active section turns yellow. Under 1000px the links fold away; under 640px a yellow mail tile stays beside the menu button, which opens a black panel.

### Call sign (signature component)
A full-width black sign: phone pictogram tile, the call title, a kind line, then the player. The waveform is the real call's loudness in 96 bars (48 on phones); unplayed bars are #6E737B (3.5:1 on the player), played bars turn yellow, the bars rise once on first view, and click, drag or arrow keys seek. The legend names the two voices in text only, because the bars show progress, not speaker. The measured-versus-simulated note sits beside it, inside the first viewport on desktop. On phones the call sign moves directly under the headline.

### Directory rows
Projects are rows, not cards: thumbnail, title, status line, text, and an action with an arrow (diagonal for external links). Hover tints the row and outlines the thumbnail.

### Route
The voice steps are a route: a 4px ink line through numbered black stops; the number is the real order of a call.

## Do's and Don'ts

- Do keep every arrow and pictogram as authored SVG at one stroke; don't use Unicode arrows or emoji.
- Do label proof honestly: yellow tag for measured on real calls, outline tag for simulated.
- Don't add cards, pills, tag clouds, glass, gradients, kickers or monospace costume. Lists of tools run as one line with slash separators.
- Don't put yellow text on the grey ground.
- Don't add a second accent color.

## Assets

Screenshots in `screenshots/` are captures of the real products (sample or empty data); `milesterminal-*.jpg` were taken from the project's own code with no data. `og.jpg` is rendered from HTML in this system. `audio/clara-ligacao-de-teste.mp3` is the public test call from domuspi.com.br.
