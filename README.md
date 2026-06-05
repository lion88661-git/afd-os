# AFD-OS v1.0 — AI First Development Operating System

> **Codex Skill**: Six-phase document-driven AI-first development methodology with architecture-first governance.
> **GitHub**: [lion88661-git/afd-os](https://github.com/lion88661-git/afd-os) · **License**: MIT

## What is AFD-OS?

AFD-OS v1.0 is a structured development protocol that turns an AI coding agent into a Chief Architect & Project Arbiter. It forces all decisions onto the filesystem — AI works against documents, code is merely the executable artifact.

## Six Phases

| Phase | Output | Description |
|---|---|---|
| **0** | Product Matrix | Mandatory requirement simplification via 5-dimension matrix |
| **X** | Non-template handling | Fallback for requests outside the matrix |
| **1** | docs/business_breakdown.md | Business goals, actors, user flows, MVP scope |
| **1.5** | docs/prd.md | Prioritized features, user stories, flows |
| **2** | docs/system_design.md | Single tech stack, data model, API contracts, dir structure |
| **2.5** | docs/adr/ADR-XXX.md | Architecture Decision Records with tombstone mechanism |
| **3** | docs/tasks.md | Atomic task execution with verification lock |
| **4 & 5** | State Governance | project_state.md updates, 3-strike rollback |
| **6** | Completion Gate | Mandatory checklist before task handoff |

## Product Positioning Matrix (Phase 0)

| Dimension | Options |
|---|---|
| 1. Product Form | [1] Web  [2] Mini Program  [3] Desktop  [4] Native App  [5] Browser Extension  [6] Backend/CLI |
| 2. Business Type | [A] Content Display  [B] Form/Management  [C] SaaS/Tool  [D] E-commerce/Payment  [E] Social/Real-time |
| 3. Infrastructure | [X] No Database  [Y] BaaS Cloud  [Z] Independent Backend |
| 4. Auth System | [Q1] Public  [Q2] Username/Password  [Q3] Third-party Login |
| 5. Business Model | [S1] Open Source/Personal  [S2] One-time Purchase  [S3] SaaS Subscription  [S4] Ad-supported |

## Core Protections

- **Phase 0 Rejection Lock**: No functional code before Phase 3, no exceptions
- **No Ghost Refactors**: Pre-existing defects go in a repair task, never fixed on the side
- **ADR Tombstone**: Rejected tech stacks are permanently banned from re-proposal
- **Verification Lock**: Tasks are not complete until tests pass with exit code 0
- **Emergency Escape**: Context threshold triggers state snapshot and forced recovery

## Installation

This is a [Codex](https://github.com/openai/codex) skill.

### Via skill-installer (Recommended)

```bash
python scripts/install-skill-from-github.py --repo lion88661-git/afd-os --path . --name afd-os

```

> **Note**: `--name afd-os` is required because the skill lives at the repo root (`--path .`).

### Manual

```bash
git clone https://github.com/lion88661-git/afd-os.git /tmp/afd-os
cp -r /tmp/afd-os /skills/afd-os

```

> Restart Codex after installation to pick up the new skill.

### One-liner

```bash
git clone [https://github.com/lion88661-git/afd-os.git](https://github.com/lion88661-git/afd-os.git) "$CODEX_HOME/skills/afd-os"

```

## Usage

Start a new conversation in Codex and say:

```bash
$afd-os I want to build a task management app

```

Or just describe your project — the skill triggers automatically when you mention starting a new project, AFD-OS, or structured development workflow.

## License

MIT — see [LICENSE](https://www.google.com/search?q=./LICENSE).

```

```
