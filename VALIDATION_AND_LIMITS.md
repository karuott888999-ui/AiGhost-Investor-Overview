# Validation, Evidence, and Known Limits

**Evidence snapshot: 2026-10-31.** This file reports what was visible in the connected GitHub repository at the time of review. It is not a certification or production-readiness statement.

## Repository evidence

- Repository: `karuott888999-ui/Ghost` — private.
- Reviewed development branch: `feat/ghost-home-node-self-dev`.
- Reviewed commit: `f82532cc47c3ad620cd2b36202940f1507dcbbd1`.
- Neuroplasma engineering note: `backend/NEUROPLASMA_OPTICAL_FABRIC.md`, dated 2026-10-30.
- Home-node architecture and participation policy: `docs/GHOST_HOME_NODE_AND_SELF_DEV.md` and `docs/HOST_A_NODE_RULES.md`.

## Test evidence recorded in project documentation

The Neuroplasma engineering note records:

- 49 tests for the Neuroplasma fabric;
- 13 guardian-policy tests;
- 1 end-to-end integration test through the consented Home Network test route;
- 63 focused tests passing together;
- 119 tests passing in a wider documented regression selection.

These are results recorded in the project note. They were not independently re-run against the latest reviewed commit as part of this investor-pack preparation. A dated, reproducible test run should be captured before formal technical diligence.

## Current GitHub status observed

For commit `f82532cc47c3ad620cd2b36202940f1507dcbbd1`, the GitHub status endpoint returned three Vercel contexts — `aighost-test`, `aighost-web`, and `ghost` — each with state `failure` and description **“Account is blocked.”** The check-runs endpoint returned zero check runs for this commit.

This is a deployment/account status failure, not evidence that the Neuroplasma unit tests failed. It nevertheless means this commit does not have a passing Vercel status and this overview does not claim a verified current production deployment.

## Not yet demonstrated

- Physical fibre/transceiver transport or optical switching in an AiGhost installation.
- A physical Neuroplasma memory device or general-purpose optical RAM.
- Production key provisioning, key distribution, rotation, or recovery for Neuroplasma frames.
- A signed, fully automated public Windows/macOS node installer.
- Federated node peering between different AiGhost accounts.
- Guaranteed uptime, packet delivery, performance at scale, or independent security certification.
- A current production deployment verified from the latest commit.

## Diligence checklist before commercial release

1. Re-run and archive the focused and full regression suites on a named commit.
2. Resolve the blocked Vercel account/status and record a fresh deployment result, if Vercel remains part of the deployment path.
3. Verify live product routes and payment flows separately; do not infer live readiness from code or tests.
4. Complete an independent security review, including key lifecycle, device revocation, and node consent.
5. Confirm the IP chain: authorship, contributor assignments, third-party licences, and any external assets.
6. Complete required terms, privacy notice, data-retention, support, and consumer-facing documentation before public pilot or paid launch.
7. For physical optical work, identify actual optical components and perform isolated laboratory measurements before publishing hardware claims.
