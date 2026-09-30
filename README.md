# kiarashk76.github.io

Personal academic website. It's built with Jekyll and served by GitHub Pages
(no build step: push to `master` and it goes live in about a minute).

## Where everything lives

| What you want to change | File |
|---|---|
| Name, email, links, location, photo, CV path | `_config.yml` (the `author:` block) |
| Bio and "Outside research" on the home page | `index.html` |
| News items on the home page | `_data/news.yml` |
| Publications | `_data/publications.yml` |
| Projects | `_data/projects.yml` |
| Teaching | `teaching.html` |
| CV page (short HTML version) | `cv.html` |
| CV PDF | `files/Kiarash_Aghakasiri_CV.pdf` (replace the file, keep the name) |
| Course reports and theses | `docs/` |
| Menu order | `_data/navigation.yml` |
| Colours and fonts | `assets/css/main.css` (tokens at the top) |
| Profile photo | `images/profile.jpg` (square, ~560px) |

## Add a publication

Add a block at the top of `_data/publications.yml`. Set `selected: true` to also show it on the home page.

## Add an idea

Copy `templates/idea.md` to `_ideas/<short-name>.md` and edit it.
`status` can be `seed`, `exploring`, `active` or `parked`.

## Write a blog post

Copy `templates/post.md` to `_posts/YYYY-MM-DD-short-title.md` and write it.

## Preview locally (optional)

```bash
bundle install
bundle exec jekyll serve   # then open http://localhost:4000
```
