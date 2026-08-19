# Ownership-as-a-Service™

> The work always finds an owner.

A satirical enterprise SaaS landing page for **OaaS™** — ownership infrastructure that
guarantees every task, decision, follow-up, and loose end has an owner. It achieves this
by observing who historically notices, follows up, retains context, and prevents failure…
and routing everything to that person.

The system works. That is the problem.

Static site built with [Astro](https://astro.build) and [Tailwind CSS](https://tailwindcss.com).

## Development

```sh
bun install
bun run dev      # or: astro dev --background
bun run check    # typecheck
bun run build
```

## Deployment

The site deploys to GitHub Pages at
`https://gabroberge.github.io/ownership-as-a-service/` via
[.github/workflows/deploy.yml](.github/workflows/deploy.yml) on every push to
`master` (build → typecheck → upload → deploy, no branch artifacts). `site` and
`base` are set in [astro.config.mjs](astro.config.mjs), so all asset and
social-preview URLs resolve correctly under the project subpath.

One-time repository setup (Pages via workflow, Dependabot, secret scanning,
action allowlist, branch protection) is scripted in
[scripts/github-setup.sh](scripts/github-setup.sh):

```sh
gh auth login
./scripts/github-setup.sh
```

## Structure

- [src/pages/index.astro](src/pages/index.astro) — page composition (the narrative order matters)
- [src/components/](src/components/) — one section per component
- [src/styles/global.css](src/styles/global.css) — Tailwind v4 theme tokens and shared component classes

OaaS is a fictional product. Any resemblance to your organization is emergent behavior.
