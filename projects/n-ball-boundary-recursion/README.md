# The n-Ball: Construction, Recursion, and What a Summary Forgets

**Genre:** public educational mathematical calibration  
**Release:** 0.1.0 — 2026-11-23  
**Status:** published introductory exposition of established geometry, with a Boundary First interpretation; **not** a novel theorem, peer-reviewed paper, or formal promotion of the private Lab's working research.

## Why this example?

The n-dimensional ball lets us compare several mathematical objects often compressed into the same informal phrase: a geometric region, its boundary, its measure, an object-level construction, and a recurrence between measures.

A rod is a one-dimensional ball. Two rods form a square by Cartesian product, **not a Euclidean disk**. A Euclidean ball can instead be constructed by sweeping a family of lower-dimensional cross sections whose radii vary with the sweep coordinate. The resulting volume can be computed through a known Gamma-function formula and a two-step numerical recurrence.

These are established mathematical facts. The specific **Boundary First reading** is to keep the type and loss of each representation visible: geometric object, boundary, radius-indexed family, scalar measure, and continuation operation are not interchangeable.

## A short path through the mathematics

1. **Start with a rod:** \(B^1_2(R)=[-R,R]\), whose length is \(2R\).
2. **Compare constructors:** two rods produce the square \(B^2_\infty(R)\); the Euclidean disk is \(B^2_2(R)\), and they have different areas.
3. **Build by slicing:** \(B^{n+1}_2(R)\) is a union of \(n\)-balls of changing radius indexed by a new coordinate.
4. **Measure and recurse:** the classical formula is
   \[
   V_n(R)=\frac{\pi^{n/2}R^n}{\Gamma(n/2+1)},
   \qquad
   V_{n+2}(R)=\frac{2\pi R^2}{n+2}\,V_n(R).
   \]
5. **Check what is lost:** two shapes can have equal area but give different areas after the same outward-offset operation. Area alone does not determine that future consequence.

## Browse this public package

- [Construction and mathematical derivation](DERIVATION.md): definitions, slicing, recurrence, rod–ball distinction, and exact negative control.
- [Claim and contribution ledger](claims.md): standard mathematics vs. the specific interpretive addition, with explicit nonclaims.
- [Reproducibility and checked values](REPRODUCIBILITY.md): a small standard-library reference calculation and its scope.
- [References](REFERENCES.md): accessible, external mathematical sources.
- [Source and rights provenance](PROVENANCE.md) and [release manifest](release.yaml): what is public, what is inherited, and what is **not licensed**.

This is one canonical public project package. The [mathematics](../../research/mathematics/README.md), [publication](../../publications/README.md), and [start-here](../../start-here/README.md) pages only **link** to it.

## What would make this research rather than a teaching calibration?

A future comparative study would need explicit task and use cases, a domain-native baseline, a measurable benefit of the extra typed relationships, withheld counterexamples, independently reproducible evidence, and a correction mechanism. Its outcome might be "the conventional methods are already sufficient." That is an acceptable result.

**Rights:** no open license is applied to the project's original prose or layout at this stage. The mathematical relationships themselves are established knowledge and are not claimed as proprietary. See [Licensing](../../LICENSING.md).
