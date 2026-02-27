# Customization

## Rubric
Edit `.github/codex-review-guidelines.md` to align with your standards.

## Label Gate
Change `requires-review` to any label you prefer in the workflow gate step.

## Incremental Reviews
By default, the workflow reviews only changes since the last Codex-reviewed commit.

## Cost Controls
- Reduce `MAX_BYTES` to limit diff size.
- Use label gating for expensive repos.
- Use `effort: low|medium|high` based on desired depth.
