# Reproducibility — Bounded n-Ball Reference Checks

**Run status:** an assistant-side Python standard-library calculation was executed on 2026-11-23 for the numeric checks below. It is **not** a formal proof, a blind test, CI certification, or an independent examination of the underlying Lab research.

## Reproduce using a local Python 3 interpreter

The following snippet computes the **established** Gamma closed form, compares it to the two-step recurrence for unit radius, and checks the exact equal-area square/disk offset example numerically. It uses only Python's standard library.

~~~python
import math

def v(n, r=1.0):
    return math.pi ** (n / 2) * r ** n / math.gamma(n / 2 + 1)

assert v(0) == 1.0
assert v(1) == 2.0

for n in range(2, 9):
    from_recurrence = (2 * math.pi / n) * v(n - 2)
    assert math.isclose(v(n), from_recurrence, rel_tol=1e-12)
    print(n, f"{v(n):.10f}")

t = 1.0
a = math.pi
area_square_offset = a + 4 * math.sqrt(math.pi) * t + math.pi * t * t
area_disk_offset = a + 2 * math.pi * t + math.pi * t * t
difference = area_square_offset - area_disk_offset
assert difference > 0
print(f"offset difference: {difference:.9f}")
~~~

## Recorded values, \(R=1\)

| \(n\) | \(V_n(1)\) |
|---|---:|
| 0 | 1.0000000000 |
| 1 | 2.0000000000 |
| 2 | 3.1415926536 |
| 3 | 4.1887902048 |
| 4 | 4.9348022005 |
| 5 | 5.2637890139 |
| 6 | 5.1677127800 |
| 7 | 4.7247659703 |
| 8 | 4.0587121264 |

At offset \(t=1\), the equal-original-area square and disk have outward-offset areas approximately \(13.373000711\) and \(12.566370614\) respectively; difference approximately **0.806630096**.

The tests check known formulas, a simple recurrence identity and a numeric consequence of Steiner's theorem. The exact symbolic derivation and the convexity conditions are stated in [Derivation](DERIVATION.md).

## Verification boundaries

- Floating-point tolerance: relative \(10^{-12}\) for the compared volume formulas, n=2…8.
- Assumptions: nonnegative integer dimensions, unit radius, Python's standard-library \(\Gamma\) implementation; convex planar square/disk for the offset example.
- No randomness or external dependencies.
- This is not verification of a unique new n-ball geometry, a general automated theorem prover, or a physical-law claim.
- The short calculation is an illustrative teaching snippet, not a separately licensed software package. See [Licensing](../../LICENSING.md).

Open corrections and references are welcome; see [Contributing](../../CONTRIBUTING.md).
