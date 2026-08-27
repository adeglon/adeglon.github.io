# agnesdeglon.com

Source for Agnès Déglon's personal site and blog, published with GitHub Pages.

**Live:** <https://agnesdeglon.com> · <https://adeglon.github.io>

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
_config.yml   Jekyll configuration
CNAME         custom domain
Gemfile       github-pages, webrick
docs/         the published site — pages and assets live here
```

GitHub Pages builds from `docs/`. Pushing to `main` republishes the site, usually within a minute.

Build check before pushing:

```bash
bundle exec jekyll build --source docs
```

## Notes

- The `source: web` key in `_config.yml` is inert — GitHub Pages serves `docs/` regardless.
  `web/` holds an old placeholder page and is not published.
- Built with Jekyll and Materialize CSS.

## License

Site code is free to reuse. Written content and images are © Agnès Déglon, all rights reserved.
