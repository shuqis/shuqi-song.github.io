# Posting Guide

## 1. Create a new article file
Add a file under `_posts/` with this naming format:

`YYYY-MM-DD-short-title.md`

Example:

`_posts/2026-02-27-first-research-note.md`

## 2. Use this front matter
```yaml
---
layout: default
title: "Your Post Title"
date: 2026-02-27 10:00:00 -0500
categories: [research]
tags: [scRNA-seq, sepsis]
---
```

`categories` controls the first level in the article tree view.

## 3. Write content in Markdown
Use headings, bullet points, code blocks, and links as needed.

## 4. Commit and push
Once pushed to GitHub, Pages rebuilds the site and your post appears in:
- `/articles/`
- the "Latest posts" section on the homepage
