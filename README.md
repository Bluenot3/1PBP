# One Page Business Plan — ZEN Proposal

The complete interactive proposal site prepared by ZEN for The One Page Business Plan Company.

This portable React, TypeScript, and Vite edition preserves the published proposal's page components, content, styles, and assets. It includes **18 opportunities**, **six interactive solution walkthroughs**, the capacity calculator, opportunity map, rollout, source references, and the corrected ZEN logo. The hosting entry point has been adapted from ChatGPT Sites; the proposal content has not been rewritten for this export.

## Run and build

Use Node.js 22.13 or newer and pnpm 11.25.0.

```sh
pnpm install --frozen-lockfile
pnpm dev
```

```sh
pnpm typecheck
pnpm build
pnpm preview
```

The deployable static website is generated in `dist/`. No API keys, database, authentication service, or environment variables are required. The demos are illustrative browser interactions, not connected production integrations.

## What is included

| Path | Purpose |
| --- | --- |
| `app/page.tsx` | Complete proposal page and interactive calculator |
| `app/proposal-data.ts` | All 18 opportunities and source references |
| `app/opportunity-assessment.ts` | Business fit, alternatives, investment gates, and overlapping scopes |
| `app/proposal-sections.tsx` | Business context, demonstrations, tools, growth, and sources |
| `app/proposal-visuals.tsx` | Opportunity map, animated walkthroughs, and capacity illustration |
| `app/globals.css`, `app/executive-polish.css` | Layout, responsive styling, and visual polish |
| `public/` | Logos, hero artwork, favicon, and existing downloadable proposal PDF |
| `src/main.tsx`, `index.html`, `vite.config.ts` | Standalone application entry and build configuration |

The existing `public/automation-proposal.pdf` covers opportunities 01–06. The website contains the full set of 18 opportunities. The PDF is not the separate proposal packet being prepared elsewhere.

## Deployment and domain

For a static host connected to this repository, use:

- Install: `pnpm install --frozen-lockfile`
- Build: `pnpm build`
- Publish directory: `dist`

The intended address is `onepagebusinessplan.zenai.world`. Uploading this repository does **not** publish that domain. First deploy on the chosen host, then use that host's exact DNS and verification instructions. The prior ChatGPT Sites DNS records are not interchangeable with a new host's records.

The existing published site is https://zen-onepage-next.zenagi.chatgpt.site.

## Lovable handoff

As checked on September 27, 2026, [Lovable's official GitHub documentation](https://docs.lovable.dev/integrations/github) says existing GitHub repositories cannot be imported directly: connecting a Lovable project creates a new repository.

If you choose Lovable, create a project there and connect its GitHub integration. Moving this site into the repository created by Lovable is a separate migration step; this repository is not automatically connected to a Lovable project. Keep the Lovable project's required configuration, review the migrated application, and verify its build and preview before publishing. After publication, add the custom domain using Lovable's own instructions.

This export uses standard client-side React/Vite to simplify that migration, but a Lovable preview or deployment has not been tested.

## Content and provenance

- Exported from published source commit `d579bcddb876458a11095254f0e9226064355681`.
- The 18 items are assessed opportunities, not 18 proven or independently costed implementation commitments.
- Preserve sample labels, assumptions, sources, and approval gates when editing the proposal.
- The calculator is an illustrative model, not measured client performance or guaranteed financial return.
- The page requests `noindex, nofollow`; this is an indexing preference, not access control.
- Application components, styles, and public assets were copied byte-for-byte from the published source. The host-specific runtime and unused starter examples are excluded.

Validation: TypeScript and the production Vite build are checked during export. Dependency versions are preserved from the source lockfile. A clean dependency installation and visual QA in Lovable remain deployment checks.
