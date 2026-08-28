# adeglon.github.io

Source for Agnès Déglon-Fischer's website: her essays, and the home of *The Within Trilogy*.

**Live:** <https://adeglon.github.io>

Agnès is a Swiss-American writer and translator in Southern California, writing about
motherhood, midlife, health and the mess in between.

## Running the site locally

```bash
git clone https://github.com/adeglon/adeglon.github.io.git
cd adeglon.github.io
bundle install
bundle exec jekyll serve --source docs
```

The preview runs at <http://localhost:4000>.

## Structure

```text
Gemfile      github-pages, webrick
docs/        the published site — everything lives here
  _config.yml    site configuration, navigation, sections
  _data/         the books
  _layouts/      default, page, post, section, book
  _includes/     header, nav, footer, ornament, and friends
  _posts/        the essays
  assets/css/    tokens, base, components
```

GitHub Pages builds from **`docs/`**, so `docs/_config.yml` is the configuration that matters.
Pushing to `main` republishes the site, usually within a minute.

Build check before pushing anything structural:

```bash
bundle exec jekyll build --source docs
```

## Design

No CSS framework. The stylesheets are a small design system derived from the approved cover
artwork: two Garamonds, a palette sampled from the comp, and a single ornament. Components use
semantic tokens (`--accent`, `--text`) rather than palette names, which is what lets one
stylesheet serve the light reading pages and the dark trilogy pages from the same file.

Pages choose their ground in front matter — `ground: dark` — and default to `auto`, which follows
the reader's system setting.

## License

Site code is free to reuse. Written content and images are © Agnès Déglon-Fischer,
all rights reserved.
