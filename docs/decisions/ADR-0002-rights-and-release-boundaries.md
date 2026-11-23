# ADR-0002 — Rights and Release Boundaries

**Date:** 2026-11-23  
**Status:** adopted for the public repository skeleton  
**Scope:** package licensing, disclosure, claim maturity, and release metadata

## Decision

A public release must keep **three independent records**: intellectual provenance; scientific/claim authority; and copyright/licensing permissions. It must also state its version and correction path.

The intended future defaults are:

- **Original research exposition / approved original diagrams:** CC BY 4.0 when the rightsholder authorizes it.
- **Approved open-source code:** MIT unless a separately reviewed alternative such as Apache-2.0 is chosen.
- **Mixed packages:** per-file or per-path SPDX/REUSE-style license assignments and third-party notices.
- **Names, logos, private data, third-party materials, or commercial code:** not implicitly covered.

**No blanket open license is granted by the initial public skeleton.** There is deliberately no root `LICENSE` applying to everything.

## Why

Copyright in original explanatory text, graphics, or code is distinct from mathematical facts and methods as such. The Lab can receive scholarly credit for an original construction or integration without claiming private property rights in conventional equations. A publication status does not establish novelty or proof. Releasing code without verifying ownership can incorrectly purport to license rights held by someone else.

## Release condition

A future project must supply its owner/version, inherited sources, specific addition, claim status and limits, proof/test evidence where available, precise copyrighted material and rights holder, file-scoped license grant, third-party exceptions, and authorized steward/correction channel.

Use the [release-manifest example](../templates/project/release.example.yaml) and [release checklist](../templates/RELEASE_CHECKLIST.md). An unfilled template is not a license or a publication.

## Consequences

A mathematical formula may be restated without treating its underlying truth as BFL-owned copyright. Licensable expressive material gets an explicit granted license only after appropriate review. Projects stay in review outside the public repo until cleared; publishing a skeleton does not admit scientific results.
