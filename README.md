# Agnes Deglon Blog

This repository hosts the source for Agnes Deglon's GitHub Pages blog.

## Getting started

1. **Clone the repository**

   ```bash
   git clone https://github.com/adeglon/adeglon.github.io.git
   cd adeglon.github.io
   ```

2. **Edit the site**

   - Web pages live in the `web/` directory. Start by editing `web/index.html`.
   - Add additional pages or assets inside `web/` as the blog grows.

3. **Preview locally**

   To preview with the configured GitHub Pages theme:

   ```bash
   bundle install
   bundle exec jekyll serve
   ```

   Visit `http://localhost:4000` in your browser.

4. **Publish**

   Commit your changes and push to the `main` branch. GitHub Pages will rebuild the site automatically.

## Customization

- Site configuration lives in `_config.yml`. It currently uses the `minima` theme. Explore other [GitHub Pages themes](https://pages.github.com/themes/) by updating this file.
- Follow common best practices: include descriptive meta tags, optimize images, and keep external dependencies up to date.

## Directory structure

```text
/
├── _config.yml         # GitHub Pages configuration
├── README.md           # Project overview and instructions
└── web/                # Website pages
    └── index.html      # Landing page
```
