# drone-mngr organization handbook

> Shared operating defaults for repositories maintained under **drone-mngr**. Repository-local policy may strengthen these rules but should not silently weaken them.

## Mission and safety boundary

drone-mngr maintains lawful drone fleet, mission, telemetry, simulation, maintenance, and operational-management software. This `.github` repository is the canonical home for shared policy, reusable templates, community health files, and planning links.

Organization software must not be designed or configured to weaponize aircraft, deploy chemical irritants, autonomously target people or animals, harass wildlife, defeat safety controls, or facilitate unlawful surveillance. Research and testing must use safe simulations, inert payloads, controlled environments, documented authorization, and human oversight.

## Repository contract

Each active repository must document purpose, ownership, maturity, supported aircraft and environments, development and test commands, authoritative command and telemetry formats, release and rollback procedures, compatibility policy, and GitHub Project/Linear links. Flight components should also document geofencing, arming and authority, manual override, loss-of-link behavior, return-to-home, failsafes, battery and weather limits, observability, privacy, and incident response.

## Change workflow

1. Anchor work in an issue, Linear item, or documented maintenance objective.
2. Keep branches and pull requests focused.
3. Explain motivation, scope, physical and legal risk, validation, compatibility, migration, and rollback.
4. Test simulations first, including stale telemetry, denied authority, geofence, low battery, sensor failure, lost link, emergency stop, and recovery paths.
5. Require explicit human approval before any real-world flight or actuation test.
6. Resolve conflicts semantically and prefer squash merges for focused work.

## Evidence, security, and documentation

Pull requests should include reproducible simulation commands, synthetic telemetry, expected and observed failsafe behavior, negative-path coverage, documentation updates, and CI or local-equivalent evidence. Never commit credentials, private keys, restricted flight data, personal imagery, or sensitive logs. Follow `SECURITY.md` for private reporting. Keep authority, safety, privacy, hardware, regulatory, and operational boundaries explicit.

## Planning ownership

GitHub owns code, reviews, checks, releases, and delivery evidence. Linear owns priority, dependencies, sequencing, and cross-project planning. The organization GitHub Project is the cross-repository execution view; see `PROJECTS.md` for routing details.

## Organization health

- [ ] Profiles, descriptions, topics, and READMEs are current.
- [ ] Community health files and reusable issue/PR guidance are present.
- [ ] Authority, geofencing, override, failsafes, privacy, and incident response are documented.
- [ ] Required checks cover simulation, denied/stale commands, lost link, emergency stop, compatibility, and supply-chain risk.
- [ ] Unsafe weaponization, targeting, harassment, or unauthorized-surveillance functionality is prohibited.
- [ ] GitHub Project and Linear links resolve and reflect completed work.
