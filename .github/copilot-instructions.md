## Repo purpose

This repository holds a single, curated GitHub profile README: `README.md`.
Primary goal: keep the profile content up-to-date (bio, skills badges, featured projects, contact links and external GitHub stats widgets).

## What an AI agent should know up front

- The repo is a single Markdown-driven presentation (no build, no tests). Changes are limited to `README.md` and optionally small image assets.
- Visual layout is achieved using a mix of Markdown and inline HTML blocks (e.g. `<div align="center">`). Preserve these wrappers when editing alignment or sections.
- Skill badges and stats are 3rd-party image embeds (shields.io, github-readme-stats, github-readme-streak-stats). Keep those as image URLs — do not embed large binary assets into the repo.

## Common edit patterns / examples

- Add or update a featured project by following the existing pattern:

  ### 🔗 [ProjectName](https://github.com/owner/repo)
  **Short one-line summary**  
  *Stack: TypeScript, Playwright, PostgreSQL*  

- Add a skill badge using shields.io (follow existing badge style):

  ![Tool](https://img.shields.io/badge/Tool-Color?style=flat&logo=tool&logoColor=white)

- Keep horizontal rules `---` between major sections — they're used for visual separation.

## External integrations to be aware of

- GitHub README widgets used here:
  - `https://github-readme-stats.vercel.app/api?...` (GitHub stats and Top Languages)
  - `https://github-readme-streak-stats.herokuapp.com/...` (streak badge)

  These are dynamic image endpoints; editing the README only changes what GitHub renders — there is no local generation step.

## Conventions & small rules

- Preserve emojis and section headings used for visual scanning (e.g., `## 🚀 Featured Projects`).
- When linking to a project, prefer the full GitHub repo URL. Keep the bold title + single-line description + `*Stack: ...*` convention.
- Avoid adding large binary files (images, PDFs). If an image is required, prefer hosting it via a CDN or in a small `assets/` folder and reference it by relative path.

## No build / testing steps

- There is no build, test, or CI configuration present in this repository. Changes are validated visually via the GitHub web UI after a PR is opened.

## Helpful next steps for a contributor or automated agent

- If adding a new badge or widget, verify the URL and parameters in a local Markdown preview or in a draft PR.  
- For PR descriptions, include a short note about what changed (e.g., "Add Playwright Mark to featured projects and update skills badges").

## Files to inspect when making changes

- `README.md` — primary file to edit.  

If anything here is unclear or you'd like me to include additional automation instructions (PR templates, spellcheck, or badge parameter conventions), tell me what to add and I will update this file.
