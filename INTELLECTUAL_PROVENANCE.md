# Intellectual Provenance and Contribution Boundaries

**Public policy — version 0.1 (2026-11-23).**

A mathematical fact is not the same object as an author's exposition of it. A reproduced theorem is not necessarily a new result. A useful integration can be a contribution without being a new primitive. Boundary First Labs requires these distinctions to remain inspectable through attribution, claims, and licensing.

## Contribution classification

Each substantive public artifact should distinguish, as applicable:

| Classification | Meaning | Public disclosure |
|---|---|---|
| **Inherited foundation** | Established mathematics, algorithms, scientific models, standards, and methods developed elsewhere | State the conventional name and cite authoritative prior art |
| **Prior influence or parallel work** | Earlier or independently developed approaches materially relevant to the artifact | Identify and compare; do not imply exclusive origination |
| **Reconstruction / translation** | A new presentation, derivation path, encoding, or interpretation of existing results | Identify the underlying known result and the particular representational changes |
| **Integration / architecture** | A composition of existing elements with declared contracts, constraints, and operational consequences | Identify each component, composition rule, and what the combination adds |
| **BFL-original construction** | A particular artifact, method, diagram, instrument, implementation, or proposed formal object developed in the Lab | Describe the exact claimed addition and its derivation/source history |
| **Claimed new result** | A specific theorem, empirical finding, classification, or other assertion of novelty | State assumptions, native literature baseline, proof/evidence, remaining defects, and review status |

These categories can coexist in one artifact. They describe provenance and the nature of a claim, **not its copyright status or scientific validity**. An independently developed construction can still have prior art; a novel diagram does not necessarily entail a novel theorem.

## Three independent records

1. **Intellectual provenance:** who developed which ideas or expressive elements, what is inherited, and which references and history support that account.
2. **Research authority:** which statements are definitions, hypotheses, established background, bounded demonstrations, verified claims, negative results, or unresolved defects.
3. **Legal rights:** which actual expressive works are protected, who holds the rights, whether third-party permissions exist, and which license (if any) applies to those works.

A provenance citation does not grant licensing rights. A copyright license does not prove novelty. A mathematical proof does not automatically provide copyright over the fact proved.

## Mathematical content and expression

In general, U.S. copyright law does not protect ideas, methods, processes, mathematical principles, equations, or facts **as such**. Original explanatory prose, illustrations, selection/arrangement, and software expression may qualify for protection, depending on the work and circumstances. This policy makes no assertion that copyright in a document prevents others from using the mathematical results it describes.

Mathematical novelty, scholarly credit, copyright, patents, and trademarks are **different questions**. A claimed discovery requires prior-art review and evidence; an applicable license governs only the rights actually held and granted. No author may license third-party material without authority.

Reference information: [U.S. Copyright Office Circular 33](https://www.copyright.gov/circs/circ33.pdf), [17 U.S.C. § 102(b)](https://www.law.cornell.edu/uscode/text/17/102), and [Creative Commons FAQ](https://creativecommons.org/faq/). This is a publication policy, not legal advice.

## Required disclosure for research releases

A substantive release should include:

- **Object:** title, version, release date, and purpose.
- **Native background:** existing theories, formulas, results, tools, and cited sources.
- **BFL operation:** what is reconstructed, composed, represented, or added.
- **Novelty ceiling:** what is *not* being claimed as new.
- **Claim status:** hypothesis, bounded demonstration, independently checked result, etc.
- **Evidence / limitations:** proof, tests, reproducibility, defects, counterexamples, domain assumptions, known failures, and meaningful negative results.
- **Provenance:** author/contributor distinctions and allowable source references; do not expose private lab materials or private conversation URLs solely to satisfy a public manifest.
- **Rights:** precise license scope, copyright holder where applicable, contributor/third-party clearances, and marks/assets exclusions.
- **Correction path:** where to challenge or amend the claim and trace revisions.

## Example: an n-ball construction

The standard formula for the volume of an n-dimensional Euclidean ball is inherited mathematics. BFL may publish its own rod–ball construction, executable derivation, diagrams, or dependency analysis as a distinct *presentation or instrument*. Those particular materials may embody copyrightable expression. The underlying formula and established theorems are not thereby claimed as BFL property. Any further mathematical result must be separately stated and established.

## Governance boundary

The public repository is a downstream projection. Canonical research evidence and maturity remain with their appropriate source owners. A release may explain or illustrate an artifact but cannot silently upgrade a conjecture, conflate common roles with formal equivalence, or erase predecessor work.

**Inspect the inheritance. Identify the addition. Test the consequence.**
