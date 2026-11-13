# BuildCrew Lite — release checklist

This is an internal release gate. A checkbox should only be marked complete after the result has been verified.

## 1. Source and installation

- [x] Confirm the canonical CLI repository and default branch (`main` in the separate source repository).
- [x] Define the supported Python range: 3.10 or later; CI currently covers Python 3.10–3.14 on Windows and Linux.
- [x] Document first-run setup in `START_HERE.md` and verify the extracted package in a fresh workspace.
- [x] Document the command set and primary usage paths in `README.md`, `START_HERE.md` and `docs/QUICK_DEMO.md`.
- [x] Include a minimal example project plan.
- [x] Include six CLI-generated example handoffs, one for each supported role, under `examples/handoffs/`.
- [x] Use an explicit package allowlist and verify the archive contains no secrets, local workspace files, interpreter caches or virtual environments.

## 2. Quality checks

- [x] Run the full automated test suite (22 tests).
- [x] Exercise the first-run and documented CLI workflow from an extracted package: doctor, init, check, report, next, handoff, start and accept.
- [x] Validate malformed plans, invalid fields, duplicate task IDs and unknown dependencies.
- [x] Validate dependency blocking and ready-task selection.
- [x] Validate handoff generation and output paths.
- [x] Verify dashboard behavior, error handling and human-acceptance gates through automated tests and a local dashboard smoke test.

## 3. Customer package

- [x] Create a versioned ZIP containing the helper, role briefs, instructions, license, README, examples, templates, tests and changelog.
- [x] Include a five-minute first-run guide.
- [x] Include troubleshooting and known limitations in the FAQ, compatibility and product-scope documentation.
- [x] Verify the staged package and extracted ZIP; run checks across Windows/Linux CI environments.
- [x] Generate and verify a SHA-256 sidecar for version 0.3.0.

## 4. Listing and delivery

- [ ] Finalize the price and product description. The current ₹299 figure is still marked as a proposed founding price.
- [ ] Connect a payment provider and configure automatic delivery.
- [ ] Test a complete purchase and download before announcing sales.
- [ ] Publish refund/support terms and a contact route.

## Product claims guardrail

Describe BuildCrew Lite as a local-first workflow kit. Do not describe it as an autonomous multi-agent system, a code executor, or a correctness guarantee. AI tools do the implementation; BuildCrew structures tasks and handoffs; a human remains responsible for review.

## Current status

The v0.3.0 package, six role-specific example handoffs and core first-run workflow are technically verified. Commercial delivery remains open. No checkout or payment integration is included in this release-readiness pass.
