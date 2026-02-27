# Setup

## Requirements
- GitHub repository with Actions enabled
- `OPENAI_API_KEY` secret in repo settings

## Steps
1. Copy `templates/codex-pr-review.yml` into `.github/workflows/`.
2. Copy `templates/codex-review-guidelines.md` into `.github/`.
3. Copy `templates/codex-output-schema.json` into the repo root.
4. Add a `requires-review` label to your PR to trigger the workflow.

## Optional
- Adjust the diff size limit in the workflow.
- Customize the rubric to your stack and code standards.
