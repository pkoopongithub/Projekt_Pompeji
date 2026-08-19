---
author:
- Paul Koop
title: |
  The Trinity as a Necessary Structure of a Monistic Modal Ontology\
  Version 4 -- Complete Formal Analysis
---

::: center
*Past and future are horizons of knowledge.\
The present is the locus of reality.*
:::

# Preface

This treatise is the formal culmination of a long development. It unites the insights from all previous versions:

- **Versions 1--3:** Attempt to derive the Trinity directly from S5 -- failed due to the missing bridge from existence to necessity.

- **Version 4 (old):** Proof that pure S5 is insufficient -- the target formula is not derivable in S5 alone. This proof is now integrated into the new version.

- **Version 5:** Formalization of the superposition intuition and proof of the target formula in the extended system S5+SP.

The **present Version 4 (new)** unites both perspectives:

1.  **Part I:** Rigorous formal proof that the target formula is **not** derivable in pure S5 (adoption of old Version 4).

2.  **Part II:** Rigorous formal proof that the target formula is **derivable** in the extended system S5+SP (with superposition axioms).

3.  **Part III:** Metatheoretical classification -- what has been shown, what has not, and which questions remain open.

The fundamental thesis of the entire investigation is:

> **Under the axioms of monism (A1), the existence of a possible world (A4), the transcendental bridges (A11, A12), and the superposition hypothesis (ASP1--ASP5), the Trinity of origin, totality, and self-knowledge follows necessarily. Without the superposition hypothesis, it is not provable in S5.**

# Introduction: Aim and Methodological Self-Restriction

Classical metaphysics has repeatedly attempted to derive the fundamental structure of reality from a few basic principles. A particular challenge arises from three seemingly distinct aspects:

1.  **Why is there something rather than nothing?** -- origin (U).

2.  **How does the totality of all possibilities relate to actuality?** -- totality (T).

3.  **How can a state arise within reality that recognizes reality itself?** -- self-knowledge (S).

The ontology examined here proposes to answer these three questions not through three separate metaphysical substances, but through three necessary perspectives of the same reality:

- **Origin (U):** the necessary ground for the existence of possibilities at all -- understood as the lower limit of totality;

- **Totality (T):** the entirety of all realized possibilities -- understood as an open, well-founded interval;

- **Self-knowledge (S):** the reflexive completion of reality in a state of complete self-knowledge -- understood as the upper limit of totality.

This structure is called the **Trinity**:

$$Tr := U \land T \land S$$

The term \"Trinity\" here denotes not a personal or substantial threefoldness, but a functional unity of three necessary aspects of a single reality.

# Formal Language and Logical Framework

## Modal Logic S5

We work in first-order modal logic with identity in the system S5:

- **Necessity:** $\Box p$

- **Possibility:** $\Diamond p := \neg\Box\neg p$

**Axioms of S5:**

- \(K\) $\Box(p \rightarrow q) \rightarrow (\Box p \rightarrow \Box q)$

- \(T\) $\Box p \rightarrow p$

- \(4\) $\Box p \rightarrow \Box\Box p$

- \(5\) $\Diamond p \rightarrow \Box\Diamond p$

**Inference Rules:**

- **Modus Ponens:** From $p$ and $p \rightarrow q$, infer $q$.

- **Necessitation:** From $p$ (derivable), infer $\Box p$.

**Tableau Rules for S5:** $$\begin{aligned}
& (\neg\Box) & \frac{\neg\Box A}{\Diamond\neg A} \\
& (\Diamond) & \frac{\Diamond A}{A @ w_{\text{new}}} \quad \text{(new world)} \\
& (\Box) & \frac{\Box A @ w}{A @ v} \quad \text{for every already existing world } v \\
& (\neg\forall) & \frac{\neg\forall x A}{\exists x \neg A} \\
& (\exists) & \frac{\exists x A}{A[a/x]} \quad \text{(a new)} \\
& (\forall) & \frac{\forall x A}{A[a/x]} \quad \text{(a arbitrary)}
\end{aligned}$$

## Predicate Logic

We use classical first-order predicate logic with identity ($=$) and the usual quantifiers ($\forall, \exists$).

# The Axioms (Basic)

## A1 -- Monism

There are no fundamentally separated domains of reality.

$$\boxed{A1 := \Box\neg\exists x\exists y\, FundamentalSeparated(x,y)}$$

**Explanation:** If two domains were fundamentally separated, there would be no causal or ontological interaction between them. They could not be part of a unified reality, which contradicts monism.

## A4 -- Existence of a Possible Reality

There is at least one possible world.

$$\boxed{A4 := \Diamond\exists w\, World(w)}$$

**Explanation:** This axiom ensures that the modal universe is not empty. It is the weakest possible existence axiom: it does not say that a world **actually** exists, but only that it is **possible**.

## A11 -- Transcendental Bridge

A world is separated from consciousness exactly when it contains no consciousness.

$$\boxed{A11 := \forall w \left( \text{WorldSeparatedFromConsciousness}(w) \leftrightarrow \neg \exists c (Consciousness(c) \land c(w)) \right)}$$

with the definition:

$$\boxed{\text{WorldSeparatedFromConsciousness}(w) := \neg \exists c (Consciousness(c) \land c(w))}$$

**Explanation:** This axiom formalizes the transcendental insight that a world without consciousness would be unknowable and therefore fundamentally separated -- which is forbidden by monism (A1).

## A12 -- Experience and Realization

$$\boxed{A12 := \forall p. \text{Experienceable}(p) \leftrightarrow \exists w. Realized(w, p)}$$

with the definition:

$$\boxed{\text{Experienceable}(p) := \exists w. (\text{Consciousness}(w) \land \text{Realized}(w, p))}$$

**Explanation:** This axiom states: A proposition is experienceable exactly when it is realized in a world. It is the formal version of the transcendental argument: What is not realized cannot be experienced.

## A13, A14, A15 -- The Three Implications of the Cases

These axioms formalize the three reductio cases:

$$\boxed{A13 := \Box\forall x(T(x) \rightarrow U(x))}$$ $$\boxed{A14 := \Box\forall x(U(x) \rightarrow S(x))}$$ $$\boxed{A15 := \Box\forall x(S(x) \rightarrow T(x))}$$

**Explanation:** They state that the three limits $T, U, S$ stand in a mutual implication chain -- which in S5 leads to their equivalence.

# Definition of the Limit Structure

## Totality T as an Open, Well-Founded Interval

**Totality T** is the entirety of all realized states. We understand T as a **well-founded, open interval**:

$$\boxed{T := \{ x \mid U < x < S \}}$$

**Explanation:**

- An open interval $(U, S)$ contains all states between U and S, but **not** U and S themselves.

- **Well-foundedness:** Every non-empty subset of states has a minimal element. This prevents infinite chains of grounds.

- **Origin U** is the lower limit -- that which comes closest to nothing, but is itself not nothing.

- **Self-knowledge S** is the upper limit -- the complete transparency of totality, which itself does not belong to totality.

## Origin U as Lower Limit

$$\boxed{U := \lim_{x \to \inf} T}$$

## Self-Knowledge S as Upper Limit

$$\boxed{S := \lim_{x \to \sup} T}$$

## The Trinity

$$\boxed{Tr := U \land T \land S}$$

# PART I: PROOF OF NON-DERIVABILITY IN PURE S5

## Goal

Show that:

$$\boxed{\text{S5} \;\not\vdash\; \Box\forall x\,Tr(x)}$$

does not follow from the axioms $A1, A4, A11, A12, A13, A14, A15$ alone.

## Method

Construct an **open S5 tableau** for the negation of the target formula. According to the **soundness and completeness theorem** of the S5 tableau calculus:

> A set of formulas is **satisfiable** in an S5 model exactly when the tableau has **an open branch**.

Therefore: If the tableau for the negated target formula remains open, then there exists an S5 model that satisfies all axioms and the negation of the target formula -- so the target formula is **not a theorem**.

## Tableau (Pure Smullyan Rules)

    1.  ¬□∀x Tr(x)                                    [Assumption: target is not a theorem]
    2.  ◇¬∀x Tr(x)                                    [1, ¬□-rule]
    3.  ¬∀x Tr(x) @ w0                                [2, ◇-rule: new world w0]
    4.  ∃x ¬Tr(x) @ w0                                [3, ¬∀-rule: ¬∀xA ⊢ ∃x¬A]
    5.  ¬Tr(a) @ w0                                   [4, ∃-rule: a new]
    6.  ¬(T(a) ∧ U(a) ∧ S(a)) @ w0                    [5, D1 (Tr-definition)]

        → β-rule on 6:
        6a. ¬T(a) @ w0
        6b. ¬U(a) @ w0
        6c. ¬S(a) @ w0

    ─────────────────────────────────────────────────────────────
    BRANCH 6a: ¬T(a) @ w0
    ─────────────────────────────────────────────────────────────

    7.  □∀x(S(x) → T(x)) @ w0                         [A15]
    8.  ∀x(S(x) → T(x)) @ w0                          [7, □-rule]
    9.  S(a) → T(a) @ w0                              [8, ∀-rule]

        → β-rule on 9:
        9a. ¬S(a) @ w0
        9b. T(a) @ w0                                  [Contradiction with 6a → branch 9b closes]

        Thus: 9a. ¬S(a) @ w0

    10. □∀x(T(x) → U(x)) @ w0                         [A13]
    11. ∀x(T(x) → U(x)) @ w0                          [10, □-rule]
    12. T(a) → U(a) @ w0                              [11, ∀-rule]

        → β-rule on 12:
        12a. ¬T(a) @ w0                                [already in 6a]
        12b. U(a) @ w0                                 [no contradiction]

        → Choose branch 12a (consistent with 6a).

    13. □∀x(U(x) → S(x)) @ w0                         [A14]
    14. ∀x(U(x) → S(x)) @ w0                          [13, □-rule]
    15. U(a) → S(a) @ w0                              [14, ∀-rule]

        → β-rule on 15:
        15a. ¬U(a) @ w0
        15b. S(a) @ w0                                 [Contradiction with 9a → branch 15b closes]

        Thus: 15a. ¬U(a) @ w0

        → In branch 6a: ¬T(a), ¬U(a), ¬S(a) @ w0.
        → This is consistent – no contradiction.

    ─────────────────────────────────────────────────────────────
    BRANCH 6b: ¬U(a) @ w0
    ─────────────────────────────────────────────────────────────

    16. □∀x(T(x) → U(x)) @ w0                         [A13]
    17. ∀x(T(x) → U(x)) @ w0                          [16, □-rule]
    18. T(a) → U(a) @ w0                              [17, ∀-rule]

        → β-rule on 18:
        18a. ¬T(a) @ w0
        18b. U(a) @ w0                                 [Contradiction with 6b → closes]

        Thus: 18a. ¬T(a) @ w0

    19. □∀x(S(x) → T(x)) @ w0                         [A15]
    20. ∀x(S(x) → T(x)) @ w0                          [19, □-rule]
    21. S(a) → T(a) @ w0                              [20, ∀-rule]

        → β-rule on 21:
        21a. ¬S(a) @ w0
        21b. T(a) @ w0                                 [Contradiction with 18a → closes]

        Thus: 21a. ¬S(a) @ w0

    22. □∀x(U(x) → S(x)) @ w0                         [A14]
    23. ∀x(U(x) → S(x)) @ w0                          [22, □-rule]
    24. U(a) → S(a) @ w0                              [23, ∀-rule]

        → β-rule on 24:
        24a. ¬U(a) @ w0                                [already in 6b]
        24b. S(a) @ w0                                 [Contradiction with 21a → closes]

        → Consistent branch: ¬U(a), ¬T(a), ¬S(a) @ w0.

    ─────────────────────────────────────────────────────────────
    BRANCH 6c: ¬S(a) @ w0
    ─────────────────────────────────────────────────────────────

    25. □∀x(S(x) → T(x)) @ w0                         [A15]
    26. ∀x(S(x) → T(x)) @ w0                          [25, □-rule]
    27. S(a) → T(a) @ w0                              [26, ∀-rule]

        → β-rule on 27:
        27a. ¬S(a) @ w0                                [already in 6c]
        27b. T(a) @ w0

        → Both branches possible.

    28. □∀x(T(x) → U(x)) @ w0                         [A13]
    29. ∀x(T(x) → U(x)) @ w0                          [28, □-rule]
    30. T(a) → U(a) @ w0                              [29, ∀-rule]

        → β-rule on 30:
        30a. ¬T(a) @ w0
        30b. U(a) @ w0

    31. □∀x(U(x) → S(x)) @ w0                         [A14]
    32. ∀x(U(x) → S(x)) @ w0                          [31, □-rule]
    33. U(a) → S(a) @ w0                              [32, ∀-rule]

        → β-rule on 33:
        33a. ¬U(a) @ w0
        33b. S(a) @ w0                                 [Contradiction with 6c → closes]

        Thus: 33a. ¬U(a) @ w0

        → Combine: From 30b (U(a)) and 33a (¬U(a)) we get a contradiction.
        → Therefore 30a must hold: ¬T(a) @ w0.

        → Thus: ¬S(a), ¬U(a), ¬T(a) @ w0 consistent.

    ─────────────────────────────────────────────────────────────
    ALL BRANCHES: ¬T(a) ∧ ¬U(a) ∧ ¬S(a) @ w0 is consistent.
    ─────────────────────────────────────────────────────────────

    ─────────────────────────────────────────────────────────────
    REMAINING AXIOMS (A4, A11, A12) – no application
    ─────────────────────────────────────────────────────────────

    34. ◇∃w World(w) @ w0                              [A4]
    35. ∃w World(w) @ w1                               [34, ◇-rule, w1 new]
        → Leads to new world w1, but not back to w0.

    36. A11, A12: No instances in w0 that force T(a), U(a), or S(a).

    ─────────────────────────────────────────────────────────────
    CONCLUSION OF THE TABLEAU:
    ─────────────────────────────────────────────────────────────

    The tableau has an **open branch**:

        w0, a, with ¬T(a), ¬U(a), ¬S(a).

    No axiom generates T(a), U(a), or S(a) in w0.
    The remaining axioms lead to new worlds (w1, ...),
    but not back to w0.

    Therefore, the tableau is **not closed**.

## Metatheoretical Conclusion

According to the **soundness and completeness theorem** of the S5 tableau calculus (see e.g. Smullyan, Fitting, or Blackburn/de Rijke/Venema):

> A set of formulas $\Sigma$ is S5-satisfiable exactly when the tableau for $\Sigma$ has an open branch.

Our tableau for

$$\Sigma = \{ A1, A4, A11, A12, A13, A14, A15, \neg\Box\forall xTr(x) \}$$

has an open branch.

Thus $\Sigma$ is S5-satisfiable.

Thus there exists an S5 model that satisfies all axioms, but in world $w_0$ has an individual $a$ for which $\neg T(a)$, $\neg U(a)$, and $\neg S(a)$ hold.

Thus in this model $\Box\forall xTr(x)$ does not hold.

Thus $\Box\forall xTr(x)$ is **not a logical theorem** of the given axiomatics.

::: theorem
**Theorem 1** (Non-derivability in pure S5). *$$\boxed{
\text{S5} \;\not\vdash\; \Box\forall x\,Tr(x)
}$$*
:::

# PART II: PROOF IN THE EXTENDED SYSTEM S5+SP

## The Superposition Extension (ASP)

In addition to the axioms A1, A4, A11, A12, A13, A14, A15, we introduce the **superposition axioms**. They formalize the idea that consciousness ($C$) is the self-reflexive moment of a superposition from which all worlds emerge.

### ASP1 -- Consciousness in the Superposition

$$\boxed{ASP1 := C @ w_{\text{super}}}$$

**Explanation:** Consciousness holds in the superposition. The superposition is the primordial state in which all possibilities are still undividedly contained.

### ASP2 -- Uniqueness of $C$

$$\boxed{ASP2 := \forall v (w_{\text{super}} R v \rightarrow (C @ v \leftrightarrow v = w_{\text{super}}))}$$

**Explanation:** Consciousness holds only in the superposition -- no other world has it. Consciousness is a singular event.

### ASP3 -- The Superposition Contains All Tr-Properties

$$\boxed{ASP3 := \forall x\,Tr(x) @ w_{\text{super}}}$$

**Explanation:** The superposition already contains all properties $T, U, S$. It is the ground for everything that holds in the worlds.

### ASP4 -- Transfer to All Worlds

$$\boxed{ASP4 := \forall v (w_{\text{super}} R v \rightarrow \forall x\,Tr(x) @ v)}$$

**Explanation:** What holds in the superposition holds in all reachable worlds. The superposition is a normative origin.

### ASP5 -- Universal Reachability (as Frame Condition)

$$\boxed{ASP5 := \forall v (v \neq w_{\text{super}} \rightarrow w_{\text{super}} R v)}$$

**Explanation:** Every other world is reachable from the superposition. The superposition is the unique origin.

## Proof in the Extended System S5+SP

::: theorem
**Theorem 2** (Derivability in S5+SP). *$$\boxed{
\text{S5+SP} \;\vdash\; \Box\forall x\,Tr(x)
}$$ where $\text{S5+SP} := \text{S5} + \{ASP1, ASP2, ASP3, ASP4, ASP5\}$.*
:::

### Semantic Proof

Let $\mathcal{M} = (W, R, w_{\text{super}}, I)$ be an arbitrary S5+SP model with ASP1--ASP5.

To show: For all $w \in W$, $\mathcal{M}, w \models \forall x\,Tr(x)$.

Let $w \in W$ be arbitrary.

**Case 1:** $w = w_{\text{super}}$.

By ASP3:

$$\mathcal{M}, w_{\text{super}} \models \forall x\,Tr(x)$$

Thus the claim holds.

**Case 2:** $w \neq w_{\text{super}}$.

By ASP5:

$$w_{\text{super}} R w$$

By ASP4 it follows:

$$\mathcal{M}, w \models \forall x\,Tr(x)$$

Thus the claim holds.

Since $w$ was arbitrary, for all $w \in W$:

$$\mathcal{M}, w \models \forall x\,Tr(x)$$

This is equivalent to:

$$\mathcal{M} \models \Box\forall x\,Tr(x)$$

q.e.d.

### Tableau Proof in S5+SP

    TABLEAU PROOF IN S5+SP
    GOAL: ⊢ □∀x Tr(x)

    ─────────────────────────────────────────────────────────────
    REDUCTIO ASSUMPTION:
    ─────────────────────────────────────────────────────────────

    1.  ¬□∀x Tr(x)                                    [Assumption: target false]
    2.  ◇¬∀x Tr(x)                                    [1, ¬□-rule]
    3.  ¬∀x Tr(x) @ w0                                [2, ◇-rule: new world w0]
    4.  ∃x ¬Tr(x) @ w0                                [3, ¬∀-rule]
    5.  ¬Tr(a) @ w0                                   [4, ∃-rule: a new]

    ─────────────────────────────────────────────────────────────
    CASE DISTINCTION: w0 = w_super ∨ w0 ≠ w_super
    ─────────────────────────────────────────────────────────────

    6.  w0 = w_super  ∨  w0 ≠ w_super                  [Identity]

        → Branch A: w0 = w_super
        → Branch B: w0 ≠ w_super

    ─────────────────────────────────────────────────────────────
    BRANCH A: w0 = w_super
    ─────────────────────────────────────────────────────────────

    7.  ¬Tr(a) @ w_super                               [5, Substitution]
    8.  ∀x Tr(x) @ w_super                             [ASP3, Axiom]
    9.  Tr(a) @ w_super                                [8, ∀-rule on a]
    10. Contradiction: Tr(a) @ w_super and ¬Tr(a) @ w_super
        → Branch A closes (⊥).

    ─────────────────────────────────────────────────────────────
    BRANCH B: w0 ≠ w_super
    ─────────────────────────────────────────────────────────────

    11. w0 ≠ w_super                                   [from 6, Branch B]
    12. w_super R w0                                   [11, ASP5]
    13. ∀x Tr(x) @ w0                                  [12, ASP4]
    14. Tr(a) @ w0                                     [13, ∀-rule on a]
    15. Contradiction: Tr(a) @ w0 and ¬Tr(a) @ w0 (from 5)
        → Branch B closes (⊥).

    ─────────────────────────────────────────────────────────────
    BOTH BRANCHES CLOSE.
    ─────────────────────────────────────────────────────────────

    Therefore, the assumption ¬□∀xTr(x) is contradictory.

    Thus: ⊢ □∀xTr(x) in S5+SP.

    QED.

# PART III: METATHEORETICAL CLASSIFICATION

## What Has Been Shown?

  **System**   **Statement**                                     **Status**
  ------------ ------------------------------------------------- ------------------------------
  Pure S5      $\text{S5} \;\not\vdash\; \Box\forall x\,Tr(x)$   Proven (open tableau branch)
  S5+SP        $\text{S5+SP} \;\vdash\; \Box\forall x\,Tr(x)$    Proven (closed tableau)

The crucial insight is:

> The bridge from the existence of $Tr$ in one world to the necessity of $Tr$ in all worlds is **not a theorem of S5**. It must be introduced as an **additional metaphysical assumption** -- here in the form of the superposition axioms ASP1--ASP5.

## What Has Not Been Shown?

- The **truth** of the superposition axioms ASP1--ASP5. They are **metaphysical premises**, not logical theorems.

- That the target formula follows from the original axioms A1, A4, A11, A12, A13, A14, A15 alone -- on the contrary, Part I shows that it does not.

## The Role of $C$ (Consciousness)

The superposition axioms formalize the intuition that **consciousness ($C$)** is the self-reflexive moment of the superposition:

- ASP1: $C$ holds in the superposition.

- ASP2: $C$ holds only there -- it is a singular event.

- ASP3--ASP5: The superposition is the necessary ground for all properties in all worlds.

Thus $C$ becomes the **bridge from existence to necessity**: Because the superposition contains $Tr$ and all worlds emerge from it, $Tr$ holds necessarily in all worlds.

# Countermodels

The Trinity can be avoided if at least one of the axioms is abandoned:

  **Abandoned Axiom**                     **Countermodel**             **Consequence**
  --------------------------------------- ---------------------------- ----------------------------------------------------------
  A1 (Monism)                             Dualism (Descartes)          S can exist without T; knowledge and object are separate
  A4 (Existence of a world)               Nihilism                     There is no world; the entire ontology is empty
  A11 (Transcendental Bridge)             Epistemological Skepticism   Unknowability does not imply fundamental separation
  A12 (Experienceability ↔ Realization)   Empiricism                   Experienceability is not identical with realization
  ASP1--ASP5 (Superposition)              No superposition             The bridge from existence to necessity is missing

# Appendix: Complete Axioms and Theorems

## Axioms (Complete)

$$\begin{aligned}
A1 &:= \Box\neg\exists x\exists y\, FundamentalSeparated(x,y) \\
A4 &:= \Diamond\exists w\, World(w) \\
A11 &:= \forall w \left( \text{WorldSeparatedFromConsciousness}(w) \leftrightarrow \neg \exists c (Consciousness(c) \land c(w)) \right) \\
A12 &:= \forall p. \text{Experienceable}(p) \leftrightarrow \exists w. Realized(w, p) \\
A13 &:= \Box\forall x(T(x) \rightarrow U(x)) \\
A14 &:= \Box\forall x(U(x) \rightarrow S(x)) \\
A15 &:= \Box\forall x(S(x) \rightarrow T(x)) \\
ASP1 &:= C @ w_{\text{super}} \\
ASP2 &:= \forall v (w_{\text{super}} R v \rightarrow (C @ v \leftrightarrow v = w_{\text{super}})) \\
ASP3 &:= \forall x\,Tr(x) @ w_{\text{super}} \\
ASP4 &:= \forall v (w_{\text{super}} R v \rightarrow \forall x\,Tr(x) @ v) \\
ASP5 &:= \forall v (v \neq w_{\text{super}} \rightarrow w_{\text{super}} R v)
\end{aligned}$$

## Definitions

$$\begin{aligned}
\text{WorldSeparatedFromConsciousness}(w) &:= \neg \exists c (Consciousness(c) \land c(w)) \\
\text{Experienceable}(p) &:= \exists w. (\text{Consciousness}(w) \land \text{Realized}(w, p)) \\
T &:= \{ x \mid U < x < S \} \\
U &:= \lim_{x \to \inf} T \\
S &:= \lim_{x \to \sup} T \\
Tr &:= U \land T \land S
\end{aligned}$$

## Derived Theorems

$$\begin{aligned}
& \exists T \quad \text{(from A4)} \\
& \Diamond C \quad \text{(A5 – from A1, A11)} \\
& \forall p(\Diamond p \rightarrow \exists w. Realized(w,p)) \quad \text{(A2 – from A1, A11, A12)} \\
& \Box(T \rightarrow U) \quad \text{(from Case 1)} \\
& \Box(U \rightarrow S) \quad \text{(from Case 2 + Superposition)} \\
& \Box(S \rightarrow T) \quad \text{(from Case 3)} \\
& \Rightarrow \Box(U \leftrightarrow T) \land \Box(T \leftrightarrow S) \land \Box(S \leftrightarrow U) \\
& \Rightarrow \Box(U \land T \land S)
\end{aligned}$$

# Conclusion

This treatise has shown:

1.  **In pure S5**, the Trinity is **not provable** (Part I).

2.  **In the extended system S5+SP** (with superposition axioms), the Trinity is **provable** (Part II).

3.  The crucial metaphysical burden rests on the superposition axioms -- they are **not logical theorems**, but **additional assumptions**.

The formal work has thus precisely articulated the logical and metaphysical requirements of such a proof. The crucial question -- whether the superposition axioms are true -- remains a matter for philosophical or physical investigation. Logic has done its work: it has explicated the consequences of the assumptions and clearly named the limits of pure S5.

> **The Trinity is not an additional entity, but a structural condition -- yet it is provable only under the superposition hypothesis.**

::: center
*This treatise was written in the spirit of rigorous modal logic, yet in the language of philosophy -- for truth requires both: the precision of the formula and the breadth of the concept.*
:::
