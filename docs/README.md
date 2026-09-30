# Centaur documentation

This directory contains the Centaur documentation.

The source files are Markdown and MDX files under `docs/pages/`. The site build is a presentation layer. Keep the content portable so it can move to another host later.

## Read the docs in GitHub

Start with these pages:

- [`what-is-centaur.mdx`](pages/what-is-centaur.mdx): product overview
- [`quickstart.mdx`](pages/quickstart.mdx): local setup
- [`architecture.mdx`](pages/architecture.mdx): system design
- [`deploying-in-production.mdx`](pages/deploying-in-production.mdx): production deployment
- [`security.mdx`](pages/security.mdx): security model

GitHub can review these files while the repository is private. No public website or domain is required.

## Preview locally

Run the existing Vocs preview from this directory:

```bash
npm ci
npm run dev
```

Open the local URL printed by Vocs. Stop the server with `Ctrl-C`.

## Keep content portable

- Write content in Markdown or MDX.
- Use relative links for pages in this directory.
- Keep images in `docs/public/`.
- Do not put secrets in docs or examples.
- Treat `docs/public/md/` as generated output. Edit the files under `docs/pages/` instead.

## Later hosting options

When the repository is ready, the same source can move to a public documentation site. Possible targets include Cloudflare Workers Static Assets, GitHub Pages, or another static host. The content does not need to change for that migration.
