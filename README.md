# kiarashk76.github.io

To update the website, edit a file in the **`_data`** folder, then commit and push.
GitHub rebuilds the site about a minute later. You never need to touch the HTML.

## Which file controls which page

| Page | File to edit |
|---|---|
| Sidebar on every page (name, photo, university, location, email, links) | `_data/profile.yml` |
| About (home): headline, bio, interests, news, outside research | `_data/home.yml` |
| Publications | `_data/publications.yml` |
| Projects | `_data/projects.yml` |
| Teaching | `_data/teaching.yml` |
| CV page (short version) | `_data/cv.yml` |
| Ideas page intro | `_data/ideas.yml` |
| Blog page intro | `_data/blog.yml` |
| Top menu | `_data/menu.yml` |

Other files you might replace:

- **CV PDF:** `files/Kiarash_Aghakasiri_CV.pdf` (keep the same name)
- **Photo:** `images/profile.jpg` (square)
- **Reports and theses linked from Projects:** `docs/`

### Tips for the `.yml` files

- Keep the indentation (spaces, not tabs). Copy an existing block when adding one.
- Wrap text in quotes if it contains a colon, for example `title: "ScoreNet: Netting ..."`.
- Text fields accept Markdown: `**bold**`, `*italic*` and `[link text](https://...)`.
- If the site stops updating after a push, open the repo's **Actions** tab on GitHub.
  The failed run usually names the file and line with the mistake.

## Add an idea

Create a file in `_ideas/`, for example `_ideas/plasticity-and-task-change.md`
(the file name becomes the URL):

```markdown
---
title: "Does the size of a task change drive loss of plasticity?"
date: 2026-10-01
status: seed        # seed | exploring | active | parked
summary: One or two sentences on the question and why it matters.
tags: [continual learning, plasticity]
---

Write anything here in Markdown: the question, why it matters, what you'd try first, related work.
```

## Write a blog post

Create `_posts/YYYY-MM-DD-short-title.md`, for example `_posts/2026-10-15-why-options.md`:

```markdown
---
title: "Why options?"
subtitle: Optional one-line summary shown in the post list
tags: [reinforcement learning]
---

The first paragraph becomes the preview on the Blog page.
```

Put images in `images/` and use `![description](/images/file.png)`.

## Design files (only if you want to change the look)

`_layouts/`, `_includes/`, `assets/css/main.css` (colours are at the top), `assets/js/main.js`.
