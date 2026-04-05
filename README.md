# openclaw-workspace

Operational workspace for Pepper.

## Purpose

This repository is not a conventional application codebase.
It is the working memory, operating context, and execution workspace for Pepper.

It stores:
- agent instructions and operating rules
- user context
- long-term and daily memory
- local documentation
- helper scripts for operations and engineering tasks

## Core files

- `AGENTS.md` — workspace rules and operating behavior
- `SOUL.md` — assistant identity and behavioral principles
- `USER.md` — context about Michael
- `IDENTITY.md` — assistant identity details
- `MEMORY.md` — long-term memory
- `memory/` — daily notes
- `TOOLS.md` — local environment notes
- `HEARTBEAT.md` — heartbeat instructions

## Directories

- `docs/` — supporting documentation and reference material
- `scripts/` — helper scripts and automations
- `tmp/` — local scratch output, ignored by git

## Git hygiene

Ignored:
- `.openclaw/`
- `tmp/`
- local env files, logs, build artifacts, editor junk

Do not commit secrets, tokens, or machine-specific runtime state.
