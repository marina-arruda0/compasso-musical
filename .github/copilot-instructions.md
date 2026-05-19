# Copilot Instructions for compasso-musical

This repository is a small static website built from a single HTML page and local image assets.

## What matters

- The main source file is `index.html`.
- There is no build tool, package manager, or test suite in the repo.
- All assets are referenced locally from the repository root (for example `guitarra.jpg`, `violão acustico.jpg`, `banda rock.jpg`).
- The page is written in Portuguese (`<html lang="pt-BR">`), so preserve existing language and text tone.

## Project structure

- `index.html` contains the full site layout:
  - Header/navigation
  - Hero section
  - Sobre (about)
  - Instrumentos section with product cards
  - Depoimentos section
  - Contato section with a contact form
  - Footer with social links
- There is no separate CSS or JS file currently.

## Developer guidance for edits

- Keep changes compatible with a static HTML workflow: update `index.html` and preview in a browser.
- Do not introduce build scripts, npm dependencies, or frameworks unless explicitly requested.
- When adding styles, create a new CSS file and add a `<link rel="stylesheet">` into `index.html`.
- Preserve local image references and avoid converting them to CDN/image-hosting URLs unless the user asks.

## Specific code patterns

- Navigation uses anchor links to section IDs: `#hero`, `#Sobre`, `#Instrumentos`, `#Depoimentos`, `#Contato`.
- Product blocks are written as `<article>` elements with `h3`, `img`, descriptive `<p>`, and an action link.
- The contact form is bare HTML and currently uses plain `<form action="">` with no JavaScript handling.

## Fixes or improvements

- Prefer semantic HTML and correct tag nesting when editing `index.html`.
- Example: close `<section>` tags in the right order and avoid nested sections that break content structure.
- Use descriptive alt text for images and keep the Portuguese copy consistent.

## When to ask the user

- If a feature requires JavaScript behavior (cart functionality, form submission, interactive UI), ask whether to add vanilla JS or a richer implementation.
- If styling is needed, confirm whether to keep it minimal or build a more complete stylesheet.
