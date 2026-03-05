# Copilot Instructions

## Project Overview

This is a static personal portfolio site deployed via GitHub Pages at `mehul-sethi.github.io`. It consists of a single `index.html` file with inline CSS — no build tools, frameworks, or JavaScript.

## Architecture

- **`index.html`** — The entire site: markup, styles (inline `<style>` block), and content. There is no external CSS or JS.
- **`profile.jpg`** — Profile photo referenced by both `index.html` and `README.md`.
- **`Mehul_CV.pdf`** — Downloadable resume linked from the page.
- GitHub Pages serves from the `main` branch root.

## Conventions

- All styling is kept in the inline `<style>` block within `index.html` — do not introduce external stylesheets.
- The design uses CSS custom properties (`:root` and `[data-theme="dark"]`) for theming. Light mode is a golden-orange "Cosmic Orange" gradient; dark mode uses dark charcoal backgrounds with the same orange accent.
- All colors reference CSS variables (`var(--accent)`, `var(--card-bg)`, etc.) — never hardcode color values.
- A small inline `<script>` at the end of `<body>` handles the dark mode toggle, persisting the choice in `localStorage` and defaulting to `prefers-color-scheme`.
- The page is responsive via a `@media (max-width: 768px)` block at the end of the styles.
