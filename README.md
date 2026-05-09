# ashkharh — The Play (Existence in Motion)

**ashkharh** is the narrative and character layer of the **UNEXUSI** ecosystem, operating within the **tiezerk** container. It is the "Play" layer: the place where characters move, concepts breathe, and locations hold tension.

## Purpose

This repository manages:
- **Living entities** and their Prime Stage progression.
- **Narrative seeds** (concepts) that drive becoming.
- **Play environments** (locations) where paths cross.
- **Story arcs** and world events.
- **Play mechanics** and song-avatar mappings.

## Repository Layout

| Directory | Contents |
|-----------|----------|
| [`characters/`](characters/) | Living entities — Runaytr, Sonny, and others |
| [`concepts/`](concepts/) | Narrative seeds — The Germ, Wisps, Yod, and others |
| [`locations/`](locations/) | Play environments — Stone Tankard, and others |
| [`narratives/`](narratives/) | Story arcs and world events |
| [`systems/`](systems/) | Play mechanics and song-avatar mappings |
| [`.github/workflows/`](.github/workflows/) | Automation — Prime Progression and security checks |

## Core Loop — The Triadic Pattern

Every entity update and automation must follow the Triadic pattern:

1. **STORY** — Narrative context.
2. **STATUS** — System state (Prime Stage / Ka Pressure).
3. **NEXT ACTION** — Immediate continuation.

## Chain of Custody

All new documents must be registered via **Pull Request** to ensure witnessing before integration. The [Prime Progression workflow](.github/workflows/prime-progression.yml) automatically validates that every Play-layer document satisfies the Triadic pattern.

---

## CI/CD Security Hardening

- Upgraded the EthicalCheck workflow to a maintained OWASP ZAP baseline scan action.
- Added workflow concurrency control to avoid overlapping scans.
- Added artifact upload and job-summary publishing for easier security report review.
- Kept scans non-blocking by default (fail_action: false) to encourage iterative hardening.
- Implemented timeouts, safer checkouts, and tighter permissions for all workflows.
