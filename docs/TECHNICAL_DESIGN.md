# Technical Design Document (TDD) — Mansion Docs

## 1. CodeGraph AST & Component Structure
- **Framework**: Docusaurus 2+ / React (`package.json`, `docusaurus.config.js`).
- **Sidebar Configuration**: Structured category definitions (`sidebars.js`).
- **Assets & Media**: Versioned application screenshots and diagrams (`static/`, `screenshots/`).
- **Markdown & MDX**: Standard CommonMark content with custom React callout components (`docs/intro.md`, `docs/*`).

## 2. Build & Deployment Specifications
- **Package Manager**: npm (`package-lock.json`).
- **Build Pipeline**: `npm run build` generates output in `build/`.
- **Hosting**: GitHub Pages via GitHub Actions workflow (`.github/workflows/deploy.yml`).
- **Quality Gates**: Markdown link validation, image asset existence checks, and clean bundle compilation without dead links.
