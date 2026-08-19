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
bun run build
```

## Structure

- [src/pages/index.astro](src/pages/index.astro) — page composition (the narrative order matters)
- [src/components/](src/components/) — one section per component
- [src/styles/global.css](src/styles/global.css) — Tailwind v4 theme tokens and shared component classes

OaaS is a fictional product. Any resemblance to your organization is emergent behavior.
