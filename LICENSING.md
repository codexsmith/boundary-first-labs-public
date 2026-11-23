# Licensing and Rights

**Interim public rights notice — version 0.1 (2026-11-23).**

This repository is public, but **no general open-source or Creative Commons license applies to the repository as a whole yet**. Public visibility alone is not an unrestricted grant to reproduce, redistribute, adapt, or commercially exploit copyright-protected material. Applicable exceptions, limitations, the public domain, and GitHub's platform terms remain unaffected.

The Lab's goal is to support appropriate open reuse *without* falsely claiming ownership of established mathematics or prematurely assigning rights to materials whose ownership or third-party status has not been reviewed.

## What copyright does and does not cover

- Mathematical facts, equations, abstract methods, scientific principles, and discoveries **as such** are not copyrighted in the United States.
- Original prose, drawings, diagrams, illustrations, and source-code expression may be protected to the extent they qualify under applicable law.
- A license to a paper's text or figures does **not** grant exclusive control over the mathematical relationships they explain.
- Attribution of mathematical origins is a scholarly and provenance obligation distinct from what copyright law requires.
- The Lab's names, marks, and logos are not licensed for third-party branding merely because they appear in this repository.

See [Intellectual Provenance](INTELLECTUAL_PROVENANCE.md) for the distinction between inherited machinery and the Lab's specific contribution.

## License choices for later releases (not currently granted)

| Material | Intended release approach |
|---|---|
| Standalone public code and executable examples | MIT as the prospective default after rights review; Apache-2.0 or another appropriate software license only by an explicit, scoped release decision |
| Original research writing and explanatory figures | Explicit, publication-scoped CC BY 4.0 where approved |
| Third-party assets, libraries, quotations, and datasets | Retain their original terms; identify required attributions and permissions |
| Product-specific or commercial implementations | Separate release terms; a public description alone is not a software grant |
| Names, logos, and brand identity | No permission for third-party branding is implied |

**Naming Apache-2.0, MIT, or CC BY 4.0 as candidates does not apply those licenses.** A release must identify the applicable complete license, the covered files, and the authorized rights holder. Creative Commons licenses are generally not recommended for software code.

Do not add a repository-wide `LICENSE` implying blanket coverage until a deliberate scope decision has been made. When open code ships, its own package may contain a `LICENSE` and appropriate notices.

## Public folder and file-level licensing

A public research or software project should carry its rights and release metadata in its own `projects/<slug>/release.yaml`. When a mixed project is approved for licensing, use path-level assignments and, where practical, SPDX file identifiers and REUSE-style license texts/notices. The reserved [LICENSES](LICENSES/README.md) directory and [project template](docs/templates/project/release.example.yaml) do not grant rights by themselves.

Different rights holders, third-party materials, fonts, diagrams, data, trademarks and source files must not be silently collapsed under one blanket license. Files with unresolved rights must not be publicly released merely because neighboring files are open.

## Per-artifact licensing contract

For every future licensed release, record:

1. Artifact name, version or commit, and included paths.
2. Author(s), copyright holder(s), and permission to license.
3. Actual license identifier and applicable text or unambiguous link.
4. Excluded third-party materials, fonts, images, trademarks, data, and other exceptions.
5. Source/attribution requirements and any compatible upstream licenses.
6. Publication approval and a correction/rights-contact route.

When rights are uncertain, release nothing beyond an appropriately cleared descriptive record. Do not silently substitute a permissive license for a required third-party permission.

## Clarifying examples

- **Euclidean n-ball formula:** the mathematical formula is not BFL-owned copyrightable subject matter; a newly written BFL explanation or diagram may have protectable expression.
- **Code implementing that formula:** the particular code may be copyrightable and should receive its own explicit software license if opened for reuse.
- **Composite research visualization:** each preexisting source or asset retains its own rights; the new presentation does not erase upstream ownership.

## References

- [U.S. Copyright Office — Circular 33](https://www.copyright.gov/circs/circ33.pdf)
- [17 U.S.C. § 102](https://www.law.cornell.edu/uscode/text/17/102)
- [Creative Commons — CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
- [Open Source Initiative — MIT](https://opensource.org/license/mit)
- [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)

This policy is a general publication and rights distinction, **not individualized legal advice**. The precise legal copyright holder and license grants must be confirmed before opening new copyrighted releases.
