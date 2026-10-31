# Validation, Evidence, and Known Limits

**Evidence snapshot: 31 October 2026.** This file reports what was visible in the connected development materials at the time of review. It is not a certification or production-readiness statement.

## Evidence reviewed

- A private development repository and its active self-development workstream.
- A Neuroplasma engineering note dated 30 October 2026.
- Home-node architecture and host-a-node participation rules.
- GitHub commit status information for the reviewed development snapshot.

The private repository name, branch names, implementation paths, and internal commit identifiers are intentionally not repeated in this public showcase.

## Test evidence recorded in project documentation

The Neuroplasma engineering note records:

- 49 tests for the Neuroplasma fabric;
- 13 guardian-policy tests;
- 1 end-to-end integration test through the consented Home Network test route;
- 63 focused tests passing together;
- 119 tests passing in a wider documented regression selection.

These are results recorded in the engineering note. They were not independently re-run against the reviewed snapshot as part of this investor-pack preparation. A dated, reproducible test run should be captured before formal technical diligence.

## Current GitHub status observed

For the reviewed development snapshot dated 31 October 2026, the GitHub status endpoint returned three Vercel contexts — web, test, and application — each with state `failure` and description **“Account is blocked.”** The check-runs endpoint returned zero check runs for that snapshot.

This is a deployment/account status failure, not evidence that the Neuroplasma unit tests failed. It nevertheless means the reviewed snapshot does not have a passing Vercel status. This public overview does not claim a verified current production deployment.

## Not yet demonstrated

- Physical fibre/transceiver transport or optical switching in an AiGhost installation.
- A physical Neuroplasma memory device or general-purpose optical RAM.
- Production key provisioning, key distribution, rotation, or recovery for Neuroplasma frames.
- A signed, fully automated public Windows/macOS node installer.
- Federated node peering between different AiGhost accounts.
- Guaranteed uptime, packet delivery, performance at scale, or independent security certification.
- A current production deployment verified from the reviewed development snapshot.

## Diligence checklist before commercial release

1. Re-run and archive the focused and full regression suites on a named commit.
2. Resolve the blocked Vercel account/status and record a fresh deployment result, if Vercel remains part of the deployment path.
3. Verify live product routes and payment flows separately; do not infer live readiness from code or tests.
4. Complete an independent security review, including key lifecycle, device revocation, and node consent.
5. Confirm the IP chain: authorship, contributor assignments, third-party licences, and any external assets.
6. Complete required terms, privacy notice, data-retention, support, and consumer-facing documentation before public pilot or paid launch.
7. For physical optical work, identify actual optical components and perform isolated laboratory measurements before publishing hardware claims.
