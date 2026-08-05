<!-- org-project-routing:start -->
# Project routing

- **GitHub organization:** [drone-mngr](https://github.com/drone-mngr)
- **Canonical GitHub Project:** [drone-mngr-project](https://github.com/orgs/drone-mngr/projects/1) (project 1)
- **Canonical Linear project:** [planning workspace](https://linear.app/denman/project/githubcomdrone-mngr-8ac391ac308d)
- **Organization documentation repository:** [drone-mngr/.github](https://github.com/drone-mngr/.github)

## Source-of-truth boundaries

GitHub is authoritative for repositories, commits, pull requests, reviews, CI checks, releases, deployable artifacts, and runtime evidence. Linear is authoritative for product planning, priorities, ownership, dependencies, milestones, and status reporting. The GitHub Project is the organization-level execution board and should contain the governance issue maintained by this repository.

## Change and merge policy

Documentation branches must be reviewed through pull requests and merged after checks pass. Concurrent edits are reconciled semantically against the latest default branch: this managed routing block is regenerated while all unrelated prose outside the block is preserved. Do not resolve conflicts by blindly choosing one side.
<!-- org-project-routing:end -->

## Current safety-research execution item

The organization-level tracking item for the wildlife-observation research boundary is [`.github` issue #4](https://github.com/drone-mngr/.github/issues/4). It is intended for `drone-mngr-project` #1 and links the implementation evidence, Linear planning mirror, and urgent safety follow-up work.

### Delivered evidence

- [Merged control-plane PR #2](https://github.com/drone-mngr/drone-mngr-ctrl-server.rs/pull/2)
- [Simulation-only research design](https://github.com/drone-mngr/drone-mngr-ctrl-server.rs/blob/main/docs/research/animal-encounter-deterrence-simulation.md)
- [Linear planning mirror](https://linear.app/denman/document/wildlife-observation-and-manual-to-auto-tracking-research-boundary-e8d31a42550d)
- Linear issues `DEN-1858` and `DEN-1859`

### Scope boundary

This work is limited to human-supervised observation, explicit target nomination, safe autonomous observer handoff, standoff tracking, deterministic simulation, conservative abort behavior, and auditability. It excludes chemical-dispersal hardware, payload integration, physical actuation, autonomous use of force, wildlife contact, chasing, and harassment.

### Next project outcomes

1. Encode policy invariants and fail-closed validation tests.
2. Add deterministic target-handoff, identity-swap, person-entry, telemetry-loss, and geofence scenarios.
3. Add auditable event schemas and trace correlation.
4. Gate inert-target hardware-in-the-loop testing behind explicit local interlocks and approvals.
