# ADR-0004 — Reverse-Chronological Breadth-First Public Recovery

**Date:** 2026-11-23  
**Status:** proposed / review required  
**Scope:** public source-selection and historical-presentation policy only  
**Public protocol:** [RCBF-001](../REVERSE_CHRONOLOGICAL_BREADTH_FIRST_RECOVERY.md)

## Context

The Lab's work has developed by longitudinal refinement. Earlier records remain valuable, but recovering and presenting the entire corpus in depth-first order would postpone public usefulness and may obscure later cross-domain synthesis.

The current architectural diagrams and public capability structure offer a practical entry point. They are candidate orientation surfaces, not proof or a mandate to reinterpret history.

Existing [ADR-0001](ADR-0001-public-information-architecture.md) and [ADR-0003](ADR-0003-public-history-and-recovery-firewall.md) already separate public projections from private authority and forbid mirroring private recovery archives.

## Proposed decision

Adopt a public-facing recovery orientation of **current baseline → backward chronological windows → breadth-first survey across eight facets → owner-reviewed synthesis → forward public projection**.

Keep history immutable. Relate older sources to the current model using evidence-backed, typed connections and retain contradictions. Newer work is a useful search prior, never an automatic truth override.

Keep public Codexware MVP implementation independent of the complete historical recovery effort.

## Alternatives considered

- **Earliest-first reconstruction:** preserves discovery order but delays present-day explanation and compounds architectural translation work.
- **One-facet depth-first excavation:** produces deep local studies but creates uneven public coverage and misses cross-facet connections.
- **Rewrite old sources into present terminology:** rejected; destroys provenance and can manufacture false continuity.
- **Mirror private lab archives into public Git:** rejected under ADR-0003 and publication/licensing rules.

## Implications and affected paths

- `docs/REVERSE_CHRONOLOGICAL_BREADTH_FIRST_RECOVERY.md` — candidate protocol.
- `docs/README.md` and `docs/decisions/README.md` — public entrypoints.
- A future reviewed frontier manifest or visualization may be added, but **not** until real public-safe source objects, owners and rights permit it.
- No change to private Lab registries, source histories, agent execution machinery, or existing public project releases.

## Review and implementation gates

Human review of this public architecture is required before calling it adopted. A future scheduler must demonstrate actual chronological ordering, eight-facet coverage, source-date uncertainty, exception logging, provenance, owner routing and output validation.

An approved architectural decision is not evidence that the scheduler exists or that historical recovery has run.

**Rights and publication:** governed by [Licensing](../../LICENSING.md) and [Publication Policy](../../PUBLICATION_POLICY.md). No new blanket license or release of private material.
