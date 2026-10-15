---
title: Publish like nobody is watching
date: 2026-10-14
lede: My portfolio ships with one command now. The command was the easy part — the guardrails that make it safe to run without thinking are what I'd actually copy.
tags: [jekyll, github-pages, automation, tooling]
---

## The one command

From the project directory, `./publish.sh "what changed"` does three things.
It builds the site and refuses to continue if the build or the link check
breaks. It copies only the Jekyll files to the public repo — the Django app,
the database, and my working notes stay behind. Then it pushes, and GitHub
Pages rebuilds the site a minute or two later. That is the entire deploy.

## Why the gate matters more than the automation

Early in this project, both writing samples on this site were silently
missing from every build. Their dates sat one day in the future, and Jekyll
skips future-dated content by default. The build passed. The site looked
fine. Every link to those pages was broken, and nothing said a word until a
link checker went looking for them.

That bug is why `publish.sh` will not push a build that fails verification.
An automated pipeline without that kind of gate doesn't prevent broken
deploys. It schedules them, faster and with more confidence than the
situation deserves.

## What I actually wired up

- The publish path excludes everything that isn't the site. The public repo
  gets public content and nothing else.
- Commits carry GitHub's noreply address, because the account blocks pushes
  that expose a real email. I hit that wall before I read about it.
- SSH wasn't an option on this machine — its keys belong to other accounts —
  so pushes authenticate through the GitHub CLI's token instead. Whatever
  works. Nobody sees the plumbing.

## The rule I'd take to the next project

Automate the push only after the check exists. The check is the feature.
