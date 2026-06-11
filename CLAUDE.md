# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Personal academic website for Jiaxuan Liu (USTC), built on the **HugoBlox Academic CV** template. This is a Hugo site — there is no application code to build; all "code" is content (Markdown/YAML) that Hugo renders to static HTML. The theme itself is consumed as a **Hugo Module** (Go module), not vendored, so editing layouts means either overriding files locally under `layouts/` or upgrading the module version in `go.mod`.

## Common commands

Hugo extended **0.119.0** is required (see `netlify.toml` / `.github/workflows/publish.yaml`). The Go module proxy is pinned to `goproxy.cn` in `config/_default/module.yaml`.

```bash
# Local dev server with live reload + future-dated content visible
hugo server -D -F

# Production build (matches GitHub Pages workflow)
hugo --minify

# Refresh theme modules after editing go.mod or imports
hugo mod get -u
hugo mod tidy

# Import publications from BibTeX → content/publication/ (also runs in CI on push of publications.bib)
pip install academic==0.10.0
academic import publications.bib content/publication/ --compact
```

There are no tests, linters, or build scripts beyond `hugo` itself.

## Architecture

### Content is the source of truth

Everything user-visible lives under `content/`, organized by **section** (Hugo's term for a top-level content type):

- `content/authors/admin/` — primary author profile; `username: admin` in homepage blocks resolves here. Other content types reference authors by folder name.
- `content/_index.md` — **the homepage**, assembled from a `sections:` list of blocks (`hero`, `about.biography`, `experience`, `accomplishments`, `collection`, `portfolio`, `contact`, etc.). Each block is a widget defined by the theme; editing the homepage means editing this YAML, not HTML.
- `content/publication/`, `content/post/`, `content/project/`, `content/event/`, `content/slides/` — auto-listed via `block: collection` filtered by `folders:` on the homepage. Each item is a folder with `index.md` + assets.

Permalink rewrites (e.g. `event/` → `/talk/:slug/`) and taxonomies (`tags`, `categories`, `publication_types`, `authors`) are configured in `config/_default/hugo.yaml`.

### Configuration is split, not monolithic

`config/_default/` is loaded in full by Hugo:
- `hugo.yaml` — site-wide settings (title, baseURL, taxonomies, output formats)
- `params.yaml` — theme-specific knobs
- `menus.yaml` — top nav
- `languages.yaml` — i18n config (single language: `en`)
- `module.yaml` — Hugo Module imports (theme + plugins)

When changing site behavior, identify which file owns the setting before editing — they are merged but not interchangeable.

### Theme override pattern

The Academic theme ships via three Hugo modules: `blox-bootstrap/v5`, `blox-plugin-netlify`, `blox-plugin-reveal`. To customize a layout, mirror the module's path under a top-level `layouts/` directory in this repo — Hugo's lookup order picks the local file first. Do NOT edit files inside the module cache.

### Deployment

Two paths are configured and **both are live** — be aware which one the user is deploying through before changing build commands:
- **GitHub Pages** via `.github/workflows/publish.yaml` (triggered on push to `main`).
- **Netlify** via `netlify.toml` (uses `hugo --gc --minify -b $URL`, with deploy-preview and branch-deploy contexts).

`baseURL` in `hugo.yaml` is `https://jiaxuanliu.netlify.app/`; the GH Pages workflow overrides it with `--baseURL` at build time.

### Publications auto-import

Dropping a `publications.bib` at the repo root and pushing to `main` triggers `.github/workflows/import-publications.yml`, which runs `academic import` and opens a PR titled "Hugo Blox Builder - Import latest publications" with the generated `content/publication/<slug>/` folders. Don't hand-edit those folders if you intend to re-import — the converter overwrites them.
