# Contractibility of the complex of incompressible Seifert surfaces: the knot case of Kakimizu's problem

**Guancheng Pan**

This repository holds a compiled PDF of a manuscript on Kakimizu's
contractibility problem for knots.

> **Read the status section at the bottom before you read anything else.**
> This manuscript is conditional, it has not been refereed, it has not been
> independently audited, and its argument was produced by an automated system.
> It is published here so that it can be checked, not because it has been.

---

## The statement

Let `K ⊂ S³` be a knot and let `E(K)` be its exterior. Let `IS(K)` be the
simplicial complex whose vertices are the ambient isotopy classes of
incompressible Seifert surfaces in `E(K)`, a finite set of distinct vertices
spanning a simplex exactly when its classes admit simultaneously pairwise
disjoint representatives; for an integer `ℓ ≥ g(K)` let `IS_ℓ(K)` be the full
subcomplex on the vertices of genus at most `ℓ`.

Kakimizu asked whether `IS(K)` is contractible. Przytycki and Schultens repeated
the question and identified the obstruction: the projection used to prove
connectedness is not known to be well defined on isotopy classes.

The manuscript proves that `IS(K)` and every `IS_ℓ(K)` are contractible —
**conditionally** on the named theorems and the residual hypotheses that §12
lists in full.

## The method, in one paragraph

The argument splits into two independent halves. The **combinatorial half** is
unconditional apart from one homotopy-theoretic input, isolated as `(C1)`: every
non-empty connected flag *exchange complex* is contractible, where an exchange
complex carries a complexity function subject to two axioms which require only
that an exchanging vertex **exist**, never that one be **selected**. That is what
gets past the obstruction. It uses no three-dimensional topology, no finiteness,
no local finiteness, and no bound on dimension or diameter. The **geometric
half** verifies that `IS(K)` is such a complex, through an exchange lemma for
incompressible surfaces obtained by minimal-surface methods.

Six technical appendices make the analytic and normal-surface inputs of the
geometric half self-contained: a version of the Hass–Scott area-minimisation
theorem 6.12 for manifolds with boundary; a compactness and blow-up analysis for
families of minimisers with fixed boundary; boundary regularity of the
constructed minimiser; the Haken normalisation and the weight–area inequality; a
self-contained treatment of divergence-form elliptic equations with Hölder
coefficients; and the combinatorial lemmas. A seventh appendix records how the
manuscript was produced.

136 pages.

## Contents of this repository

| File | |
|---|---|
| `kakimizu.pdf` | the manuscript, 136 pages, 11pt `article` |

The LaTeX source is not published here.

## Status — please read this before citing

Being typeset and compiling cleanly says nothing about whether the mathematics
is right. As of 2026-09-02:

- **The result is conditional, and the conditions are printed.** §12 carries a
  table of every residual hypothesis. Nothing has been deleted to make a
  conditional theorem look unconditional.
- **`(C1)` has never been proved here.** The statement that an inclusion with the
  homotopy extension property which is also a homotopy equivalence is a strong
  deformation retract inclusion is written in Appendix F as an explicit unproved
  hypothesis, and nothing in this manuscript is derived from it. Theorem 10.1 is
  stated conditionally on it. An earlier internal repair of it was withdrawn.
- **The universal-disjointness input remains research-level**, as do several
  questions the appendices raise about themselves: whether Dini continuity
  suffices for isothermal coordinates, whether `C¹` domains suffice, what happens
  at the two right-angled corners, and whether the Bers–Nirenberg input can be
  discharged by the replacement given in Remark E.52 — that replacement is new
  here and has not been audited by anyone.
- **Not refereed.** The manuscript has not been submitted to a journal and has
  not been read by a referee.
- **Not independently audited.** The argument was produced by an autonomous
  research system of roughly forty agent processes, every one of them running the
  same language model, Fable 5.1 (`claude-fable-5-1`). The internal reviews were
  performed by that same model family and are therefore **not** independent. By
  the criteria the project itself uses, the independent-audit count is **0 of 3**
  and **none of the four closure criteria — complete proof, self-containment,
  three independent cross-engine audits, machine-checked formalisation — is met.**
- **No formal verification is claimed.** No part of this manuscript has been put
  through an interactive theorem prover.
- **Appendix G lists ten places where the system's output was wrong**, and what
  each was corrected to. That appendix is the most useful page in the document
  for deciding how much weight to give the rest.
- **No novelty or priority is claimed.** No literature comparison has been run on
  this manuscript. If part of this argument is already in print, that has not been
  checked either way.

Corrections, counterexamples and pointers to prior art are all welcome — open an
issue. A refutation is worth more than a citation.

## Licence

Copyright © 2026 Guancheng Pan. `kakimizu.pdf` is licensed under
[Creative Commons Attribution 4.0 International](LICENSE) (CC BY 4.0): reuse,
redistribute and adapt freely, including commercially, with attribution.
