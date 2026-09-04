# Contractibility of the complex of incompressible Seifert surfaces: the knot case of Kakimizu's problem

**Guancheng Pan**

A preprint on Kakimizu's contractibility problem for knots. This is the
**third version** (4 September 2026, 52 pages). It replaces the first version
of 2 September 2026, which was a 136-page conditional manuscript; the
differences are listed under *Version history* below, and the earlier file
remains in the commit history of this repository.

> Read *What is proved, and on what* before citing anything from this
> manuscript. The main theorem is stated unconditionally, but one input taken
> from the literature is used at its word, and the manuscript says which.

---

## The statement

Let `K ⊂ S³` be a non-trivial knot and let `E(K)` be its exterior. Let `IS(K)`
be the simplicial complex whose vertices are the ambient isotopy classes of
incompressible Seifert surfaces in `E(K)`, a finite set of distinct vertices
spanning a simplex exactly when its classes admit simultaneously pairwise
disjoint representatives.

Kakimizu proved that `IS(K)` is connected. Whether it is contractible was asked
by Przytycki and Schultens, who also identified the obstruction: the projection
used in the connectedness proof is not known to be well defined on isotopy
classes.

- **Theorem A.** `IS(K)` is contractible.
- **Theorem B.** Every non-empty connected flag *exchange complex* is
  contractible. An exchange complex is a flag complex with a complexity
  function into a well-ordered set, subject to two axioms `(N1)`, `(N2)` which
  require only that an exchanging vertex *exist*, never that one be
  *selected*. That is what circumvents the obstruction.
- **Theorem C.** Every truncation `IS_ℓ(K)` on the vertices of genus at most
  `ℓ` is isometrically embedded in `IS(K)` and contractible; likewise the
  truncation by genus and relative area. Taking `ℓ = g(K)` recovers the
  Przytycki–Schultens theorem for the minimal-genus complex.
- **Theorem D.** For a non-split link satisfying a linking condition which
  forces every spanning surface to be connected, `IS(L)` is contractible.

## The method, in one paragraph

The proof of Theorem A verifies that `IS(K)` is an exchange complex for the
complexity `(genus, infimal area)` ordered lexicographically. Axiom `(N1)` comes
from Kakimizu's connectedness theorem, flagness and an apex construction;
axiom `(N2)` is the substance, and is supplied by an exchange lemma for
incompressible surfaces proved by minimal-surface methods: given two vertices
at distance two, cutting and recombining area minimisers in the two classes
along their intersection produces a common neighbour of strictly smaller
complexity. The exchange lemma rests on four inputs about area minimisers in
`E(K)`; three are cited from Hass–Scott and from Schultens (with the appendix
by Kapovich), and the fourth, boundary regularity of a relative area minimiser,
is both cited and proved again from the first variation of area and Hopf's
boundary point lemma. Theorem B is located against the existing literature: it
is not a corollary of dismantlability (a seven-vertex example is given), and
when every descending link is finite it follows from Zaremsky's descending-link
criterion by a reindexing.

## Contents of this repository

| File | |
|---|---|
| `kakimizu.pdf` | the manuscript, 52 pages, `amsart` |

The LaTeX source is not published here.

## What is proved, and on what

This section is part of the mathematics, not a disclaimer.

- **One input is taken from the literature at its word.** Theorem 6.12 of
  Hass–Scott asserts that the area infimum over the piecewise smooth surfaces
  isotopic to `F` rel `∂F` is attained *within that class*. The printed proof
  establishes interior regularity of the limit and does not reach its behaviour
  at `∂M`. Everything geometric in this paper, and everything resting on the
  appendix to Schultens, rests on that assertion being true. The manuscript
  isolates exactly which clause is consumed (§2, the displayed statement
  labelled as the one reading), states the underlying existence question as
  the first of its open problems (§1.5), and records five routes around the
  local Plateau question that do **not** work.
- **The residual content of Theorem B is confined to exchange complexes with an
  infinite descending link.** Whether `IS(K)` is one is not known.
- **Theorem D does not extend to general links.** The step that fails is
  identified; no counterexample is given, only an obstruction.
- **The equivariant version is blocked**, not merely unproved, and there is no
  analogue for a general Haken manifold because the required connectedness
  has no source in the literature.
- **A small part of §6 has been formalised in Lean 4** against mathlib
  (913 lines, no `sorry`, no `axiom`, no `native_decide`): the ordering
  statement, the reduction to an injective complexity, a reformulation of
  dismantlability, and the seven-vertex example. Theorem B itself has **not**
  been formalised and no such claim is made.

## Version history

- **v3, 4 September 2026 (this file).** The manuscript was rebuilt from the
  first version under the following rules: textbook facts are cited, never
  reproved; every citation's statement *and* numbering was checked against the
  source text; residual hypotheses are named in the statement of the theorem
  that uses them, not collected in a table. Concretely: the six appendices of
  v1 are gone; the homotopy-theoretic input `(C1)` that v1 left unproved is no
  longer needed (the argument now uses two propositions from Hatcher instead);
  the boundary-regularity hypothesis `(R1)` of v1 is now a theorem (§2), with
  the exposure reduced to the single clause described above; §5 (the exchange
  lemma) was rewritten with a complete case division, including the case of
  disjoint boundaries with interior tangencies that v1 omitted; the
  combinatorial theorem was relocated against dismantlability and Zaremsky's
  criterion. Two rounds of external referee comments and several rounds of
  adversarial checking were applied in the course of this rebuild.
- **v1, 2 September 2026.** 136 pages, `article`. Conditional on `(C1)` and on
  a table of residual hypotheses. Superseded; available in the commit history.

## Status

This is a preprint. It has not been submitted to a journal and has not been
refereed. The manuscript was produced with substantial assistance from large
language models, used for literature search, drafting and adversarial checking;
the author is responsible for all statements. The most recent corrections
(to §2 and §5) were checked by the same process and not yet by an independent
referee. No literature comparison has been carried out on this manuscript, so
no claim of novelty or priority is made here; if part of this argument is
already in print, that has not been checked either way.

Corrections, counterexamples and pointers to prior art are all welcome — open an
issue. A refutation is worth more than a citation.

## Licence

Copyright © 2026 Guancheng Pan. `kakimizu.pdf` is licensed under
[Creative Commons Attribution 4.0 International](LICENSE) (CC BY 4.0): reuse,
redistribute and adapt freely, including commercially, with attribution.
