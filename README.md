# Jiaxuan Liu — Academic Website

Source for my personal academic site, **[jiaxuanliu.netlify.app](https://jiaxuanliu.netlify.app/)**.

I'm Jiaxuan Liu (刘佳璇), an M.Eng. student at the [National Engineering Research Center of Speech and Language Information Processing (NERC-SLIP)](http://nelslip.ustc.edu.cn/), University of Science and Technology of China. My research focuses on text-to-speech, expressive & emotional speech synthesis, multimodal movie dubbing, and speech foundation models.

The site is built with [Hugo](https://gohugo.io/) on top of the [HugoBlox Academic CV](https://github.com/HugoBlox/theme-academic-cv) theme, consumed as a Hugo Module — no fork, just config and content.

## Repository layout

- `content/authors/admin/` — author profile (bio, interests, education, socials)
- `content/_index.md` — homepage, assembled from widget blocks (`hero`, `about.biography`, `experience`, `collection`, `contact`, …)
- `content/publication/` — papers (`audiobook-tts`, `diffstyletts`, `fun-cineforge`, `uddetts`)
- `content/project/` — projects (`pinn-pde`, `road-damage-detection`, `wenxin-creative-app`, `xray-keypoint-detection`)
- `config/_default/` — site config (`hugo.yaml`, `params.yaml`, `menus.yaml`, `languages.yaml`, `module.yaml`)
- `layouts/`, `assets/`, `static/` — local theme overrides and static assets
- `publications.bib` — drop a BibTeX file here to auto-import publications via CI

## Local development

Requires Hugo extended **0.119.0** (matches `netlify.toml` and the GitHub Pages workflow).

```bash
# Live-reload dev server, including draft and future-dated content
hugo server -D -F

# Production build (same flags as the Pages workflow)
hugo --minify

# Refresh theme modules after editing go.mod or imports
hugo mod get -u
hugo mod tidy
```

The Go module proxy is pinned to `goproxy.cn` in `config/_default/module.yaml` for faster module fetches in mainland China.

## Importing publications

```bash
pip install academic==0.10.0
academic import publications.bib content/publication/ --compact
```

Pushing an updated `publications.bib` to `main` also triggers `.github/workflows/import-publications.yml`, which runs the importer and opens a PR with the regenerated `content/publication/<slug>/` folders. Don't hand-edit those folders if you intend to re-import — the converter overwrites them.

## Deployment

Two deploy paths are wired up and both are live:

- **Netlify** (primary, `https://jiaxuanliu.netlify.app/`) — configured in `netlify.toml`, with deploy-preview and branch-deploy contexts.
- **GitHub Pages** — configured in `.github/workflows/publish.yaml`, triggered on push to `main`. The workflow overrides `baseURL` at build time via `--baseURL`.

## Customizing the theme

The Academic theme ships through three Hugo modules: `blox-bootstrap/v5`, `blox-plugin-netlify`, `blox-plugin-reveal`. To override a layout, mirror the module's path under the top-level `layouts/` directory — Hugo's lookup picks the local file first. Don't edit files inside the module cache.

## License

Site content (text, figures, publications) © Jiaxuan Liu.
The underlying [HugoBlox Academic CV](https://github.com/HugoBlox/theme-academic-cv) theme is distributed under its own license — see [`LICENSE.md`](./LICENSE.md).
