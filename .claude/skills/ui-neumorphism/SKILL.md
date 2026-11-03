---
name: ui-neumorphism
description: Build or restyle web UI in strict Neumorphism (Soft UI) — one light grey surface, dual top-left-lit shadows, raised controls that press inset, no borders or gradients. Use when the user asks for neumorphism, neumorphic, soft UI, 新拟物 / 新拟物派, "the workshop style", or wants a page to match the DigitalFuture-Learning workshop look. Works for plain CSS or Tailwind.
---

# UI Neumorphism (Soft UI)

Generate interfaces that look pressed out of, or into, one soft clay-like surface. Follow these rules exactly and do not drift into other styles. When rules conflict, the **Never** list wins, except where accessibility requires an exception (see Accessibility).

For ready-to-paste CSS tokens and components, read `reference/tokens.css`. For Tailwind class equivalents, read `reference/tailwind.md`.

## The physics

- **One surface.** Use `#e0e5ec` for the page and every element on it (`#f0f0f3` for a lifted surface such as a tooltip). Elements share the background colour; shadows alone create shape.
- **Fixed light source, top left.** The white highlight is always at −X/−Y and the dark shadow `#b8bcc2` always at +X/+Y. Never flip it.
- **Raised** = can be pressed, or a card: `8px 8px 16px #b8bcc2, -8px -8px 16px #ffffff` (blur = 1.5–2× the offset).
- **Inset** = a channel (inputs, editor, display, well) or something already pressed (selected tab, current item, open disclosure): `inset 8px 8px 16px #b8bcc2, inset -8px -8px 16px #ffffff`.
- **Corners** 12–24px everywhere. Small dots and step numbers may be circles.
- **Motion:** every transition is `300ms ease-in-out` (Smooth Molding).

## Interaction states

| Element | Default | Hover | Active / selected | Focus |
|---|---|---|---|---|
| Button | raised 6–8px | **smaller** shadow, 3–4px | inset 4px | 2px accent outline, offset 3px |
| Primary button | accent `#6d5dfc` fill, white text, raised | smaller shadow | inset in accent tones (`#5246c9` / `#8a7dff`) | same ring |
| Input, textarea | inset 6px | — | — | inset **relaxes** to 2px, plus a 2px accent ring |
| Tabs | inset track; selected tab raised 3px | — | pressed tab inset | ring |
| Toggle (`aria-pressed="true"`) | stays inset | — | — | ring |
| Disabled | opacity .5, small shadow | no change | no change | — |

- **Extrude to Intrude:** pressing switches the shadow from outer to inset. Never use `translate` or `scale`; the element is part of the surface and does not float.
- **Hover Shadowing:** hover always *shrinks* the shadow, as if a finger is blocking the light. Never grow it.

## Colour

| Role | Value |
|---|---|
| Surface | `#e0e5ec` (lifted `#f0f0f3`) |
| Shadow dark / light | `#b8bcc2` / `#ffffff` |
| Heading text | `#2b2f36` |
| Body text | `#333333` (about 9:1 on the surface) |
| Secondary text | `#545b66` (about 5:1; do **not** use `#6b7280`, it fails AA) |
| Accent (primary actions only) | `#6d5dfc` |
| Supporting accents (small marks only) | `#ff6b6b`, `#4ecdc4`, `#ffe66d` |

Keep colour for meaning: primary actions, status dots, and small category marks. Large areas stay surface grey. No high-contrast blocks.

## Never

- Pure white or black backgrounds, or dark mode (this style is light only).
- High-contrast colour blocks, gradients (`bg-gradient-*`, `linear-gradient` fills), gradient text.
- Borders of any kind used for shape (`border`, `border-2`+); hairline dividers too. Use spacing or an inset groove.
- Square corners (`rounded-none`, `rounded-sm`) or stock shadows (`shadow`, `shadow-md`, `shadow-lg`…).
- Hard offset shadows (`4px 4px 0`), glows, glassmorphism.
- `translate` or `scale` on buttons; a larger shadow on hover; a deeper inset on focus.
- Bounce or elastic easing.
- Cards inside cards. Inset wells (an input, a preview, a console) inside a raised card are correct; a raised card inside a raised card is not.
- Tiny uppercase tracked eyebrows above headings, or a thick coloured stripe on one side of a card.
- Inter, Roboto or Geist as the type voice. Pick a characterful sans (the workshop uses Archivo) and a mono for code.

## Accessibility (these override the style where they conflict)

- Text meets WCAG AA: 4.5:1 for body text, 3:1 for large text. Check every text colour against `#e0e5ec`, including hover colours.
- Keyboard focus must be visible. The spec's "focus:outline-none" is allowed only when a 2px accent ring replaces the outline (`box-shadow: …, 0 0 0 2px #6d5dfc`).
- Never use shadow alone to carry state. Pair inset/raised with text, an icon, or `aria-pressed` / `aria-current`.
- Touch targets are at least 44px.
- Provide a `prefers-reduced-motion: reduce` block that removes transitions.
- Turn off code ligatures (`font-variant-ligatures: none`) in code areas so `=>` shows as typed.

## Responsive

- Phones (under 800px): halve shadows (cards 4px/8px, buttons 4px).
- Desktop: cards 8px/16px.
- Spacing: padding 16–32px, gaps 16–32px; give raised elements at least about 1.5× their shadow offset of breathing room, so shadows don't collide.

## Workflow

1. Define the tokens from `reference/tokens.css` (or the Tailwind values) first.
2. Build the layout with a clear hierarchy: size and weight for importance, not colour.
3. Assign each element exactly one role: **raised** (pressable or card), **inset** (channel or selected), or **flat** (text).
4. Implement all states in the table above.
5. Run the checklist before delivering.

## Checklist

- [ ] Background is `#e0e5ec` (or `#f0f0f3` for lifted surfaces); there's no white, black, or dark mode.
- [ ] Every shadow is a dual pair, highlight at −X/−Y and dark at +X/+Y.
- [ ] Buttons: hover shrinks the shadow and active turns inset, with no translate or scale.
- [ ] Inputs: inset by default, relaxing on focus, with a visible ring.
- [ ] Corners are 12–24px; there are no borders or gradients.
- [ ] Transitions are `300ms ease-in-out`, and a reduced-motion fallback exists.
- [ ] All text passes AA, and focus is visible on every control.
- [ ] No raised card sits inside a raised card.
- [ ] Shadows are smaller on phones, and nothing scrolls sideways at 390px.
- [ ] It is still recognisable as Neumorphism at a glance.

## Example in this repo

`01-building your first website/style.css` and `playground/index.html` are full working examples: a lesson rail, cards, segmented tabs, inset editors, a preview well, a console, a dialog, and tiles that press in when completed.
