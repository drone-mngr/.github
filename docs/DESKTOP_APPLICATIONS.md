# Desktop application allocation

Verified **2026-08-05**.

Drone Manager is a **strong candidate** for paired native desktop ground-control applications:

- Rust: [`drone-mngr/drone-mngr-desktop.rs`](https://github.com/drone-mngr/drone-mngr-desktop.rs) — **proposed**, not yet verified as a published repository.
- Flutter: [`drone-mngr/drone-mngr-flutter`](https://github.com/drone-mngr/drone-mngr-flutter) — **proposed**, not yet verified as a published repository.

These names are proposed allocation targets, not proof that either remote exists and not a claim that implementation is approved or complete. Promote the pair from proposed to planned only when scope, safety ownership, milestones, supported hardware, and repository creation are accepted in Linear.

## Product boundary

The pair should cover semantic parity for maps, live telemetry, mission planning, vehicle state, video, controller input, local recording, serial/radio/network connections, alerts, geofencing, pre-flight checks, emergency controls, reconnect and recovery, and audit logs.

A shared Rust telemetry and mission core may sit behind an explicit library, FFI, or service boundary, but the Flutter application remains independently buildable, testable, and releasable. Shared schemas, command/telemetry contracts, fixtures, simulator traces, mission files, safety-state models, and conformance tests should be versioned deliberately.

## Feature-delivery rule

Once planned, every desktop-facing change must inspect both implementations, define shared acceptance and safety criteria, update both or record an explicit no-change rationale, and report Rust and Flutter status separately. Hardware support and emergency-control behavior must be verified per platform and device.

## Project routing

- GitHub Project: [`drone-mngr-project` — Project 1](https://github.com/orgs/drone-mngr/projects/1)
- Linear project: `github.com/drone-mngr`
- Central registry: [`approved-private-registry`](private-registry://canonical/registry/desktop-applications.json)
- Portfolio rollout: [`DEN-2469`](https://linear.app/denman/issue/DEN-2469/roll-out-paired-rust-flutter-desktop-repositories-across-the-portfolio)

Promotion, repository creation, renames, transfers, archival, hardware-support changes, or platform-status changes must update this document, Linear, the central registry, and both companion repositories together.
