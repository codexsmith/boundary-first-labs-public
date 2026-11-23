# Mathematical Construction and Representation Boundaries

**Scope:** elementary Euclidean/norm-ball geometry and planar convex offsets. All identities in this note are inherited mathematics. The Boundary First contribution here is a deliberately typed presentation, **not a claim of new geometry**.

## 1. Define the carrier

For integer \(n\ge1\) and \(R>0\), let
\[
B_2^n(R)=\{x\in\mathbb R^n:\sum_{j=1}^{n}x_j^2\le R^2\}.
\]
Use \(B_2^0(R)=\{()\}\) and, by convention, \(V_0(R)=1\). For \(n\ge1\), the Euclidean ball has boundary \(\partial B_2^n(R)=S^{n-1}(R)\), and its n-dimensional volume is \(V_n(R)\).

The *ball* is a set, its *boundary* is a different set, and *volume* is a scalar measurement. Keeping those types distinct prevents substituting a number for a geometric object.

## 2. Rod times rod is not the Euclidean disk

The rod \(I_R=[-R,R]\) is a one-dimensional Euclidean ball. Its Cartesian square is
\[
I_R\times I_R=[-R,R]^2
=\{(x,y):\max(|x|,|y|)\le R\}
=B_\infty^2(R).
\]
This is the \(L^\infty\) square with area \(4R^2\), not the Euclidean disk
\[
B_2^2(R)=\{(x,y):x^2+y^2\le R^2\},
\qquad A(B_2^2(R))=\pi R^2.
\]

Both are topological disks, but that topological equivalence does **not** establish equal metrics, boundary shapes, or areas. The construction's norm and measure must be declared.

## 3. Geometric one-step construction by slicing

For \(t\in[-R,R]\), the cross section of \(B_2^{n+1}(R)\) at last coordinate \(t\) is an \(n\)-ball of radius \(\sqrt{R^2-t^2}\):
\[
B_2^{n+1}(R)
=\bigcup_{t=-R}^{R}
\left(B_2^n(\sqrt{R^2-t^2})\times\{t\}\right).
\]

This is an **object-level constructor**: it consumes an entire radius-indexed family of cross sections. It is not equivalent to multiplying a scalar volume by a fixed number. By Fubini's theorem, its volume satisfies
\[
V_{n+1}(R)
=\int_{-R}^{R}V_n(\sqrt{R^2-t^2})\,dt.
\]
Using homogeneous scaling \(V_n(a)=V_n(1)a^n\), the integral can be evaluated through classical Beta/Gamma identities.

## 4. Two-step scalar recurrence

Pair the two new coordinates into a polar disk. For \(n\ge0\),
\[
\begin{aligned}
V_{n+2}(R)
&=\int_{u^2+v^2\le R^2}
 V_n\!\left(\sqrt{R^2-u^2-v^2}\right)\,du\,dv\\
&=2\pi V_n(1)\int_0^R
  \rho(R^2-\rho^2)^{n/2}\,d\rho\\
&=\frac{2\pi R^2}{n+2}V_n(R).
\end{aligned}
\]

The scalar recurrence must be supplied with *both parity seeds*, \(V_0(R)=1\) and \(V_1(R)=2R\), to generate all integer dimensions. This differs from the one-step, radius-indexed geometric construction.

Gamma's standard functional equation, \(\Gamma(z+1)=z\Gamma(z)\), packages these sequences into
\[
V_n(R)=\frac{\pi^{n/2}}{\Gamma(n/2+1)}R^n.
\]
For example \(V_2(R)=\pi R^2\) and \(V_3(R)=4\pi R^3/3\). No dimension outside the nonnegative integers is being asserted to be a literal Euclidean ball merely because the right-hand formula has an analytic continuation.

## 5. Exact negative control: equal area, different consequences

Let \(D\) be the disk of radius 1 and \(Q\) a square of side \(\sqrt{\pi}\). Both are planar compact convex bodies with area \(\pi\):
\[
A(D)=A(Q)=\pi.
\]
Their perimeters differ:
\[
P(D)=2\pi,\qquad P(Q)=4\sqrt{\pi}.
\]

Define the permitted operation \(T_t(K)=K\oplus tD\), the Minkowski sum with a disk of radius \(t\ge0\). The **classical planar Steiner formula**, under its convexity assumptions, gives
\[
A(T_t(K))=A(K)+tP(K)+\pi t^2.
\]

Therefore
\[
A(T_t(Q))-A(T_t(D))
=t(4\sqrt{\pi}-2\pi)>0
\quad\text{for }t>0.
\]

A representation \(q(K)=A(K)\) cannot predict future area after all \(T_t\): it assigns the *same* value to \(D\) and \(Q\), which have *different* future results. For this specified operation family and observed quantity, \((A,P)\) is sufficient for computing those future areas. That statement does not mean area and perimeter reconstruct the original shape or suffice for every other operation, such as arbitrary clipping.

This is an established convex-geometric example of **use-relative information sufficiency**, not a novel general theorem.

## 6. The Boundary First accounting layer

| Thing represented | Native mathematical object | What it preserves / omits |
|---|---|---|
| Rod | interval \(I_R\) | a one-dimensional geometric carrier |
| Square from two rods | \(B_\infty^2(R)\) | product construction; not Euclidean area/metric |
| Euclidean ball | \(B_2^n(R)\) | full region and its intrinsic shape |
| Boundary | \(S^{n-1}(R)\) | boundary locus; not the interior measure |
| Scalar volume | \(V_n(R)\) | measure; generally loses shape and boundary detail |
| Scalar recurrence | \(V_{n+2}=2\pi R^2 V_n/(n+2)\) | scalar volumes under specified dimensional family |
| Offset readout | \(K\mapsto A(K\oplus tD)\) | depends on both area and perimeter for planar convex \(K\) |

The table is a **representation and dependency audit**. It does not identify all listed mathematical objects, prove a universal boundary calculus, or establish a new physical mechanism.

For sources and qualifications, see [References](REFERENCES.md) and [Claims](claims.md).
