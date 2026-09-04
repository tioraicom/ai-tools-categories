# Changelog

Notable changes to this taxonomy. Typo fixes and small wording tweaks are not logged.

The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## 1.1.0 — 2026-09-04

### Added

- The full taxonomy in both READMEs. All 182 categories now render on the page, grouped
  under their top-level parent and sorted by name, with each subcategory's description and
  slug. The section is generated from `data/categories.json`, so it cannot disagree with the
  data files.
- Arabic names and descriptions for all 182 categories, written in Arabic rather than
  translated from the English line.

### Changed

- `Contents` in both editions now lists the twenty top-level categories, so a reader reaches
  any group in one click.

### Removed

- The top-level-only summary table, superseded by the full listing. Reading the taxonomy no
  longer requires downloading a data file.

## 1.0.0 — 2026-09-04

Initial public-ready release.

### Added

- 182 categories across two levels as JSON and CSV: 20 top-level and 162
  subcategories, each with a stable slug, a parent, a description, and aliases.
- Categories: Writing and content, Image generation and editing, Video, Audio, music, and voice, Coding and development, Developer infrastructure and models, Chatbots and assistants, Automation and agents, Productivity and workflow, Presentations and documents, Design and creative, Marketing and advertising, SEO and search, Sales and CRM, Customer support, Data and analytics, Research and knowledge, Education and learning, Business and finance, and Health and lifestyle.
- Contribution files: `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md` (Contributor Covenant 2.1),
  `SECURITY.md`.
- `LICENSE` — CC BY 4.0, canonical text.
- Issue forms for suggesting a category and reporting a broken link, plus a pull
  request template and issue template configuration.
- `.editorconfig`, `.gitattributes`, and `.gitignore`.
- `FEATURES.md` — what ships now, what is committed, and what is only an idea.

### Notes

- The dataset names no products and makes no claims about any vendor, so it carries no links
  that can rot. The release check is structural: every parent and every child reference
  resolves, no name appears twice anywhere in the tree, and no level-2 node has children.
- The data validates against `data/schema.json`, which was tested to reject a level-3 node and a
  malformed slug. Referential integrity is not something JSON Schema can express, so the
  dangling-parent and duplicate-name checks are in the build instead, and block the release.
- Every code sample in the README was run against the shipped data.
- Licensed under CC BY 4.0. A content licence rather than a software licence, because this repository is category names, descriptions, and structure rather than code.
