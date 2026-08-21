# xiaosunmacroeconomics.github.io

Source for [xiaosunmacroeconomics.github.io](https://xiaosunmacroeconomics.github.io) —
the academic homepage of Xiao Sun, PhD candidate in Economics at the London School of Economics.

Built with [Jekyll](https://jekyllrb.com) on the
[Academic Pages](https://github.com/academicpages/academicpages.github.io) template
(itself a fork of [Minimal Mistakes](https://mademistakes.com/work/minimal-mistakes-jekyll-theme/))
and served by GitHub Pages from the `master` branch.

## Where the content lives

| What | File |
| --- | --- |
| Homepage (bio, education) | `_pages/about.md` |
| Research page | `_pages/publications.md` |
| Teaching page | `_pages/teaching.md` |
| Top navigation | `_data/navigation.yml` |
| Name, bio, email, profile links | `_config.yml` (`author:` block) |
| Profile photo | `images/profile.jpg` |
| PDFs (papers, slides, CV) | `files/` — served at `/files/<name>.pdf` |
| Colours and typography | `_sass/theme/_custom_light.scss`, `_sass/theme/_custom_dark.scss`, `_sass/_site.scss` |

Editing any of these on GitHub is enough — GitHub Pages rebuilds the site automatically,
usually within a minute or two.

## Adding a profile link

The sidebar icons (Google Scholar, LinkedIn, GitHub, ORCID, …) appear automatically once the
matching field under `author:` in `_config.yml` is filled in. Leave a field blank to hide its icon.

## Running locally

Requires Ruby and Bundler.

```bash
bundle install
bundle exec jekyll serve --livereload
```

The site is then at <http://localhost:4000>. A `Dockerfile` and `docker-compose.yaml` are also
included if you would rather not install Ruby:

```bash
docker compose up
```

## Licence

Template code is MIT licensed (see `LICENSE`). Site content is © Xiao Sun.
