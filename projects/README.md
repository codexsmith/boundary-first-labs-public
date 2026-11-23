# Public Project Packages

**One public project package owns each released artifact and its versioned source/evidence bundle.** Research-area guides, publication pages, and software indexes link here rather than copying the source.

A future approved package uses a readable slug, for example:

    projects/example-project/
      README.md
      release.yaml
      claims.md
      provenance.md
      [manuscript/]
      [figures/]
      [src/]
      [tests/]
      [evidence/]
      [LICENSE or LICENSES/ only when a release explicitly grants rights]

Bracketed folders are optional and should be created only when real, approved content exists. This example is **not a published project**, license, or scientific result.

For a reusable starting point, see [the project template](../docs/templates/project/README.md) and [release manifest example](../docs/templates/project/release.example.yaml).

**A package records two separate states:** source/claim maturity and permission to publish/use its expressive material. Project location, Git commit, or successful CI checks do not change either automatically.
