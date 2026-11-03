# Personal website

A simple personal site (About, Research, Blog) built with
[Jekyll](https://jekyllrb.com/), which GitHub Pages builds automatically.
No build tools are needed. Edit the files and push.

## Where things are

| What you want to change       | File                                   |
|-------------------------------|----------------------------------------|
| Name, tagline, footer links   | `_config.yml`                          |
| Bio and research (home page)  | `index.md`                             |
| Blog posts                    | `_posts/YYYY-MM-DD-title.md`           |
| Colors, fonts, spacing        | `assets/style.css`                     |
| Page layout (header/footer)   | `_layouts/default.html`                |

## Add a blog post

Create a new file in `_posts/` named like `2026-11-02-my-idea.md`:

```markdown
---
layout: post
title: My idea
---

Write the post here in Markdown.
```

## Add a paper

1. Put the PDF in `papers/`.
2. In `index.md` (Research section), copy a `<div class="paper">` block and edit the title,
   authors, abstract and PDF link.

## Publishing with GitHub Pages

1. The repo must be **public** (or you need GitHub Pro for Pages on a private repo).
2. Go to **Settings → Pages** and set the source to **Deploy from a branch**,
   branch `main`, folder `/ (root)`.
3. If the repo is named `<username>.github.io`, the site is at
   `https://<username>.github.io`. Otherwise, set `baseurl` in `_config.yml`
   to `"/<repo-name>"`.

## Preview locally (optional)

```bash
gem install bundler jekyll
jekyll serve
```
Then open http://localhost:4000.
