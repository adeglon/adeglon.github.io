# Codex

This repository contains the source for Agnes Deglon's public website.

- **Primary URL:** <https://adeglon.github.io/>
- **Custom domain:** <https://agnesdeglon.com/> (configured via `CNAME`).
- **Content root:** GitHub Pages serves files from the `docs/` directory.
- **Repository visibility:** Public. Avoid committing confidential or personally identifiable information.

## Development notes
- Pages and assets should live under `docs/`.
- To preview locally:
  ```bash
  bundle install
  bundle exec jekyll serve --source docs
  ```
- Commit changes directly to the `main` branch; GitHub Pages will rebuild automatically.

