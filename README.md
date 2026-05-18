# Computational Imaging and Discovery Lab — Website

Source for the **CID Lab** site, built with [Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio) theme.

## Local development

```bash
bundle install
bundle exec jekyll serve --livereload
```

Then visit `http://localhost:4000`. A Docker setup is also available — see `INSTALL.md`.

## Content layout

- `_pages/about.md` — landing page (lab mission, themes, join us).
- `_pages/profiles.md` — people page. Add new members by replicating the profile block and creating a content file in `_pages/`.
- `_pages/publications.md` — auto-generated from `_bibliography/papers.bib`.
- `_pages/projects.md` — project cards rendered from `_projects/*.md`.
- `_news/*.md` — short news items shown on the landing page and `/news/`.
- `_data/socials.yml` — lab/PI social links.
- `_config.yml` — site title, description, navigation, scholar settings.

## Deploying

Standard Jekyll site — host on GitHub Pages, Netlify, or any static host. For GitHub Pages, set `url` and `baseurl` in `_config.yml` and follow the al-folio [deployment guide](https://github.com/alshedivat/al-folio#deployment).

## Credits

Theme by [al-folio](https://github.com/alshedivat/al-folio) (MIT). See `LICENSE`.
