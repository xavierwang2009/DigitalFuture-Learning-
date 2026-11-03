---
name: Building Your First Website
description: A Periodic Table of the Web. Each lesson adds element tiles, and the student's own table fills in as they learn.
colors:
  ground: "#f3f5fb"
  rail: "#e7ebf8"
  surface: "#ffffff"
  surface-2: "#f6f8fd"
  sunk: "#eceff8"
  ink: "#0f1838"
  ink-2: "#4a5675"
  line: "#d6dceb"
  line-2: "#b3bcd4"
  html: "#2546e8"
  on-html: "#ffffff"
  html-soft: "#e3e8fe"
  css: "#c2186e"
  on-css: "#ffffff"
  css-soft: "#fbe3ef"
  plan: "#ffc52e"
  on-plan: "#0f1838"
  plan-soft: "#fff3d1"
  plan-ink: "#8a6200"
  ok: "#0e7c55"
  on-ok: "#ffffff"
  ok-soft: "#e1f3ea"
  warn: "#8a5300"
  warn-soft: "#fff1d6"
  code-bg: "#0f1838"
  code-ink: "#e3e8f8"
  code-select: "#3550d6"
  focus: "#2546e8"
typography:
  display:
    fontFamily: "Archivo, system-ui, -apple-system, Segoe UI, Roboto, sans-serif"
    fontSize: "clamp(27px, 2.4vw, 35px)"
    fontWeight: 820
    lineHeight: 1.1
    letterSpacing: "-0.022em"
    fontVariation: "'wdth' 118"
  symbol:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "32px"
    fontWeight: 820
    lineHeight: 1
    letterSpacing: "-0.02em"
    fontVariation: "'wdth' 125"
  headline:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "clamp(21px, 1.8vw, 25px)"
    fontWeight: 760
    lineHeight: 1.15
    letterSpacing: "-0.015em"
    fontVariation: "'wdth' 112"
  title:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "15.5px"
    fontWeight: 760
    lineHeight: 1.55
    fontVariation: "'wdth' 110"
  intro:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "17.5px"
    fontWeight: 400
    lineHeight: 1.5
  body:
    fontFamily: "Archivo, system-ui, -apple-system, Segoe UI, Roboto, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.55
  control:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "14px"
    fontWeight: 560
    lineHeight: 1.2
  label:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "12.5px"
    fontWeight: 650
    lineHeight: 1.3
    fontFeature: "'tnum'"
  code:
    fontFamily: "JetBrains Mono, ui-monospace, SFMono-Regular, Consolas, monospace"
    fontSize: "13.5px"
    fontWeight: 400
    lineHeight: 1.7
  code-small:
    fontFamily: "JetBrains Mono, ui-monospace, SFMono-Regular, Consolas, monospace"
    fontSize: "11.5px"
    fontWeight: 650
    lineHeight: 1.25
rounded:
  tile-inner: "2px"
  tile-sm: "3px"
  tile: "4px"
  control-sm: "6px"
  control: "7px"
  well: "8px"
  track: "9px"
  card-sm: "10px"
  card: "12px"
  dialog: "14px"
  pill: "999px"
spacing:
  hair: "4px"
  xs: "6px"
  sm: "8px"
  md: "12px"
  lg: "16px"
  xl: "18px"
  2xl: "22px"
  3xl: "24px"
  4xl: "28px"
components:
  button:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    typography: "{typography.control}"
    rounded: "{rounded.control}"
    padding: "9px 14px"
    height: "42px"
  button-hover:
    backgroundColor: "{colors.surface-2}"
  button-primary:
    backgroundColor: "{colors.html}"
    textColor: "{colors.on-html}"
    rounded: "{rounded.control}"
    padding: "9px 14px"
    height: "42px"
  button-primary-hover:
    backgroundColor: "color-mix(in oklab, #2546e8, #0f1838 18%)"
  button-ink:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.surface}"
    rounded: "{rounded.control}"
    padding: "9px 14px"
    height: "42px"
  button-ink-done:
    backgroundColor: "{colors.ok-soft}"
    textColor: "{colors.ink}"
  tab-track:
    backgroundColor: "{colors.sunk}"
    rounded: "{rounded.track}"
    padding: "3px"
  tab:
    backgroundColor: "transparent"
    textColor: "{colors.ink-2}"
    rounded: "{rounded.control-sm}"
    padding: "6px 12px"
    height: "36px"
  tab-pressed:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
  input-text:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "10px 12px"
    height: "44px"
  element-tile:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.tile}"
    padding: "8px 9px 10px"
    height: "120px"
  element-tile-collected-html:
    backgroundColor: "{colors.html}"
    textColor: "{colors.on-html}"
  element-tile-collected-css:
    backgroundColor: "{colors.css}"
    textColor: "{colors.on-css}"
  element-tile-collected-plan:
    backgroundColor: "{colors.plan}"
    textColor: "{colors.on-plan}"
  table-tile:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink-2}"
    rounded: "{rounded.tile-sm}"
  lesson-link-current:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.well}"
    padding: "8px 10px 8px 8px"
    height: "44px"
  step-dot:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.tile-sm}"
    size: "26px"
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.card}"
    padding: "28px 28px 22px"
  code-editor:
    backgroundColor: "{colors.code-bg}"
    textColor: "{colors.code-ink}"
    typography: "{typography.code}"
    padding: "18px 20px"
  snippet:
    backgroundColor: "{colors.sunk}"
    textColor: "{colors.ink}"
    rounded: "{rounded.well}"
    padding: "14px 16px"
  dialog:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.dialog}"
    padding: "26px 30px 30px"
  jump-pill:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "7px 12px"
---

# Design System: Building Your First Website

## Overview

**Creative North Star: "The Periodic Table of the Web"**

HTML calls its parts elements, so the workshop is a classroom chart. Every lesson introduces a few elements and properties as square chart tiles, and the student's own table in the lesson rail fills in, column by column, as lessons are marked complete. The page is a well-lit chart poster crossed with a web reference: cool chart-white ground, ink-navy type, and colour that only appears when it has a job.

Colour belongs to element families. Cobalt means HTML structure, magenta means CSS style, signal yellow means planning and testing, and green means done. A family colour fills a tile when the student has collected it; before that the tile is an empty white slot with an ink border. The interface around the student's code stays quiet: white cards on a pale ground, thin cool-grey rules, soft one-step shadows. The code editor is the one dark surface in light mode, so the student's code reads as the most important thing on the page.

Dark mode is the same chart printed on deep ink-blue, not a hacker screen. Families keep their meaning and only brighten to stay legible. The user rejected "hacker-movie dark" (black screens, green matrix text, glowing neon), and the build honours that: no black, no glow, no green code text.

**Key Characteristics:**
- Square element tiles with a 1px ink border, atomic number top-left, a heavy expanded symbol, and a mono name below.
- Four family colours with fixed meanings (HTML, CSS, Plan & test, Done); everything else is ink, grey, and white.
- One expanded variable grotesk (Archivo) for everything readable, JetBrains Mono for code.
- Tiles fill from the bottom up, staggered, when a lesson is completed. This is the only showpiece motion.
- Light by default for classrooms and projectors; deep ink-blue when the device asks for dark.

## Colors

A cool, near-white chart with ink-navy text and four saturated family colours that each mean one thing.

### Primary
- **Electric Cobalt** (#2546e8; dark #7d95ff): the HTML family. Fills collected HTML tiles, the brand tile, the Run preview button, links, and the focus ring. Its soft tint (#e3e8fe; dark #22306b) marks pressed utility buttons and the current table column.

### Secondary
- **Style Magenta** (#c2186e; dark #ff6fb0): the CSS family. Fills collected CSS tiles and the Session 2 swatches. Soft tint #fbe3ef (dark #4a1f3d). Also used as the save-error dot.

### Tertiary
- **Signal Yellow** (#ffc52e; dark #ffd45a): the Plan & test family. Fills collected planning tiles, text selection, the editor caret, and the "preview is out of date" dot. Text on yellow is always ink (#0f1838). On white, yellow-family numbers and symbols use the darker Plan Ink (#8a6200) so they stay readable. Soft tint #fff3d1 (dark #3f3416).
- **Done Green** (#0e7c55; dark #3ccb92): completion only. Completed step numbers, check marks, the "saved" and "up to date" dots, correct quiz answers, and the done state of the Mark complete button (on Done Mint, #e1f3ea; dark #133b33).
- **Caution Amber** (#8a5300; dark #ffc76b): "try again" quiz results and "try this" feedback icons. Soft tint #fff1d6 (dark #3b2c12).

### Neutral
- **Chart White** (#f3f5fb; dark #0d1430): the page ground.
- **Rail Tint** (#e7ebf8; dark #111a3b): the lesson rail and the mobile top bar.
- **Surface** (#ffffff; dark #151f42): cards, panels, tiles, buttons, inputs, the dialog.
- **Surface Raised** (#f6f8fd; dark #1a254d): button hover and the checklist box.
- **Sunk** (#eceff8; dark #0f1736): code snippets, the feedback box, the tab track, the preview well.
- **Ink Navy** (#0f1838; dark #e6eaf7): all primary text, tile borders, the current step and current table column.
- **Slate** (#4a5675; dark #a6b1ce): secondary text, captions, counts, icons at rest.
- **Rule** (#d6dceb; dark #2a3663): card borders and dividers.
- **Strong Rule** (#b3bcd4; dark #46538a): button, input, empty-tile and step-dot borders.
- **Editor Ink** (#0f1838 background, #e3e8f8 text; dark background #0a1027): the code editor. Selection is #3550d6.

### Dark mode
Every colour above is a CSS custom property redefined inside `@media (prefers-color-scheme: dark)`. Components never pick colours directly; they use the tokens, so they switch automatically. On dark, text on a family fill flips from white to deep ink (#0d1430).

### Named Rules
**The Colour Has A Job Rule.** Cobalt, magenta and yellow appear only to say which family something belongs to, or to mark the one primary action (cobalt Run preview). Never use a family colour as decoration.

**The Green Means Done Rule.** Green is reserved for completion and correctness. It is never used for code text, headings, or atmosphere.

**The Ink On Yellow Rule.** Anything sitting on Signal Yellow is ink navy, never white. Yellow-family text on a white surface uses Plan Ink (#8a6200).

**The Family Hook Rule.** To give an element a family colour, add `fam-html`, `fam-css` or `fam-plan`. The hook sets `--fam` (fill), `--on-fam` (text on fill), `--fam-soft` (tint) and `--fam-ink` (text on white). Swatches, session chips, tiles and table tiles all read these four variables; nothing hard-codes a family colour.

## Typography

**Display Font:** Archivo, variable width and weight (with system-ui, -apple-system, Segoe UI, Roboto, sans-serif)
**Body Font:** Archivo at normal width (same fallbacks)
**Label/Mono Font:** JetBrains Mono (with ui-monospace, SFMono-Regular, Consolas, monospace)

**Character:** One grotesk does two jobs. Pushed wide and heavy it becomes the chart's voice for symbols and headings; at normal width and weight it is a calm reading face. Mono is kept for real code and element names, so anything in mono is something the student could type. Both fonts are self-hosted from `fonts/` under the SIL Open Font License.

### Hierarchy
- **Symbol** (820, 32px, width 125%, line-height 1, -0.02em; 26px under 800px): the big letters on element tiles. The table tiles in the rail use the same face at 12.5px, weight 760.
- **Display** (820, clamp(27px, 2.4vw, 35px), width 118%, line-height 1.1, -0.022em; 25px under 800px): the lesson title. One per screen.
- **Headline** (760, clamp(21px, 1.8vw, 25px), width 112%, line-height 1.15, -0.015em; 22px under 800px): the page title. The dialog title is the same family at 23px, weight 800.
- **Title** (760, 15.5px, width 110%): section headings inside a lesson and inside the dialog. Panel titles are 14.5px, weight 700, width 108%. The brand name is 17px, weight 760, width 112%.
- **Intro** (400, 17.5px, line-height 1.5): the first paragraph of each lesson.
- **Body** (400, 15px, line-height 1.55): everything else. Lesson paragraphs stop at 68ch.
- **Control** (560, 14px): buttons. Primary and ink buttons go to 650.
- **Label** (650, 12 to 12.5px, tabular numbers): atomic numbers, session group labels, step numbers, counts. Sentence case; never uppercase or letter-spaced.
- **Code** (JetBrains Mono 400, 13.5px, line-height 1.65 to 1.7): the editor and code snippets. Reflection notes use 13px.
- **Code small** (JetBrains Mono 650, 11.5px): element names on tiles, e.g. `background-color`. Plan-family tile names are not code and use Archivo at 12.5px instead.

### Named Rules
**The Wide Means Chart Rule.** Width above 100% (font-stretch 108 to 125%) is for the chart voice only: symbols, titles, headings, the brand. Reading text, buttons and labels stay at normal width.

**The Mono Means Typeable Rule.** Use the mono face only for text a student could type into the editor: code, element and property names. Plain-language names stay in Archivo.

**The Numbers Line Up Rule.** Every number that counts something (atomic numbers, lesson steps, "14 of 21 elements") uses tabular figures.

## Layout

The page is a two-column workbench: a sticky lesson rail on the left (328px wide, full height, scrolls on its own) and a main area capped at 1640px. Inside main, a header row (title and byline left, Download and save status right, a rule underneath) sits above a two-column workspace: the lesson card (minmax(340px, 1fr)) and the studio (editor panel above preview panel, minmax(440px, 1.2fr)), with a 24px gap.

The rail holds, top to bottom: brand, tagline, the lesson list grouped by session, the "Your table" card (an 8-column grid, one column per lesson, 4px gaps), the family legend and lesson count, then session notes and the MDN link.

Spacing works on small steps: 4px inside the table, 6 to 8px between tiles and inside button groups, 12 to 16px inside cards and panels, 18 to 24px between sections, and 28px for the lesson card's padding and the main area's top padding.

**Responsive behaviour:**
- **1600px and wider:** the workspace leans toward the studio (0.95fr / 1.25fr) and the editor and preview grow taller (340px and 380px).
- **1150px and narrower:** the rail narrows to 276px. The workspace stacks: lesson card first, then the studio, whose editor and preview sit side by side. Pill-shaped jump links (Lesson, Code editor, Preview) appear under the header.
- **800px and narrower:** the rail becomes a menu. A sticky top bar in Rail Tint shows a smaller brand tile and a "Lessons & progress" button that opens the rail above the content. Everything is a single column; Mark complete moves to a full-width row above Back and Next.
- **480px and narrower:** the lesson's element tiles drop from 4 per row to 3.

Touch targets are at least 42px (buttons) and 44px (inputs, lesson links, summaries, utility buttons on mobile).

## Elevation & Depth

Mostly flat. Depth comes from tonal layering (Chart White ground, white Surface cards, Sunk wells inside them) plus thin rules. Shadows are soft and small, and there are only two.

### Shadow Vocabulary
- **Rest** (`box-shadow: 0 1px 2px rgb(15 24 56 / 0.07)`; dark `0 1px 2px rgb(0 0 0 / 0.28)`): lesson card, panels, and the current lesson link. Just enough to lift a white card off a pale ground.
- **Lift** (`box-shadow: 0 2px 4px rgb(15 24 56 / 0.08), 0 14px 32px rgb(15 24 56 / 0.12)`; dark uses black at 0.3 and 0.35): the session notes dialog only, over a 55% ink-navy backdrop.

### Named Rules
**The Two Shadows Rule.** Cards rest on the Rest shadow; only things that float above the page (the dialog) use Lift. Tiles never have shadows: they are printed on the chart.

**The No Glow Rule.** No coloured shadows, no outer glows, no neon. Emphasis comes from fill and ink, not light.

## Shapes

Two corner families. **Chart pieces are nearly square:** element tiles 4px, table tiles, step numbers and task numbers 3px, family swatches 2px. **Interface pieces are gently rounded:** buttons and inputs 7px, tab buttons 6px, snippets and lesson links 8px, the tab track 9px, the "Your table" card 10px, the lesson card and panels 12px, the dialog 14px. Fully round shapes are reserved for small status dots and the mobile jump pills.

Borders are 1px. Chart pieces use an ink border (element tiles, task numbers) or a Strong Rule border (empty table tiles, step numbers); cards and panels use the lighter Rule. The current table column's tiles thicken to 1.5px.

### Named Rules
**The Square Means Element Rule.** If it is an element, a step number, or a swatch, its corners are 4px or less. If it is something you click or read inside, it is rounded 6px or more. Keep the two apart so the chart reads as a chart.

## Components

### Buttons
Plain and sturdy, like classroom equipment.
- **Shape:** gently rounded (7px), at least 42px tall, 9px 14px padding, an 18px stroke icon before the label with an 8px gap.
- **Default:** white Surface, Strong Rule border, ink text. Hover moves to Surface Raised with a Slate border. Pressed nudges down 1px. Disabled drops to 45% opacity.
- **Primary (cobalt):** HTML cobalt fill, white text, weight 650. One per panel; used for Run preview. Hover mixes in 18% ink.
- **Ink:** ink-navy fill with white text, used for Mark complete. When the lesson is done it becomes Done Mint with a green border and a green check.
- **Pressed toggle:** utility buttons with `aria-pressed="true"` use the cobalt soft tint with a cobalt border.
- **Focus:** a 3px cobalt outline, offset 2px, on everything focusable.

### Tabs (segmented control)
- **Style:** a Sunk track (9px radius, 3px padding) holding transparent 36px buttons in Slate text. The pressed tab becomes a white chip with ink text, a 1px Rule ring and a hairline shadow. HTML and CSS tabs carry their family swatch; Wide and Narrow carry stroke icons.

### Cards / Containers
- **Corner Style:** 12px for the lesson card and panels, 10px for the table card.
- **Background:** white Surface on the Chart White ground.
- **Shadow Strategy:** Rest shadow (see Elevation & Depth).
- **Border:** 1px Rule.
- **Internal Padding:** 28px on the lesson card (24px under 1150px, 20px 18px under 800px). Panels have a 10px 12px header bar with a bottom rule.

### Inputs / Fields
- **Style:** white Surface, 1px Strong Rule border, 7px radius, at least 44px tall. Reflection notes are textareas in mono (13px) and resize vertically.
- **Hover / Focus:** hover darkens the border to Slate; focus uses the global 3px cobalt outline.
- **Checklist:** native checkboxes tinted Done Green, inside a Surface Raised box.

### Navigation
- **Lesson list:** grouped under a label with a family swatch ("Session 1 · HTML"). Each lesson link is a full-width 44px row: a 26px square step number, the title, and a green check when done. Hover gives a faint white wash. The current lesson is a white card with a Rule border, Rest shadow and an ink-filled step number. Done lessons get green step numbers.
- **Mobile:** a sticky top bar with the brand and a "Lessons & progress" button replaces the rail; jump pills link to Lesson, Code editor and Preview.

### Element Tile (signature component)
The heart of the system: a periodic-table square for one HTML element, CSS property, or planning step.
- **Anatomy:** atomic number top-left (Label, 11.5px, tabular), the symbol (Symbol style, 32px wide and heavy), the name in small mono, then a one-line plain-English definition (12px). A small check appears top-right once collected.
- **Size:** up to 116px wide, at least 120px tall, 8px 9px 10px padding, 4 per row (3 under 480px), 8px gaps (6px on mobile).
- **Empty:** white Surface with a 1px ink border. Number and symbol use the family's text colour (`--fam-ink`), so you can tell the family before it is collected.
- **Collected:** the family colour fills the tile, the border takes the family colour, and all text flips to the on-fill colour.

### Table Tile
The small version in "Your table". Square (aspect ratio 1), 3px corners, Strong Rule border, Slate symbol at 12.5px weight 760. Tiles in the current lesson's column get the family soft tint and a 1.5px border, and the column number above them turns into an ink chip. Collected tiles fill with the family colour. Hovering or focusing a tile shows its name and definition in an ink tooltip with 6px corners above it. Arrow keys move between tiles.

### The Fill (signature motion)
When a lesson is marked complete, its tiles fill with family colour from the bottom up, one after another.
- **Fill:** the colour layer scales from 0 to full height over 0.6s with the house ease (cubic-bezier(0.16, 1, 0.3, 1)), each tile starting 110ms after the one before.
- **Text:** tile text turns to the on-fill colour just after the fill passes (120ms later in the table, 180ms later on lesson tiles); the check pops in last (380ms later).
- **Everything else:** interface transitions are 0.15s; tooltips 0.15 to 0.2s; disclosure chevrons rotate in 0.25s.
- **Reduced motion:** with `prefers-reduced-motion: reduce`, all animation and transition times drop to near zero and delays are removed. Tiles still end up filled.

### Code Editor and Preview
- **Editor:** the one dark surface in light mode: Editor Ink background, pale text, JetBrains Mono 13.5px at 1.7 line height, 18px 20px padding, a yellow caret, cobalt selection. Below it, a note row in 12.5px Slate with a status dot (green when up to date, yellow with an amber ring when stale).
- **Preview:** the student's page sits in a white iframe with a 1px Rule border and 6px corners, inside a Sunk well. The iframe stays white in dark mode because it shows the student's own page.

### Code Snippet
Example code inside lessons: a Sunk box with a Rule border, 8px corners, 14px 16px padding, mono 13.5px at 1.65, wrapping long lines.

### Dialog
Xavier's session notes: white Surface, 14px corners, 26px 30px 30px padding, Lift shadow, max 640px wide and 85% of the screen tall, over an ink-navy backdrop at 55%.

## Do's and Don'ts

### Do:
- **Do** give anything that belongs to a family the `fam-html`, `fam-css` or `fam-plan` hook and colour it through `--fam`, `--on-fam`, `--fam-soft` and `--fam-ink`.
- **Do** build new element tiles with the full anatomy: atomic number top-left, wide heavy symbol, mono name, short definition, square corners (4px or less), 1px ink border when empty.
- **Do** keep text on Signal Yellow ink navy (#0f1838), and use Plan Ink (#8a6200) for yellow-family text on white.
- **Do** use Done Green only for completion and correct answers.
- **Do** add every new colour as a custom property in both the light `:root` and the dark-mode block, so dark mode keeps working.
- **Do** use the Fill (bottom-up, 0.6s, 110ms stagger, house ease) for collecting elements, and keep the reduced-motion override.
- **Do** keep buttons at least 42px tall and inputs and list rows at least 44px, with the 3px cobalt focus ring visible.
- **Do** use stroke icons from the page's SVG sprite (24px viewBox, 1.8 stroke, round caps) at 18px.

### Don't:
- **Don't** make it look like a hacker movie: no black backgrounds, no green code text, no neon glows. Dark mode is deep ink-blue (#0d1430).
- **Don't** use a family colour for decoration, backgrounds of whole sections, or headings. Colour means a family.
- **Don't** put white text on Signal Yellow.
- **Don't** round chart pieces (tiles, swatches, step numbers) beyond 4px, or square off buttons and cards below 6px.
- **Don't** add shadows to tiles, or shadows beyond the Rest and Lift pair.
- **Don't** use the wide font widths for body text, buttons or labels, and don't uppercase or letter-space labels.
- **Don't** set code in Archivo or plain-language names in mono.

## Addendum: five element families

The 12-lesson curriculum adds two families to the original three. Each keeps the same job-per-colour rule and the `.fam-*` hook (`--fam`, `--on-fam`, `--fam-soft`, `--fam-ink`).

| Family | Light | Dark | Used for |
|---|---|---|---|
| JavaScript behavior (`.fam-js`) | `#c2410c` | `#ff9a62` | querySelector, addEventListener, classList, toggle; the JS editor tab |
| AI skills (`.fam-ai`) | `#6d3fd6` | `#b49bff` | Session 2 AI tiles (prompts, iteration); the Session 2 marker |

"Your table" now has 40 tiles in a 6-column grid: lessons 1–6 on the first row, 7–12 on the second. Code fonts render with ligatures off, so `=>` shows exactly as typed.
