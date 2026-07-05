# your notes site

A minimal Jekyll site styled like a commit log — each note is an entry on a timeline, with its own hash and date. No build tools to install; GitHub builds it for you.

## Put it online (~5 minutes)

1. Create a new repo on GitHub. If you name it `YOUR_USERNAME.github.io`, your site lives at `https://YOUR_USERNAME.github.io`. Any other name works too — it'll live at `https://YOUR_USERNAME.github.io/REPO_NAME`.
2. Push these files to it:
   ```
   git init
   git add .
   git commit -m "first commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```
3. On GitHub: go to the repo's **Settings → Pages**, and under "Build and deployment" set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
4. Wait a minute or two, then visit the URL from step 1.

## Before you push

- In `_config.yml`, change `author` to your name, and `title`/`description` if you want something other than "notes".

## Writing a new entry

Add a file to `_posts/` named `YYYY-MM-DD-a-short-title.md`:

```markdown
---
layout: post
title: "whatever you're calling it"
tags: [optional, tags]
---

Write in plain markdown. Code blocks, links, and images all work normally.
```

It'll appear on the homepage automatically, newest first. Delete the example post (`_posts/2026-07-05-hello-log.md`) whenever you want.

## Editing the design

Everything visual lives in `assets/css/style.css` — colors and fonts are defined as CSS variables at the top of the file if you want to adjust the palette later.
