# The Model Forgot the Boundary

**A five-minute example of why Boundary First asks what comes next.**

Suppose you describe a region by one number: its area. That's reasonable if the only question is "how much area does it occupy right now?"

But now imagine expanding every point of the shape outward by the same distance. Can that one number predict the new area?

Take a unit disk and a square whose side is \(\sqrt{\pi}\). Their original areas are equal: \(\pi\). After an outward expansion of one unit, their areas differ by approximately **0.80663** square units.

Why? Their perimeters differ, and the classical planar Steiner formula needs both the original area and the perimeter to calculate the expanded area of a convex shape.

The original area was **correct**, but it was not a sufficient description for the *later operation*.

That is the kind of question Boundary First asks of software, mathematics, and other consequential systems: **which distinction is the current model allowed to forget, and for which future use?** Different fields have their own mature mathematical and practical answers; the Lab's method should use those before claiming anything new.

This is an accessible illustration, not a social-science conclusion or a novel mathematical discovery.

[See the exact construction, sources, numerical check, and claim limits in the n-ball public project](../projects/n-ball-boundary-recursion/README.md).

For a more general procedure, read the [Boundary First field guide](../method/BOUNDARY_FIRST_FIELD_GUIDE.md).
