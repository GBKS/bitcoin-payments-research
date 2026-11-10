# CLAUDE.md

Guidance for Claude (and any other contributor) working in this repository.

## What this is

**bitcoin-payments-research**: a public research notebook asking where demand for bitcoin payments could actually come from. It's written by a designer building a bitcoin wallet, and that perspective shapes which areas are studied, but the research itself stays neutral. It's experimental, with no promise of ongoing maintenance.

It will be published with GitHub Pages (Jekyll), with a very simple look inspired by Apple's Human Interface Guidelines.

## Structure

- `00-start-here.md`: entry point (also the site's home page), working thesis, areas and status, what we've learned so far, log.
- `01-method.md`: principles, say/do/make, quick-scan and deep-dive templates, evidence labels, file conventions.
- `02-landscape.md`: context (Spiral's posts, payments in numbers, cost baseline, lessons from other payment systems, key projects).
- `03-stablecoins.md`: what "stablecoins" covers, and who wants dollars and who doesn't.
- `11`–`18`: research areas. `11`, `12`, `14` and `16` are deep dives; the others are quick scans. `11a` and `11b` are the group orders teardown and research kit.
- `90-auto-research.md`: where AI agents could do research work (checking claims, keeping numbers current), the one-page pilot and its results.
- `claims/`: claims lists per page (`NN-short-name.yml`, format in `90-auto-research.md`) and pilot audit sheets. GitHub-only (excluded from the site). When a page's wording changes, keep the `text` of its claims in sync.
- `TODO.md`: open work, assumptions to check, items marked **help wanted**.

File naming: `00`–`09` entry and foundation, `11`–`29` areas (`NN-short-name.md`), `90`–`99` cross-cutting.

## Rules for content

1. **Neutral research.** Never assume a particular product. Sections on "What could serve this" compare kinds of product and kinds of wallet; they don't recommend one.
2. **Public sources only.** Use public sources or sources that can be attributed openly. Nothing learned in private conversations goes here.
3. **Never reference private material.** A separate private folder of product strategy exists outside this repo. Never link to it, name its files, or link to anything outside this repo (no `../` paths).
4. **Label what isn't verified,** inline in square brackets and italics: *[from memory]*, *[assumption]*, *[from earlier research]*, *[to verify]*. Anything unlabeled must link to a source that was actually opened.
5. **Say versus do.** Every scan notes where what people say differs from what they do.
6. **People's privacy.** Anonymize individuals and small community accounts (for example group order managers), even when their pages are public. No minors.
7. **Dates:** each file has a status line and "Last updated" date in italics under the title; update it when editing.

## Writing style

- Plain, clear English. Short sentences and paragraphs. Specifics over adjectives: numbers with units, names, dates.
- Lead with the point; avoid filler, hype and jargon (explain terms like Ark, Lightning, BOLT-12 on first use where needed).
- Tables for comparisons, bullet lists for parallel items, prose for arguments.
- American spelling.

## Links

- Use standard relative Markdown links with the target's title as link text, for example `[Stablecoins, unpacked](03-stablecoins.md)`. No Obsidian `[[wikilinks]]`.
- These work in Obsidian, on GitHub, and on GitHub Pages (which converts `.md` links to page links).

## The site (GitHub Pages, Jekyll)

Goal: extremely simple, inspired by Apple's Human Interface Guidelines, without using Apple's fonts, icons or branding.

- **No theme; a minimal custom setup:** `_config.yml`, one layout (`_layouts/default.html`), one stylesheet (`assets/style.css`), and `_data/nav.yml` for sidebar sections and order.
- **Keep the Markdown files plain:** no front matter required. GitHub Pages takes titles from the first heading (jekyll-titles-from-headings), handles files without front matter (jekyll-optional-front-matter) and converts relative `.md` links (jekyll-relative-links). Set defaults in `_config.yml` so every page uses the layout.
- **Home page:** `00-start-here.md` (set as the site index, for example via a permalink default or a small `index.md` that includes or redirects to it). A short `README.md` serves the repo on GitHub.
- **Look:** `system-ui` font stack; large bold page titles; larger lead paragraph; generous whitespace; narrow reading column; one accent color; quiet tables; light and dark mode via `prefers-color-scheme`.
- **Header:** site title on the left, a GitHub link on the right (from `repository` in `_config.yml`).
- **Left sidebar:** grouped sections (Getting started, Foundation, Research areas, Deep-dive materials, Cross-cutting, To do) that can be collapsed, current page highlighted; single-page sections show as plain links. No filter box.
- **Right "On this page":** built from each page's `h2` headings with a small script.
- **Status line:** the italic paragraph directly under each page title renders as a light gray rounded card.
- Mobile: sidebar collapses behind a menu button.
- No search, analytics, comments or custom domain for now.
- Keep `TODO.md` on the site (it invites contributions); exclude `CLAUDE.md` from the site via `_config.yml`.

## Repository

- Public repo: `bitcoin-payments-research`. License: CC BY 4.0 for the content (add `LICENSE`).
- `.gitignore`: `.obsidian/`, `.DS_Store`, `_site/`, `.jekyll-cache/`.
- `README.md`: one paragraph on what this is, the author's perspective (a designer building a bitcoin wallet), "experimental, no promise of maintenance," how to contribute (issues and pull requests welcome; see `TODO.md` and `CONTRIBUTING.md`), license, and a link to the agent prompt in `CONTRIBUTING.md`.
- `CONTRIBUTING.md`: where to start, the content rules in short, pull request rules, and the agent prompt. The agent prompt lives only here; `README.md` and `90-auto-research.md` link to it. `README.md` and `CONTRIBUTING.md` are GitHub-only (excluded from the site).
- **Issues for claims to verify:** each item in the "To verify" list in `TODO.md` has an open issue labeled `to verify`. When an item is added or resolved, open or close its issue to match.
- Before every push: check the content rules above, especially rules 2, 3 and 6. Git history is permanent.
