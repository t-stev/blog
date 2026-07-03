# Blog

A [Hugo](https://gohugo.io) blog, deployed to GitHub Pages automatically on
every push to `main`.

## Writing a post

Add a Markdown file to `content/posts/`:

```markdown
---
title: My post title
date: 2026-07-03
---

Post body in Markdown.
```

Commit and push. GitHub Actions rebuilds and deploys the site.

## Local preview

Requires Hugo (`brew install hugo`), then:

```sh
hugo server
```

and open http://localhost:1313.

## One-time GitHub setup

1. Create a repo and push this directory to it.
2. In the repo settings on GitHub: **Settings → Pages → Build and
   deployment → Source: GitHub Actions**.
3. Push to `main` (or re-run the workflow). The site appears at
   `https://<username>.github.io/<repo>/`.
