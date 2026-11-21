---
name: Mert Lafcı
description: An engineer's computation pad. Three shipped apps as filled-in sheets on green-tinted grid paper.
colors:
  pad-paper: "#e8efe0"
  mount-card: "#f7faf3"
  grid-line: "rgba(47, 104, 72, 0.09)"
  grid-line-major: "rgba(47, 104, 72, 0.17)"
  graphite-ink: "#17202b"
  graphite-soft: "#3b4855"
  rule-soft: "rgba(23, 32, 43, 0.2)"
  red-pencil: "#b52d17"
  on-ink: "#f1f5ec"
  board-paper: "#0f1813"
  board-mount: "#18231c"
  board-grid-line: "rgba(150, 214, 172, 0.06)"
  board-grid-line-major: "rgba(150, 214, 172, 0.12)"
  chalk-ink: "#e3ebe1"
  chalk-soft: "#a7b6aa"
  chalk-rule: "#cfdccf"
  chalk-rule-soft: "rgba(207, 220, 207, 0.2)"
  red-pencil-night: "#ff8466"
typography:
  display:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2.9rem, 13.5vw, 10rem)"
    fontWeight: 850
    lineHeight: 0.92
    letterSpacing: "-0.035em"
    fontVariation: "'wdth' 125"
  headline:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2.1rem, 6vw, 3.6rem)"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "-0.03em"
    fontVariation: "'wdth' 112"
  title:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(1.5rem, 3.6vw, 2.25rem)"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "-0.025em"
    fontVariation: "'wdth' 108"
  body:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.6
    fontVariation: "'wdth' 100"
  lead:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(1.08rem, 2.2vw, 1.22rem)"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "0.82rem"
    fontWeight: 650
    letterSpacing: "0.07em"
    fontFeature: "'tnum' 1"
    fontVariation: "'wdth' 75"
  button:
    fontFamily: "Archivo, Helvetica Neue, Arial, sans-serif"
    fontSize: "0.95rem"
    fontWeight: 700
    fontVariation: "'wdth' 90"
rounded:
  hairline: "2px"
  device: "14px"
spacing:
  grid: "24px"
  grid-major: "120px"
  cell-x: "1rem"
  gap-sm: "0.75rem"
  gap-md: "1.5rem"
  gap-lg: "2.5rem"
  section: "clamp(3rem, 8vw, 6rem)"
components:
  button-primary:
    backgroundColor: "{colors.graphite-ink}"
    textColor: "{colors.on-ink}"
    typography: "{typography.button}"
    rounded: "{rounded.hairline}"
    padding: "0 1.2rem"
    height: "3rem"
  button-primary-hover:
    backgroundColor: "transparent"
    textColor: "{colors.graphite-ink}"
  button-line:
    backgroundColor: "{colors.pad-paper}"
    textColor: "{colors.graphite-ink}"
    typography: "{typography.button}"
    rounded: "{rounded.hairline}"
    padding: "0 1.2rem"
    height: "3rem"
  button-line-hover:
    backgroundColor: "{colors.graphite-ink}"
    textColor: "{colors.on-ink}"
  link-cell:
    backgroundColor: "{colors.pad-paper}"
    textColor: "{colors.graphite-ink}"
    rounded: "{rounded.hairline}"
    padding: "0 1rem"
    height: "2.9rem"
  link-cell-hover:
    backgroundColor: "{colors.graphite-ink}"
    textColor: "{colors.on-ink}"
  title-block-cell:
    backgroundColor: "{colors.pad-paper}"
    textColor: "{colors.graphite-soft}"
    typography: "{typography.label}"
    padding: "0 1rem"
    height: "3rem"
  sheet-cell:
    backgroundColor: "{colors.pad-paper}"
    textColor: "{colors.graphite-ink}"
    typography: "{typography.label}"
    padding: "0.6rem 0.85rem"
  sheet-cell-status:
    textColor: "{colors.red-pencil}"
---

# Design System: Mert Lafcı

## Overview

**Creative North Star: "The Computation Pad"**

The page is an engineer's pad of green-tinted grid paper. Each shipped app is a filled-in sheet: a ruled title block of cells across the top, a plain-language description, a verified claim ticked in red pencil, and screenshots clipped on as numbered figures. Chrome is drawn with rules, not boxes of colour; the paper, its grid and graphite ink do nearly all the work, so the products carry the page.

Dark mode is the same pad laid on a green-black drafting board: chalk ink, a grid that glows faintly, and luminance doing the job colour does in light mode. One red-pencil colour exists in each theme and is held for state: what is verified, what is active, what has focus. Motion is a pencil, not a slide: strokes draw themselves once when they enter view and then stay.

Type is a single variable family, Archivo, used across its width axis. Expanded heavy cuts set names at architectural scale; condensed caps fill the ruled cells; the normal width carries reading text.

**Key Characteristics:**
- Pale green grid paper (24px cells, every fifth line stronger) as the page itself, not a texture on a card.
- Ruled title blocks: hairline cells in condensed caps, identical across every sheet header and the top bar.
- One red pencil per theme, reserved for verification, active state, focus and selection.
- Archivo across its width axis: 125% for the name, ~108-112% for headings, 75-80% for cell labels, 100% for reading.
- Near-square corners (2px); screenshots mounted on lighter card stock with one soft ambient shadow.
- Strokes (check marks, the process line) draw once on entry; nothing slides or bounces.

## Colors

Graphite on green-tinted pad paper, one red pencil; at night, chalk on a green-black board.

### Primary
- **Red Pencil** (`red-pencil`, light; `red-pencil-night`, dark): the only hue that is not paper or ink. Drawn check marks beside each verified claim, the status cell of every sheet header, the active language switch, the underline under the current nav cell, the focus outline and text selection. Contrast on paper is 5.3:1 (light) and 7.5:1 (dark).

### Neutral
- **Pad Paper** (`pad-paper`): the page background and the fill of every ruled container (title block, sheet head, sheet index, contact field), so ruled containers read as drawn on the paper rather than laid on top of it.
- **Mount Card** (`mount-card`): the lighter stock screenshots are clipped onto, and thumbnail backgrounds in the sheet index.
- **Graph Grid** (`grid-line`, `grid-line-major`): the 24px minor and 120px major grid lines; the minor grid colour doubles as the hover wash on nav cells and index rows.
- **Graphite Ink** (`graphite-ink`): body text, headings, heavy 2px rules, primary button fill, the hover fill of line buttons and link cells.
- **Soft Graphite** (`graphite-soft`): secondary text (vision paragraph, section leads, idle nav cells, figure captions, footer, stack cells) and the dotted main line of the process diagram.
- **Hairline Rule** (`rule-soft`): 1px dividers between cells and rows.
- **On Ink** (`on-ink`): text on graphite fills and on red selection.
- **Drafting Board** (`board-paper`, `board-mount`, `board-grid-line*`, `chalk-ink`, `chalk-soft`, `chalk-rule`, `chalk-rule-soft`): the dark-theme counterparts, mapped role for role onto the same custom properties.

### Named Rules
**The One Red Pencil Rule.** Red marks state and verification only: a checked claim, a status cell, the active choice, focus, selection. It never decorates a heading, a background or an icon that is not a mark.

**The Luminance Is State Rule.** In dark mode, emphasis comes from brightness (chalk ink against soft chalk, brighter red pencil), not from new hues or glows.

## Typography

**Display Font:** Archivo variable (self-hosted woff2, latin and latin-ext, weight 100-900, width 62-125%, SIL OFL), with Helvetica Neue and Arial as fallbacks.
**Body Font:** the same Archivo at normal width.
**Label Font:** the same Archivo, condensed.

**Character:** One family stretched to every job. The width axis carries the hierarchy as much as size does: wide and heavy reads as a stamped name, narrow caps read as a printed form.

### Hierarchy
- **Display** (850, 125% width, clamp 2.9-10rem, line-height 0.92): the owner's name in the first viewport only.
- **Headline** (800, 112% width, clamp 2.1-3.6rem, line-height 1): section titles, sitting on a 2px rule.
- **Title** (800, 108% width, clamp 1.5-2.25rem, line-height 1.1): app names in sheet heads; process step titles use the same voice at 105% width and clamp 1.3-1.6rem; the contact email field uses it at 105% width, clamp 1.3-2.75rem.
- **Body** (400, 1.0625rem, line-height 1.6): descriptions, max 38rem; process steps max 30rem.
- **Lead** (400, clamp 1.08-1.22rem, line-height 1.6, soft graphite): the vision paragraph and section leads, max 34-38rem.
- **Label** (600-700, 75-80% width, 0.75-0.86rem, letter-spacing 0.06-0.08em, uppercase, tabular numerals): title-block cells, nav cells, sheet-head cells, figure captions, index "Fig." lines, footer. The role line under the name is the same voice at clamp 1.05-1.3rem.
- **Wordmark** (800, 118% width, 1rem, uppercase): the top-left cell only.

### Named Rules
**The Width Axis Rule.** Hierarchy is set with font-stretch as well as size: names expand, cells condense, reading stays at 100%. Never introduce a second family to get contrast.

**The No Handwriting Rule.** Red-pencil marks are drawn SVG strokes with round caps; a handwriting or script font never stands in for them.

## Layout

A single centred column, `min(100% - 2rem, 72rem)` wide, laid on a full-bleed grid background (24px minor, 120px major, anchored at the page origin). The top bar is a sticky title block: a row of ruled cells (wordmark, three nav cells, EN/TR, theme) with a 2px bottom rule; under 700px the nav cells drop to a second full-width row of equal cells.

The opening sheet puts the name across the full width, then splits (from 960px) into the role, vision and actions on the left and a 21rem sheet index of three figure thumbnails on the right; below 960px the index follows the text. Sections open with `clamp(3rem, 8vw, 6rem)` top padding and a head that pairs the headline with a right-aligned lead (from 860px) over a 2px rule.

Projects: the lead sheet spans the width with description and figures side by side (from 860px); the two secondary sheets sit in two columns from 1000px, with figures stacked above their text. Paired phone figures offset the second by 3rem. The process section runs as a vertical line with a branch out and merge back on phones, and as three columns under a horizontal branch-and-merge drawing from 860px. Spacing steps observed: 0.75rem, 1rem, 1.5rem, 2rem, 2.5rem, 3rem.

## Elevation & Depth

Flat and ruled. Depth comes from rule weight (2px for structure, 1px soft hairlines for subdivisions) and from the one lighter stock, the mount card. A single soft ambient shadow exists, and only under mounted screenshots, the way a clipped photo sits on paper.

### Shadow Vocabulary
- **Clipped Figure** (`box-shadow: 0 14px 30px -12px rgba(23, 32, 43, 0.28), 0 2px 6px rgba(23, 32, 43, 0.08)`; dark: `0 16px 34px -12px rgba(0, 0, 0, 0.6), 0 2px 6px rgba(0, 0, 0, 0.3)`): screenshot mounts only.

### Named Rules
**The Drawn Not Stacked Rule.** Containers are outlined with rules on the paper colour; they never float. A shadow belongs to a clipped-on figure and nothing else.

## Shapes

Near-square everywhere: 2px corners on buttons and link cells, square ruled containers, square thumbnails. The only rounding is borrowed from the objects themselves: 14px on phone screenshots (device corners) and round process nodes (hollow, the merge node filled with ink). Strokes use round caps and joins so marks read as pencil.

## Components

### Buttons
Solid, square, ruled; they invert rather than glow.
- **Shape:** 2px corners, 2px graphite border, 3rem tall, 1.2rem side padding, 1rem icon with 0.6rem gap.
- **Primary:** graphite fill, on-ink text. Hover empties to transparent with graphite text.
- **Line:** paper fill, graphite text. Hover fills with graphite and on-ink text.
- **Focus:** 2px red-pencil outline, 3px offset (global).

### Link Cells
Project outbound links (store, repository, download): 1px graphite border, 2px corners, 2.9rem tall, paper fill; hover inverts to graphite. They wrap as a row with 0.6rem gaps.

### Title Block (navigation)
- **Style:** sticky, paper fill, 2px bottom rule, 3rem cells divided by soft hairlines.
- **Cells:** condensed uppercase labels in soft graphite; hover lifts to graphite on a grid-colour wash; the current section gets graphite text and a 3px inset red-pencil underline.
- **Language switch:** EN/TR in condensed caps; the active language is red pencil with a 2px underline.
- **Theme switch:** a drawn sun/moon icon cell; hidden without JavaScript so the page follows the system setting.
- **Mobile:** nav cells become an equal-width second row, 2.75rem tall.

### Sheet Head (signature)
The ruled title block on every project sheet: a 1px graphite frame holding a full-width app-name cell, then condensed caps cells for platform, status (red pencil) and stack (soft graphite), and on the lead sheet a full-width meta cell in sentence case. Every sheet uses the same cells in the same order.

### Verified Claim
A drawn red-pencil check (1.6rem, stroke 2.6, round caps) beside a semibold claim sentence, in a 1.6rem/1fr grid. One per sheet.

### Figure Mount
Screenshot on mount-card stock, 0.5rem padding, soft hairline border, clipped-figure shadow; caption below in label voice ("Fig. 1.1").

### Sheet Index
A 2px-ruled list of three rows: a 4.5rem by 3.5rem thumbnail, a "Fig. n" label line with the platform, and the app name; hover washes the row with grid colour and underlines the name.

### Contact Field
The email as a filled form field: 2px-ruled box, the address in the title voice at up to 2.75rem with an arrow; hover inverts to graphite and nudges the arrow up and right. Social links split the row beneath into equal ruled cells that invert on hover.

### Pencil Strokes (motion)
Check marks and the process line draw once via stroke-dashoffset when they enter view (1.4s, `cubic-bezier(0.16, 1, 0.3, 1)`; checks 0.7s after a 0.25s delay). The dotted main process line never animates. Under reduced motion, strokes are shown drawn and transitions are effectively instant.

## Do's and Don'ts

### Do:
- **Do** draw every container as a rule on the paper colour: 2px graphite for structure, 1px soft hairline for subdivisions.
- **Do** reuse the sheet-head cells (name, platform, status, stack) in the same order for any new project sheet.
- **Do** set cell and caption labels in Archivo at 75-80% width, uppercase, letter-spacing 0.06-0.08em.
- **Do** number figures "Fig. n.m" by sheet and keep captions in the label voice.
- **Do** keep red pencil to verification, status, the active choice, focus and selection; check text contrast against both paper colours.
- **Do** let new marks (ticks, connectors) be SVG strokes with round caps that draw once on entry and respect reduced motion.
- **Do** keep both themes mapped through the same custom properties so every component inherits the swap.

### Don't:
- **Don't** add a second accent hue or tint backgrounds with red.
- **Don't** use a handwriting or script font for pencil marks.
- **Don't** round containers beyond 2px or give ruled containers a drop shadow; the shadow belongs to mounted figures only.
- **Don't** add a second type family; get contrast from Archivo's width and weight.
- **Don't** introduce slide-in, fade-up or bouncing entrances; the only entry motion is a stroke drawing itself.
- **Don't** replace the grid paper with a flat background or a gradient, or add neon glows in dark mode.
