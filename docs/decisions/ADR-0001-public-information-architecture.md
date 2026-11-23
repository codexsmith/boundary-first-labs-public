# ADR-0001 — Public Information Architecture

**Date:** 2026-11-23  
**Status:** adopted for the public repository skeleton  
**Scope:** `codexsmith/boundary-first-labs-public`, navigation and public artifact placement only

## Context

The private Lab maintains distinct foundations, core theory, domains, operations, publication projections, migrations, and extensive recovery evidence. Its accumulated architecture decisions prioritize semantic locality, source ownership, routing, nonduplicated state, and authority carried by metadata rather than folder placement.

That private topology is useful as a **source of design constraints**, not an appropriate public directory tree.

## Decision

Keep one **public project package** as the owner of each published artifact. Separate public discovery and explanation into short, audience-facing routes:

- `start-here/`, `about/`: accessible orientation.
- `method/`: Boundary First as a portable method, distinct from theory.
- `theory/`: Boundary Theory and its bounded formal program.
- `research/`: native-domain reader indexes; links, not duplicate manuscripts.
- `projects/`: owner-local source, reproducibility, proof/evidence, provenance, releases, and scoped rights.
- `publications/`, `software/`: human-facing catalogs resolving back to project packages.
- `assets/`, `LICENSES/`: only cleared reusable public materials with distinct rights.
- `docs/`, `history/`: navigation, decisions, release standards, and public revisions.

No public counterparts of `999_Library`, `998_Intake`, private registers, agent queues, bulk imports, or recovery dumps are created.

## Relations and authority

**Institution != method != research program != apparatus != instrument != domain result.** A common term across domains is not proof of common semantics. Public indexes do not become scientific authority.

The public project owns the bytes of its **published version**, but the original research's canonical Lab owner retains authority over ongoing work and evidence. Metadata—not folder location—declares claim status and rights. For cross-domain work, one owner is chosen and other routes link to it.

## Alternatives rejected

1. **Mirror the private numbered corpus:** exposes confusing administrative structure and encourages accidental disclosures and inferred authority.
2. **Duplicate each work under mathematics, software, publications, and projects:** creates competing copies and divergent rights or claim statuses.
3. **Use only one broad flat list:** prevents local package reconstruction and makes provenance/tests/licensing hard to inspect.

## Consequences

Projects use stable readable slugs and durable identifiers in their manifests. Research area folders remain navigation routes. A project may optionally contain source, tests, evidence, proofs, figures, license files, and corrections as justified by its actual approved release. Empty reserved folders are not created.

This is a public routing decision, not publication of any private research, proof, source code, or unreviewed content.
