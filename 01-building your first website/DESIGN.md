---
name: Building Your First Website
description: Neumorphism (Soft UI). One light grey surface; everything is pressed out of it or into it, lit from the top left. Element tiles from a "Periodic Table of the Web" press in as students learn.
colors:
  bg: "#e0e5ec"
  bg-2: "#f0f0f3"
  shadow-dark: "#b8bcc2"
  shadow-light: "#ffffff"
  heading: "#2b2f36"
  ink: "#333333"
  ink-2: "#545b66"
  control-ink: "#3d434c"
  error-ink: "#a3125c"
  accent: "#6d5dfc"
  html: "#2546e8"
  css: "#c2186e"
  js: "#c2410c"
  ai: "#6d5dfc"
  plan: "#8a6200"
  ok: "#0e7c55"
  warn: "#8a5300"
radius: { md: 12px, lg: 16px, xl: 24px }
motion: "300ms ease-in-out on every transition"
---

# Design system: Neumorphism (Soft UI)

All tokens live in `:root` in `style.css`.

## Surface and light
- One surface colour, `#e0e5ec`, for the page, rail, cards, buttons, and inputs. There are no borders, gradients, or pure white or black backgrounds.
- Light always comes from the top left: the white highlight sits at −X/−Y and the `#b8bcc2` shadow at +X/+Y.
- **Raised** (`--out-*`) means "you can press this", or a card. **Inset** (`--in-*`) means a channel (editor, inputs, preview, snippets, checks) or something already pressed (current lesson, selected tab, open hint, collected tile).
- Cards use `--out-lg` (8/16px) on desktop and `--out-sm` (4/8px) under 800px.

## Interaction physics
- Buttons: raised by default, a **smaller** shadow on hover, inset on press (`:active`). Nothing ever moves with `translate`.
- Inputs and the editor: a deep inset that **relaxes** to `--in-xs` on focus, plus a 2px accent ring for keyboard users.
- Toggles (`aria-pressed="true"`) and the current lesson stay inset.

## Colour has a job
- The accent `#6d5dfc` is used only for primary actions (Run preview, Mark complete), the brand tile, and the current lesson.
- Family colours appear only as tile symbols and small dots: HTML is blue, CSS magenta, JS orange, AI violet, and plan/test ochre. Green means done; amber means try again.
- Text is `#333` on `#e0e5ec` (about 9:1); secondary text `#545b66` is about 5:1.

## Type
- Archivo (self-hosted) for the interface; JetBrains Mono for code, with ligatures off so `=>` shows as typed.

## Signature: Periodic Table of the Web
- Each lesson shows its elements as raised tiles: a number, a symbol in its family colour, the name, and a definition. When a lesson is marked complete, its tiles press into the surface one after another (110ms stagger) and a check appears.
- "Your table" in the rail has 40 small tiles in a 6-column grid (lessons 1–6, then 7–12). It has one tab stop, arrow-key movement, and a tooltip on hover or focus.

## Playground
- `playground.html` reuses the same tokens: an editor panel (HTML/CSS/JS tabs, Auto-run), a preview panel with Phone 375 / Tablet 768 / Desktop widths, and an inset console.

## Responsive
- 1150px: narrower rail; lesson stacked above editor and preview.
- 800px: top bar and menu, single column, smaller shadows.
- 480px: three tiles per row.
- Reduced motion turns transitions off.
