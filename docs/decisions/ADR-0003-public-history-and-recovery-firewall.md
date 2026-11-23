# ADR-0003 — Public History and Recovery Firewall

**Date:** 2026-11-23  
**Status:** adopted for public repository architecture  
**Scope:** public history, retrospective outputs, imported content, correction records

## Context

The private Lab's bulk recovery and retrospectives preserve historical source bytes, provenance, negative findings, transitional decisions, and recovered research states. They also teach why a recovery snapshot or broad retrospective should not override an owning research artifact.

## Decision

- Preserve **public-facing** release history, decisions, corrections, retractions, and supersessions in this repository.
- Keep private raw conversation archives, migration imports, internal branch rescues, research-exhaust queues, private legal/operational records, and generated internal control state **out** of the public repository.
- A retrospective may guide editorial selection and reveal missing evidence, but it is not a new authoritative research source or automatic publication approval.
- Do not turn a historical recovered claim into a current result solely by moving it, summarizing it, or rendering it.
- When updating public artifacts, preserve earlier versions through Git history and explicit supersession/correction links; do not silently replace contested evidence.
- A public index should be a reproducible view over approved releases; generated views are not edited to counterfeit canonical changes.

## Consequences

Publish bounded, reviewed **public reconstructions** with source completeness and provenance explicitly declared. Keep failed/rejected experiments and known limitations visible when they materially affect a claim. Maintain the smallest useful history for public correction, not a second private-archive mirror.

This ADR does not transfer private archives, alter the private Lab's controls, or authorize release of any research artifact.
