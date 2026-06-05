# AFD-OS v2.1 — AI First Development Operating System

> **Codex Skill**: Six-phase document-driven development methodology with architecture-first governance.

## What is AFD-OS?

AFD-OS v2.1 is a structured development protocol that turns an AI coding agent into a Chief Architect & Project Arbiter. It forces all decisions onto the filesystem — AI works against documents, code is merely the executable artifact.

## Six Phases

| Phase | Output | Description |
|-------|--------|-------------|
| **0** | Product Matrix | Mandatory requirement simplification via 5-dimension matrix |
| **X** | Non-template handling | Fallback for requests outside the matrix |
| **1** | docs/business_breakdown.md | Business goals, actors, user flows, MVP scope |
| **1.5** | docs/prd.md | Prioritized features, user stories, flows |
| **2** | docs/system_design.md | Single tech stack, data model, API contracts, dir structure |
| **2.5** | docs/adr/ADR-XXX.md | Architecture Decision Records with tombstone mechanism |
| **3** | docs/tasks.md | Atomic task execution with verification lock |
| **4 & 5** | State Governance | project_state.md updates, 3-strike rollback |
| **6** | Completion Gate | Mandatory checklist before task handoff |

## Core Protections

- **Phase 0 Rejection Lock**: No functional code before Phase 3, no exceptions
- **No Ghost Refactors**: Pre-existing defects go in a repair task, never fixed on the side
- **ADR Tombstone**: Rejected tech stacks are permanently banned from re-proposal
- **Verification Lock**: Tasks are not complete until tests pass with exit code 0
- **Emergency Escape**: Context threshold triggers state snapshot and forced recovery

## Installation

This is a [Codex](https://github.com/openai/codex) skill.

### Via skill-installer

`ash
python scripts/install-skill-from-github.py --repo <owner>/afd-os --path skills/afd-os
`

### Manual

`ash
cp -r skills/afd-os /skills/afd-os
`

Then restart Codex.

## Usage

Start a new conversation in Codex and say:

`
$afd-os I want to build a task management app
`

Or just describe your project — the skill triggers automatically when you mention starting a new project or AFD-OS.

## License

MIT — see [LICENSE](./LICENSE).
