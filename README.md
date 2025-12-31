# Conceptual Roadmap: Why a Fisher-Geometry Companion Paper?

This repository accompanies the paper  
**“Constraint-Induced Reversibility under Natural-Gradient Dynamics”**,  
which serves as a conceptual companion to  
**“The Inaccessible Game”**.

The purpose of this note is not to introduce new results, but to clarify
*why* a second paper is needed, *what conceptual distinctions it isolates*,
and *how the two formulations should be read together*.

The core message is simple:

> The reversible (antisymmetric) structure observed in the inaccessible game
> is *not* a coordinate artefact of working in natural parameters.
> It is a consequence of constraint geometry.
> The choice of dissipation metric determines whether that structure appears
> *emergent* or *canonical*, not whether it exists.

What follows explains that statement.

---

## 1. What the original paper does

The inaccessible game derives dynamics from four information-theoretic axioms
and an information relaxation principle:

- joint entropy is maximised,
- a sum of marginal entropies is conserved,
- dynamics are defined on an exponential-family manifold.

In the original formulation:

- coordinates are *natural parameters*,
- steepest ascent is defined using a *Euclidean inner product*,
- the constraint is enforced by orthogonal projection,
- linearisation reveals a GENERIC-like decomposition
  $$
    \dot{\theta} = (S + A) \theta,
  $$
  with symmetric (dissipative) and antisymmetric (reversible) parts.

The antisymmetric component is *not postulated* — it emerges from
constraint enforcement.

---

## 2. Why this raises a legitimate question

Natural parameters are closely associated with *information geometry*.
In that setting, the canonical choice of metric is the Fisher (or BKM) metric,
and steepest ascent is given by the *natural gradient*.

This raises an obvious concern:

> “If the Fisher metric had been used instead of a Euclidean metric,
> would the antisymmetric (reversible) structure still appear?”

If the answer were “no”, then the reversible structure could be dismissed as
a coordinate or metric artefact.

The companion paper exists to answer this question cleanly.

---

## 3. The key conceptual distinctions (often conflated)

Understanding the answer requires separating several notions that are
frequently blurred:

### (i) Coordinates vs metrics
- Natural parameters are a *coordinate choice*.
- Euclidean vs Fisher/BKM is a *metric choice*.
- Natural parameters do *not* imply natural gradients unless the Fisher metric
  is explicitly chosen.

### (ii) Constraints vs Casimirs
- A *constraint* is enforced on the full dynamics (via projection).
- A *Casimir* is conserved by the antisymmetric operator alone.
- A quantity can be conserved without generating Hamiltonian flow.

### (iii) Antisymmetry vs Poisson structure
- An antisymmetric Jacobian is *not* automatically a Poisson operator.
- Jacobi identity requires additional algebraic structure.
- In classical exponential families, this structure is absent.
- In quantum exponential families, it is intrinsic (via commutators).

### (iv) Global dynamics vs linearisation
- GENERIC structure in these papers arises **locally**, upon linearisation.
- Global Hamiltonian structure is a stronger condition and is not assumed
  in the classical case.

The original paper relies on these distinctions, but does not foreground them.
The companion paper makes them explicit.

---

## 4. What the Fisher-geometry companion shows

The companion paper repeats the inaccessible-game construction using:

- the *Fisher/BKM metric* as the dissipation geometry,
- natural-gradient entropy ascent,
- Fisher-orthogonal projection to enforce the same constraint.

The result:

- the constrained flow is different in detail,
- but *linearisation still yields a GENERIC-like decomposition*,
- with a symmetric entropy-producing sector and an antisymmetric
  entropy-conserving sector.

Therefore:

> The reversible structure does *not* disappear under natural gradients.

What changes is *interpretation*:

- Under Euclidean geometry, reversibility appears *emergent*:
  nothing in the geometry enforces it.
- Under Fisher geometry, reversibility appears *canonical*:
  the geometry already encodes dual affine structure.

The metric controls *how the structure is attributed*, not *whether it exists*.

---

## 5. Why the Euclidean formulation is still essential

The Fisher formulation is invariant, but it is not neutral.

Using Fisher geometry builds information-geometric structure into the dynamics
from the outset. This can obscure whether reversibility is imposed or derived.

The Euclidean formulation serves a different purpose:

- it strips the geometry to the minimum,
- avoids pre-imposing reversible structure,
- and demonstrates that antisymmetric dynamics arise *solely*
  from constraint enforcement.

The two papers therefore play complementary roles:

| Formulation | What it shows |
|------------|---------------|
| Euclidean | Reversibility can *emerge* from constraints alone |
| Fisher | Reversibility is *robust* under coordinate-invariant geometry |

Neither replaces the other.

---

## 6. How the quantum case fits

In the matrix exponential family, a further distinction appears:

- the operator algebra is noncommutative,
- the commutator defines a genuine Lie–Poisson structure,
- the antisymmetric sector becomes intrinsically Hamiltonian,
- Jacobi identity holds globally by construction.

Here the reversible structure is not merely emergent or canonical —
it is *forced* by the algebraic framework.

This explains why:

- classical antisymmetry is parameter-dependent and fragile,
- quantum antisymmetry is structural and stable.

---

## 7. How to read the papers

*Recommended order:*

1. *The Inaccessible Game*  
   — understand the axioms, the Euclidean construction, and emergent reversibility.

2. *Constraint-Induced Reversibility under Natural-Gradient Dynamics*  
   — see that the structure survives Fisher geometry and is not a coordinate artefact.

3. *The Origin of the Inaccessible Game* (quantum paper)  
   — see how noncommutativity forces a genuine Hamiltonian sector.

Each paper isolates a different logical layer of the same framework.

---

## 8. The takeaway

The inaccessible game is not about choosing the “right” metric.
It is about understanding *which structures are assumed,
which are enforced, and which are forced*.

- Metrics encode dissipation assumptions.
- Constraints encode protected information.
- Geometry determines attribution.
- Algebra determines inevitability.

The companion paper exists to make that separation explicit.
