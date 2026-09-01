# Agent workflow

Clone this repo per client. **`client.md`** is the single source of truth for project context — read it first, update it as you work.

## Before starting

- Read `client.md`

## While working

- Keep **Progress** in `client.md` current
- Record new facts in the relevant section (contacts, brand, preferences). Do not invent requirements.

## Stack

- Astro + TypeScript + Tailwind + MDX
- Pages live in `src/content/pages/`

## Content collections

Each page is a `.md` or `.mdx` file with YAML frontmatter at the top:

```yaml
---
title: Page title
description: Optional, for meta tags
draft: false
---
```

Astro validates frontmatter against the schema in `src/content/config.ts` and builds a route for each file at `/{filename}` (e.g. `example.mdx` → `/example`). To add a page, create a file — no routing code needed.

## Code

- Match existing patterns; keep diffs small
- Run `npm run build` before finishing

## Dev server

```
npm run dev
```
