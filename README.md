# Charles Gao — Personal Portfolio

A static Jekyll site for `charlesgao721.github.io`. GitHub Pages can build it
directly from the `main` branch and repository root; no separate build workflow
is needed.

## Update the site

- Edit `index.md`, `about.md`, `work-experience.md`, or `contact.md` in the
  repository root. Keep the YAML front matter at the top of each page.
- Shared page structure is in `_layouts/`; the document head, navigation, and
  footer are in `_includes/`.
- Edit the visual styles in `assets/css/styles.css`. The favicon is
  `assets/favicon.svg`.
- Keep internal links on the `relative_url` filter so they continue to work if
  the site URL changes.
- Add only details you want published. Do not put private contact information in
  the site.

## Preview locally

Install Ruby 3.2 and Bundler, then from the repository root run:

```sh
bundle install
bundle exec jekyll serve
```

Open the local URL printed by Jekyll (normally `http://127.0.0.1:4000`). Jekyll
regenerates the site when you save a file.

## Publish on GitHub Pages

In the repository's Pages settings, choose **Deploy from a branch**, select
`main`, and select `/(root)`. Keep `_config.yml`'s `url` set to
`https://charlesgao721.github.io` and `baseurl` empty. GitHub Pages runs the
Jekyll build when changes are pushed; do not commit `_site/`.

## Run Lighthouse

1. Preview the site locally or open the published site in Chrome.
2. Open Chrome DevTools, choose **Lighthouse**, and select Performance,
   Accessibility, Best Practices, and SEO.
3. Run the report for both mobile and desktop. Review any reported issue and
   rerun Lighthouse after changes.

The site avoids remote fonts, images, scripts, and tracking so the document stays
small and quick to load.
