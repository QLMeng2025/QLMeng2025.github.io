# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Site Overview

This is a personal academic website for Qinglin Meng (PhD Candidate in CS at Purdue University), built on the [Academic Pages](https://github.com/academicpages/academicpages.github.io) Jekyll template and hosted via GitHub Pages at https://QLMeng2025.github.io.

## Local Development

```bash
# Install dependencies (first time)
bundle install

# Serve locally with live reload
bundle exec jekyll serve -l -H localhost
# Site available at http://localhost:4000

# Using Docker instead
docker compose up
# Site available at http://localhost:4000
```

> `_config.yml` is **not** hot-reloaded — restart the server after changing it.

## Content Architecture

Content is separated from theme. Each content type lives in its own collection directory as Markdown files with YAML front matter:

| Directory | URL pattern | Key front matter fields |
|---|---|---|
| `_publications/` | `/publications/:path/` | `title`, `collection`, `category`, `permalink`, `date`, `venue`, `paperurl`, `citation` |
| `_talks/` | `/talks/:path/` | `title`, `collection`, `type`, `date`, `venue`, `location` |
| `_posts/` | `/:categories/:title/` | standard Jekyll post fields |
| `_teaching/` | `/teaching/:path/` | `title`, `collection` |
| `_portfolio/` | `/portfolio/:path/` | `title`, `collection` |
| `_pages/` | defined by `permalink` | page-specific |

Site-wide config is in `_config.yml`. Navigation menu is in `_data/navigation.yml`.

Static files (PDFs, slides) go in `files/` and are served at `/files/filename`.

## Adding Publications

Create a new `.md` file in `_publications/` with this front matter structure:

```yaml
---
title: "Paper Title"
collection: publications
category: conferences   # or: manuscripts, books
permalink: /publication/slug-or-external-url
excerpt: 'Short description'
date: 2025-06-01
venue: 'Conference or Journal Name'
paperurl: 'https://...'
citation: 'Author, A., & Author, B. (2025). Title. Venue.'
---
```

Alternatively, use `markdown_generator/` notebooks (`publications.ipynb`, `talks.ipynb`) to batch-generate Markdown from TSV spreadsheets.

## Key Files

- `_config.yml` — author profile, social links, site URL, plugins
- `_pages/about.md` — homepage content (permalink: `/`)
- `_pages/cv.md` — CV page
- `_data/navigation.yml` — top navigation menu items
- `assets/` — JS/CSS theme assets (rarely need editing)
- `_sass/` — SCSS theme styles
- `_includes/`, `_layouts/` — Liquid HTML templates
