# Fix Bug Prompt

Use this prompt when asking the agent to investigate and fix a bug.

## Prompt

Investigate the following bug:

{bug-description}

Relevant files or feature area:

{files-or-feature-area}

Follow:

- `AGENTS.md`
- The related requirement file under `docs/requirements/`
- The related architecture file under `docs/architecture/`

Expected output:

- Root cause analysis.
- Proposed fix.
- Files expected to change.
- Validation steps after the fix.
