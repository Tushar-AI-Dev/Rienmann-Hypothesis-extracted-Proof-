# Project Structure

The source tree follows Lean module imports: directory names map to namespaces, and `.lean` files contain definitions, lemmas, and theorems.

| Path | Role in the extracted project |
| --- | --- |
| `src/Main.lean` | Top-level theorem declarations, including `riemannHypothesis`. |
| `src/Statements.lean` | Formal propositions used by the top-level declarations. |
| `src/Supplements/` | Supplementary theorem modules; `Kernels/MainTheorems.lean` provides `rhOfAll`. |
| `src/Formalism/` | Formal theorem development imported by the supplement modules. |
| `src/Development/` | General mathematical development modules. |
| `src/CompanionTheory/` | Supporting theory modules. |
| `src/GroundTheory/` | Foundational theory modules. |
| `src/BuildAid/`, `src/Lemmata/` | Build support and lemma modules. |
| `src/PositivityTheory/`, `src/ReciprocityTheory/` | Additional theory modules. |

The archive contains about 175,000 Lean source files. This guide is an orientation aid; follow the `import` statements to trace any particular result through its dependencies.
