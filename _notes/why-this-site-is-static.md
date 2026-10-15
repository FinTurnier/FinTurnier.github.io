---
title: Why this site is static
date: 2026-10-15
lede: The reasoning behind moving the portfolio from a Django app to a static Jekyll site on GitHub Pages — and what stays in Django.
tags: [jekyll, github-pages, django, architecture]
---

## The decision

My first portfolio draft was a private Django project. Django is the right
tool when content is dynamic — user accounts, submissions, databases. A
portfolio is none of those things: it is content (projects, notes, lessons,
a timeline) rendered the same way for every visitor.

GitHub Pages serves static files only — no Python runtime. So the options
were:

1. **Static site on GitHub Pages** — free, fast, zero maintenance.
2. **Keep Django and host elsewhere** — free tiers sleep, spin down, and
   change terms; cold starts make a bad first impression on a portfolio.
3. **Hybrid** — static portfolio now, Django kept as a dev playground for
   genuinely dynamic projects deployed later and linked from here.

I chose the hybrid. Jekyll builds natively on GitHub Pages, and every piece
of content is plain Markdown with YAML front matter — portable to any future
stack.

## What stays in Django

The Django project remains my sandbox for things that genuinely need a server:
authentication experiments, database-backed demos, API work. When one of those
matures, it deploys separately (Render, Railway, or similar) and gets a link
from the [Projects](/projects/) page.

## The rule

> If every visitor sees the same bytes, the site should be static. Reach for
> a server only when the bytes differ per visitor or per action.
