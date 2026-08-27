# Agnès Déglon — Blog

Source for Agnès Déglon's GitHub Pages blog.

- **Live:** <https://adeglon.github.io/>
- **Custom domain:** <https://agnesdeglon.com/> (see `CNAME`)
- **Status:** prototype. The blog currently published to readers is the WordPress site at
  <https://agnesdeglonblog.com/>; this repo is where it is being migrated to.

## Getting started

```bash
git clone https://github.com/adeglon/adeglon.github.io.git
cd adeglon.github.io
bundle install
bundle exec jekyll serve --source docs   # preview at http://localhost:4000
```

## Editing the site

GitHub Pages builds from the **`docs/`** directory. Pages and assets go there.

```bash
bundle exec jekyll build --source docs   # build check
git add -A && git commit -m "..." && git push
```

Pushing to `main` republishes the site automatically, usually within a minute.

> **Note:** `_config.yml` contains a `source: web` line that is stale — Pages ignores it and serves
> `docs/`. `web/index.html` is an abandoned placeholder, not the live page.

## Directory structure

```text
/
├── _config.yml   # Jekyll config (minima theme)
├── CNAME         # custom domain
├── Gemfile       # github-pages + webrick
├── CLAUDE.md     # working guidance for Claude
├── AGENTS.md     # older guidance, written for Codex
├── docs/         # ← the published site
│   ├── index.html
│   ├── mama-hood-menopause.html
│   ├── family-misadventures.html
│   ├── feeding-healthy.html
│   └── when-menopause-and-puberty-collide.html
└── web/          # abandoned placeholder, not served
```

## Conventions

- Commit directly to `main`; no branches.
- This repository is public — no confidential or personally identifiable information.
- Material Design, responsive on every screen size.
- Descriptive meta tags, optimized images, current dependencies.
