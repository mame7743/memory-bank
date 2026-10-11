# Memory Bank

A small, Git-tracked project-memory skill for coding agents.

It keeps durable project context in Markdown so a later session, a different
agent, or a different machine can resume work without reconstructing decisions
from chat history.

## What it manages

- `AGENTS.md`: durable project instructions and the entry point to memory
- `docs/memory/README.md`: memory index and current state
- `docs/memory/YYYY-MM-DD-<slug>.md`: one dated record per decision, finding,
  handoff, or investigation

## Principles

- Treat repository files as the source of truth; do not rely on chat history.
- Read the project instructions and memory index before resuming work.
- Record meaningful decisions with context and status (`draft`, `decided`, or
  `superseded`), then link replacements rather than overwriting history.
- Keep entries short, factual, and free of secrets, passwords, tokens, private
  keys, and unnecessary personal data.
- Ask before initializing or materially changing a project's memory structure.

## Install

Install it in a host agent's skills directory, or use a skill manager that
supports a repository containing `SKILL.md`. The included templates initialize
a minimal `AGENTS.md` and `docs/memory/` structure in a project.

## License

MIT. See [LICENSE](LICENSE).
