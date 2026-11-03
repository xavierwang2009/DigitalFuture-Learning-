# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

- **Students, grades 7–11** (about 10 per cohort) in Xavier Wang's two-session "Building Your First Website" workshop. Each student builds and owns one page, working in buddy pairs. They use the page both on classroom laptops (sometimes with Xavier projecting it) and on their own devices at home, in roughly equal measure.
- **Xavier, the facilitator**, who demonstrates changes, reads the session notes dialog, and checks understanding by asking students to explain their code.

## Product Purpose

A single-page, in-browser workshop that takes a beginner from an idea to a downloaded HTML file they wrote themselves. Eight lessons across two sessions (Session 1: HTML, Session 2: CSS) sit beside a real code editor and a live preview. Success is a student who can change a heading, explain a CSS rule, show one tested improvement, and leave with their own `my-first-website.html`.

## Positioning

Students edit real HTML and CSS, not blocks or templates, in a loop the page names: edit → run → observe → explain. No account, no server, nothing sent anywhere; progress lives only in the student's browser. Exercises are original and organized around MDN's beginner website guide (not an MDN course or endorsement).

## Operating Context

- Two in-person sessions plus practice at home; buddy pairs check each other's work.
- Classroom laptops (some Macs), a projector for demonstrations, and students' personal laptops or tablets.
- Xavier rehearses on every laptop before class: typing, Run preview, download, reopening the downloaded file.

## Capabilities and Constraints

- Static files only: `index.html` (markup + inline script) and `style.css`. No build step, framework, or backend.
- Features that must keep working: lesson navigation and progress (8 lessons, 2 sessions), mark complete / undo, back / next, notes fields, checklist, hints, quick understanding quiz, HTML/CSS editor tabs, Run preview, Wide/Narrow preview, Check my code, Ask AI for a hint (prompt helper only, no AI connection), Reset workspace, Download my website, Xavier's session notes dialog, mobile menu toggle, skip link.
- Saved state uses localStorage key `xavier-first-website-v1`; its shape must stay compatible so students keep their work.
- The preview iframe is sandboxed with a Content-Security-Policy; student HTML is sanitized (no scripts, forms, iframes, external resources) and links are inactive in preview.
- Lesson text, hints, quizzes, and session notes are content and stay word for word.

## Brand Commitments

- Title "Building Your First Website", byline "Xavier Wang's Instruction", sidebar name "Website workshop".
- The user asked for a technology theme. They explicitly rejected a "hacker-movie dark" look (black screens, green matrix text, glowing neon that is hard to read for long).

## Evidence on Hand

- The workshop's real lesson content, starter code, and session notes in `index.html`.
- No logos, photos, testimonials, or student work exist; none may be invented as real.

## Product Principles

1. The student's own code and page are the hero; the interface is the workbench around them.
2. Understanding over completion: explaining a change matters more than a checkmark.
3. Private by default: nothing leaves the browser, and the page says so plainly.
4. Readable in a lit classroom, on a projector, and on a small screen at home.

## Accessibility & Inclusion

- Audience aged roughly 12–17 with mixed experience; plain language.
- Full keyboard use with visible focus, a skip link, labelled controls, and live status messages must be preserved.
- Text must stay readable when projected and on narrow screens; touch targets of at least 42–44px.
