# hex-lll-mathlib

Mathlib correspondence proofs for [`hex-lll`](https://github.com/kim-em/hex-lll):
the executable LLL reduction is connected to Mathlib's lattice / submodule
theory. Proof-only.

```
require HexLLLMathlib from git "https://github.com/kim-em/hex-lll-mathlib.git" @ "<rev>"
```

Depends on `hex-lll`, `hex-gram-schmidt-mathlib`, `hex-matrix-mathlib`,
`hex-gram-schmidt`, `hex-matrix`, and Mathlib (all pinned). Development happens
in [`hex-dev`](https://github.com/kim-em/hex-dev).

The pins above must stay consistent: when you bump `hex-lll`, bump this repo to
match in the same step. Lake does not reconcile mismatched revisions of a
package required at more than one point in the dependency graph, so an
out-of-sync pin fails to resolve.
