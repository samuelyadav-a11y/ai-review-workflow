# ai-pr-review

Opinionated, cost-aware AI PR review workflows with incremental diffs, label gating, and schema-validated inline comments.

## Why
Large PRs are expensive to review and noisy to maintain. This project provides a battle-tested GitHub Actions workflow that:
- Reviews only **new changes** since the last review (incremental diff)
- Gates execution with a **label** to control cost
- Validates inline comment locations to avoid GitHub API errors
- Supports **custom rubrics** per repo/stack

## Quickstart
1. Copy the workflow template into your repo:
   - `templates/codex-pr-review.yml`
2. Copy the rubric and schema:
   - `templates/codex-review-guidelines.md`
   - `templates/codex-output-schema.json`
3. Add `OPENAI_API_KEY` to your repo secrets.
4. Add the `requires-review` label to a PR to trigger review.

## What’s Included
- GitHub Actions workflow with incremental diff + size guard
- Rubric template for high-signal reviews
- JSON schema to validate structured review output
- Docs on customization and cost control

## Repo Structure
- `templates/` : Workflow + rubric + schema to copy into your repo
- `docs/` : Setup, customization, and cost controls
- `examples/` : Example configs and outputs

## License
MIT
