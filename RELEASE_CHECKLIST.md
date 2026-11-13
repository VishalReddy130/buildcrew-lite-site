# BuildCrew Lite — release checklist

This is an internal release gate. A checkbox should only be marked complete after the result has been verified.

## 1. Source and installation
- [ ] Confirm the canonical CLI repository and default branch.
- [ ] Pin supported Python versions.
- [ ] Document installation from a clean environment.
- [ ] Document all commands, arguments, and expected outputs.
- [ ] Include a minimal example project plan.
- [ ] Include generated example handoffs for each supported role.
- [ ] Ensure no secrets, local paths, caches, or virtual environments are included.

## 2. Quality checks
- [ ] Run the full automated test suite.
- [ ] Test the documented commands from a clean checkout.
- [ ] Validate malformed plans, missing fields, duplicate task IDs, and unknown dependencies.
- [ ] Validate dependency blocking and ready-task selection.
- [ ] Validate handoff generation and output paths.
- [ ] Confirm errors are actionable and do not silently corrupt project plans.

## 3. Customer package
- [ ] Create a versioned ZIP containing source, license, README, examples, and changelog.
- [ ] Include a 5-minute quick-start path.
- [ ] Include troubleshooting and known limitations.
- [ ] Verify the ZIP extracts and works on a clean machine.
- [ ] Generate SHA-256 checksum and record package version.

## 4. Listing and delivery
- [ ] Finalize price and product description.
- [ ] Connect payment provider and configure automatic delivery.
- [ ] Test a complete purchase and download before announcing sales.
- [ ] Publish refund/support terms and a contact route.

## Product claims guardrail

Describe BuildCrew Lite as a local-first workflow kit. Do not describe it as an autonomous multi-agent system, a code executor, or a correctness guarantee. AI tools do the implementation; BuildCrew structures tasks and handoffs; a human remains responsible for review.
