# Publication and Research Status

**Public release policy — version 0.1 (2026-11-23).**

This repository is a **public projection**, not the complete working laboratory or an authority over its canonical research. A publication's availability is distinct from the maturity of the results it describes.

## The release contract

For every substantive research artifact, identify:

1. **Object and purpose:** what is being represented and what task it serves.
2. **Inherited foundations and prior art:** conventional mathematics, existing algorithms, standards, established literature, and parallel contributions.
3. **BFL-specific addition:** the precise reconstruction, composition, implementation, instrument, relation, or claimed result.
4. **Claim ceiling:** definitions vs. conjectures vs. checked bounded results; what has *not* been shown.
5. **Assumptions and limits:** state/domain, conventions, tolerances and units where relevant, possible failure conditions.
6. **Evidence:** proof, code, tests, source data, counterexamples, negative results, reproducibility instructions, and independent review where available.
7. **Rights and provenance:** origin, author/contributor attribution, copyright scope, explicit licenses, third-party restrictions, cleared publication source.
8. **Correction path:** release version/date, owner approval, known defects, and revision trace.

Use [Intellectual Provenance](INTELLECTUAL_PROVENANCE.md) and [Licensing and Rights](LICENSING.md) for the corresponding rules.

## Research-status vocabulary

| Label | Meaning |
|---|---|
| **Established background** | An attributed existing result or technique, not claimed as a BFL invention |
| **Working definition** | A proposed vocabulary, formal object, or explicit assumption without automatic external validation |
| **Hypothesis / conjecture** | A claim to be tested or proved; not presented as established |
| **Bounded demonstration** | A construction, test, or computation that supports only the declared scope |
| **Verified result** | A specific claim with stated evidence, method, and checking conditions; verification scope must be explicit |
| **Negative result / open defect** | A counterexample, failed test, obstruction, missing proof, or unresolved issue |

A locally passed test is not an independently replicated experiment. A formal mathematical correspondence is not an empirical physical theory. An analogy, diagram, or common analytical role does not prove cross-domain equivalence. A useful systematization is not necessarily a new theorem.

## Publication vs. promotion

Publishing a polished representation does **not**:

- promote hypotheses into theorems;
- confer ownership of mathematical laws or inherited algorithms;
- change the original Lab artifact's evidence or governance status;
- transform a prototype into a production-ready service;
- authorize release of private data, proprietary code, contributor works, or licensed third-party material.

Novelty claims must survive native-domain comparison. If existing machinery already suffices, document that finding instead of disguising the reduction.

## Corrections, criticism, and negative outcomes

Preserve meaningful failures and counterexamples. A revision should identify what changed, what evidence motivated it, and which earlier claims are narrowed, superseded, or withdrawn. Avoid silent rewriting of the public record.

## Public package and navigation contract

A future substantial release lives in one versioned [project package](projects/README.md) with its claim and rights metadata. Domain guides, [publications](publications/README.md), and [software](software/README.md) are navigation views, not second copies. Use the [release example](docs/templates/project/release.example.yaml) and [release checklist](docs/templates/RELEASE_CHECKLIST.md) only after rights and publication approval.

## Founder review of disclosure scope

Publicly visible repositories are not suitable staging areas for unreviewed substantive research. A request to create a folder, populate a skeleton, or explain the Lab does not grant continuing authorization to publish specific proofs, derivations, reproducibility bundles, executable methods, or other technical material. Apply a separate, affirmative review of disclosure scope **before** committing such material to a public branch. Rights clearance and scientific maturity checks are necessary but do not replace this disclosure review.

## Current repository scope

The repository currently contains public orientation, architecture, documentation templates, and governance rules. It does **not** release or endorse additional theorems, physics results, professional legal conclusions, executable products, or third-party content. Each substantive research or software release requires its own review.
