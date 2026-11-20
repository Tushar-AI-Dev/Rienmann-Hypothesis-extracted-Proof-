# Riemann Hypothesis Lean Project (Extracted Archive)

This repository contains the extracted Lean source tree from the 14-part archive hosted at [alpo.ge](https://alpo.ge/lean.tar.gz.part01). The source is organized as a Lean project and includes the project configuration files and its `.lean` modules.

## Where the Riemann Hypothesis claim appears

- [`src/Main.lean`](src/Main.lean) declares `riemannHypothesis` and assigns it `rhOfAll`.
- [`src/Supplements/Kernels/MainTheorems.lean`](src/Supplements/Kernels/MainTheorems.lean) defines `rhOfAll` through `Formalism.VW.rh_of_every allChi`.
- [`src/Statements.lean`](src/Statements.lean) contains the formal statement `RiemannHypothesis`.

The formalization is distributed across many imported files; these entry points are a map into that source, not a standalone proof document. This repository records the archive's claim and does not certify that the claim is correct or that the project builds.

## Project layout

```text
.
├── src/
│   ├── Main.lean
│   ├── Statements.lean
│   ├── BuildAid/
│   ├── CompanionTheory/
│   ├── Development/
│   ├── Formalism/
│   ├── GroundTheory/
│   ├── Lemmata/
│   ├── PositivityTheory/
│   ├── ReciprocityTheory/
│   └── Supplements/
├── lakefile.toml
├── lake-manifest.json
└── lean-toolchain
```

See [`docs/PROJECT_STRUCTURE.md`](docs/PROJECT_STRUCTURE.md) for a brief guide to the source areas.

## Lean version and dependencies

The included `lean-toolchain` requests Lean `v4.33.1`. `lakefile.toml` declares Mathlib and the library targets. Dependencies are not vendored in this repository.

The source has not been built or checked in this preparation. Treat it as untrusted downloaded source; review it before running Lean or Lake commands.

## Provenance and licensing

The files were downloaded from the archive parts linked above and assembled for this repository. The archive does not include a license file, so no reuse license is implied here. Refer to the original [remark PDF](https://alpo.ge/remark.pdf) for its accompanying claims and context.
