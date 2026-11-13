# BuildCrew Lite — product website

This repository contains the public BuildCrew Lite landing page, interactive browser demo, and a small free sample.

## Live site

https://vishalreddy130.github.io/buildcrew-lite-site/

## What is available today

- Static landing page with an interactive handoff demo.
- A fictional inventory project plan in `sample/sample_project_plan.json`.
- A sample task handoff in `sample/EXAMPLE_HANDOFF.md`.
- A short explanation of the sample and product limitations in `sample/README.md`.

The browser demo uses illustrative sample data. It is a product preview, not a hosted BuildCrew application.

## Product scope

BuildCrew Lite is intended to be a local-first workflow kit for coordinating AI-assisted software work. Its intended workflow includes task planning, dependency-aware task selection, role-specific briefs, Markdown handoffs, and human review.

It is **not** an autonomous agent runtime. It does not independently execute code, call an LLM, include model/API credits, or guarantee the correctness of AI-generated code.

## Local preview

Open `index.html` in a browser. The site is static and has no build step.

## Deployment

GitHub Actions deploys the site to GitHub Pages when changes are pushed to `main`.

## Release readiness

The paid downloadable package and checkout are not published yet. Before a paid release, the actual CLI source must be connected to this repository or its release pipeline, packaged with installation instructions and examples, and verified from a clean installation. Do not treat the website demo or the free sample files as the paid product.
