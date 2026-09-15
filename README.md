# Blaze docs

Documentation site for Blaze, built with [Mintlify](https://mintlify.com).

## Local development

Requires Node.js 20 or later.

```bash
npm i -g mint   # install the CLI once
mint dev        # serve the site at http://localhost:3000
```

Run every command from this directory — the one that contains `docs.json`.

| Command | What it does |
| --- | --- |
| `mint dev` | Preview the site locally with hot reload |
| `mint broken-links` | Report internal links pointing at pages that do not exist |
| `mint validate` | Validate the whole build: config, pages, and OpenAPI spec |
| `mint update` | Update the CLI to the version production builds with |

## Repository layout

```
docs.json              Site configuration: theme, colors, navigation, navbar, footer
index.mdx              Landing page
quickstart.mdx         Getting started guide
development.mdx        Local preview and troubleshooting
essentials/            Writing guides: markdown, code, images, navigation, settings, snippets
ai-tools/              Editor setup for Claude Code, Cursor, and Windsurf
api-reference/         OpenAPI spec and the endpoint pages generated from it
snippets/              Reusable MDX imported into pages
images/, logo/         Static assets, referenced by absolute path
.github/workflows/     CI link checking
```

## Adding a page

1. Create the `.mdx` file with `title` and `description` frontmatter.
2. Add its path, without the extension, to a group under `navigation` in `docs.json`.
3. Check it in `mint dev`, then run `mint broken-links`.

A page that is not listed in `docs.json` never appears in the sidebar.

## Publishing

Install the [Mintlify GitHub App](https://dashboard.mintlify.com/settings/organization/github-app)
on this repository. Pull requests get a preview deployment, and merging to `main` deploys to
production.

## Before you customise

This repository ships as a template. Replace the following with your own content:

- `name`, `colors`, `logo`, and the GitHub/support links in `docs.json`
- `logo/light.svg`, `logo/dark.svg`, `favicon.svg`, and the hero images in `images/`
- `api-reference/openapi.json` — the sample Tasks API — and the endpoint pages that point at it
