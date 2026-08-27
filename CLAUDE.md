# CLAUDE.md — adeglon.github.io

Guidance for Claude working in this repository. **This repo is public** — nothing private,
personal, or unpublished goes in a committed file.

## What this is

Agnès Déglon's blog, hosted on GitHub Pages. It is the target of a migration off WordPress
(<https://agnesdeglonblog.com/>), so that the blog can be written and published directly from
files rather than through a WordPress admin.

- Live: <https://adeglon.github.io/>
- Custom domain: `agnesdeglon.com` (see `CNAME`)

## How it builds

- **GitHub Pages serves the `docs/` directory.** All site content and assets go in `docs/`.
- Jekyll via the `github-pages` gem, `minima` theme.
- Push to `main` → Pages rebuilds automatically, roughly a minute.

Preview locally:

```bash
bundle install
bundle exec jekyll serve --source docs    # http://localhost:4000
bundle exec jekyll build --source docs    # build check before pushing
```

## Repo quirks to know

- `_config.yml` contains `source: web`. It is stale — GitHub Pages ignores it and serves `docs/`.
  Do not "fix" this by moving content into `web/`.
- `web/index.html` is an abandoned Bootstrap "under construction" stub. It is not the live page.
- `AGENTS.md` and `codex.md` were written for a previous Codex setup. Where they disagree with this
  file, this file wins.

## Working agreements

- Commit directly to `main`. Do not create branches or PRs unless asked.
- Keep commits focused and descriptive.
- Run the build check above before pushing structural or config changes.
- Design: Material Design, fully responsive across devices. Current pages use Materialize CSS.
- Descriptive meta tags on every page; optimize images; keep external dependencies current.

## Writing for this site

Posts are in Agnès's voice, not assistant voice:

- Flowing, breathy, run-on, parenthetical sentences with a French cadence in English. Never choppy
  one-line sentences.
- Warm and funny about hard things; sarcasm is welcome, cynicism is not.
- Section headers open a curiosity gap rather than give away the joke.
- Family members stay anonymous — husband as "Dad" or "my husband", sons unnamed.
- No emoji in blog text.

## Open question — do not decide silently

The prototype and the WordPress site do not agree on identity:

| | Prototype (here) | WordPress (live) |
|---|---|---|
| Name | Messy Soul Soup | Agnès Déglon-Fischer |
| Tagline | A Mama-Hood and Menopause Survival Guide | Words from the trail, stories from the soul |
| Sections | Mama-Hood & Menopause · Family Misadventures · Feeding Healthy | Health & Science · Soul & Self · Mis-Adventures |

Which name, which sections, and which domain the migrated blog lands on are Agnès's decisions.
Ask before migrating content in bulk.
