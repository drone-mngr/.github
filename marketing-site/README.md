# Drone Manager marketing site

Complete Astro source staged for the future public repository `drone-mngr/drone-mngr.github.io` and URL `https://drone-mngr.github.io/`.

## Canonical planning

- Linear project: [github.com/drone-mngr](https://linear.app/denman/project/githubcomdrone-mngr-4e11d2ca1339)
- GitHub Project: [drone-mngr-project #1](https://github.com/orgs/drone-mngr/projects/1)
- Organization: [drone-mngr](https://github.com/drone-mngr)

## Product context

Drone Manager is being organized as a fleet and airspace control platform with explicit mission, command, telemetry, safety, and audit boundaries. The marketing page emphasizes bounded commands, operator review, geofencing/airspace policy, durable mission state, and observable fleet health.

There is not yet a public `drone-mngr-clients` repository. The TypeScript, Rust, curl, and mission-document examples are therefore labeled as an **API preview** rather than released SDKs. Endpoint and payload shapes must be reconciled with the final public interface repository before production publication.

## Publish

1. Create public repository `drone-mngr.github.io` in the `drone-mngr` organization.
2. Copy this directory to its repository root.
3. Run `npm install && npm run build`.
4. Add the standard Astro GitHub Pages workflow and enable GitHub Actions as the Pages source.
5. Verify `https://drone-mngr.github.io/` and update the linked GitHub and Linear tickets.
