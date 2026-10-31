# gaingod-xu.github.io

Hao Xu's personal academic site, built on [al-folio](https://github.com/alshedivat/al-folio) (Jekyll).

## Content

- `_pages/home.md` — homepage: vision (Trustworthy World Models for Life Science) with animated molecule-to-phenotype schematic, three questions, trustworthiness framework, building-the-world-model progression, selected research, domains, about, news
- `_pages/about.md` — short bio, appointments, education (`/pi/` redirects here)
- `_pages/research.md` — research directions with representative papers
- `_pages/publications.md` + `_bibliography/papers.bib` — full publication list, auto-grouped by year
- `_pages/cv.md` + `_data/cv.yml` — education, experience, awards, patents
- `_pages/people.md` — Team: student and faculty collaborators
- `_pages/teaching.md` — teaching experience
- `_data/socials.yml` — social/contact links

## Local development

Requires Ruby (see `.github/workflows/deploy.yml` for the pinned version) and Node.

```bash
bundle install
bundle exec jekyll serve
```

## Deployment

Pushes to `main` trigger `.github/workflows/deploy.yml`, which builds the site and
publishes it to the `gh-pages` branch. GitHub Pages (Settings → Pages) should be
set to deploy from that branch.
