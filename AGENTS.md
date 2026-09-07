# AGENTS.md

## Project overview

This repository is a small static web app for a cozy note-taking / writing interface. It is built with plain HTML and CSS and does not require a package manager, bundler, or build step.

Primary implementation files:
- [bloc.html](bloc.html)
- [cozy-ui.css](cozy-ui.css)

## Working conventions

- Keep the project as a lightweight static site: prefer simple HTML structure and CSS classes over introducing frameworks or tooling.
- Maintain the existing warm, soft visual language: pastel colors, rounded cards, subtle shadows, and friendly typography.
- Prefer small, targeted edits. This project is intentionally simple and easy to follow.
- Reuse the existing design tokens and class patterns in [cozy-ui.css](cozy-ui.css) before creating new ad hoc styles.
- If updating the interface, preserve accessibility basics: visible focus states, readable contrast, and keyboard-friendly controls.

## File responsibilities

- [bloc.html](bloc.html): page structure, content, layout, and interaction markup.
- [cozy-ui.css](cozy-ui.css): shared design system, theme variables, buttons, panels, inputs, and reusable visual utilities.

## Validation

There is no automated test suite or build command for this project.

Use one of these checks when validating work:
1. Open [bloc.html](bloc.html) in a browser, or use a simple local preview extension such as Live Server.
2. Confirm the layout still renders correctly without console errors.
3. If changing styles in [cozy-ui.css](cozy-ui.css), check the affected component in both desktop and narrow widths.

## Typical agent guidance

- Do not add frameworks, package.json files, or bundlers unless explicitly requested.
- Preserve the current design intent and avoid introducing heavy or cluttered UI patterns.
- Prefer CSS variables and existing utility classes over duplicate hard-coded colors and spacing values.
- Keep HTML semantic and readable; avoid unnecessary wrappers or over-engineering.
- When adding UI elements, follow the naming and styling patterns already established in the existing code.

## Useful next steps

If the app grows, the most natural extensions would be:
- adding lightweight JavaScript for note management,
- implementing local persistence via browser storage,
- or extracting repeated sections into reusable HTML/CSS patterns without changing the static-first approach.
