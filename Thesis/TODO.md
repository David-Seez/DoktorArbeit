# Thesis TODO — Morse-Theoretic Construction of the AHSS

_Generated 2026-06-22. Tick boxes as you go; file:line refs point into the repo._

---

## 1. New chapter: Topological Preliminaries (state, don't prove)

Goal: pull all cited point-set / homotopy machinery into one forward chapter so the
proofs stay clean. Create `text/topologicalPreliminaries.tex`, `\include` after the
notation chapter in `main.tex`.

### A. Extension theorems (compact Hausdorff / normal)
- [ ] Tietze extension theorem            — used kTheory.tex:28
- [ ] Partitions of unity (finite covers) — used kTheory.tex:28, 315

### B. Mapping spaces / currying
- [ ] Compact-open topology (already defined, vectorBundles:296 — move here?)
- [ ] Exponential law / currying is a homeomorphism (compactly generated)
- [ ] Loop-suspension adjunction  [ΣX,Y]* ≅ [X,ΩY]*   — used kTheory.tex:1026

### C. Quotients / final topology / colimits
- [ ] Universal property of the quotient topology — used kTheory.tex:97, 700, 736
- [ ] Final/colimit topology (closed iff closed in each stage) — kTheory.tex:422, 950

### D. Cofibrations / HEP / NDR
- [ ] NDR ⟹ cofibration                         — used kTheory.tex:766
- [ ] Cofibration + contractible A ⟹ X→X/A h.e.  — used kTheory.tex:753

### E. Classical groups
- [ ] GL_n(C), U(n) path-connected            — used kTheory.tex:116, 241
- [ ] Gram-Schmidt retraction GL_n(C) ↘ U(n)  — used kTheory.tex:1021

### F. Compactness
- [ ] Tube lemma                                   — used kTheory.tex:58
- [ ] Compact subset of a colimit lands in a stage — used kTheory.tex:468 (currently self-proved)

### G. Spheres / smash
- [ ] S^n ≅ I^n/∂I^n and S^n ∧ S^m ≅ S^{n+m}   — used kTheory.tex:705

### H. Differential-topology inputs (decide: same chapter or own)
- [ ] Collar neighbourhood theorem    — used kTheory.tex:767
- [ ] Tubular neighbourhood theorem   — used kTheory.tex:767, orientation.tex
- [ ] ODE flow (existence/uniqueness/smoothness) — used vectorBundles:504

> Decision needed: items in **F** and the colimit closed-embedding lemmas
> (kTheory.tex:403-415, 467-481) are currently PROVED. Keep the proofs OR
> move to this chapter as cited facts — not both.

---

## 2. Bott periodicity (chapter stub: text/bottPeriodicity.tex)

- [ ] **Decide the route** (philosophy fork):
  - [ ] Proved centerpiece → elementary clutching proof (Atiyah §2 / Hatcher VBKT §2.1).
        Reuses your clutching machinery; ~8-15 pp; self-contained.
  - [ ] Required input only → 2-3 pp bridge: cite Milnor §23 / Mitra for ΩU ≃ Z×BU,
        then representability (§3.4) + loop-suspension adjunction ⟹ K̃(Σ²X) ≅ K̃(X).
  - [ ] (Do NOT half-prove the Morse version — long AND citing.)
- [ ] If Mitra route: add Milnor "Morse Theory" to the bibliography.
- [ ] Write the statement in the homotopy/representable form (matches §3.4).

---

## 3. Open math to finish / check

- [ ] `K̃(ΣX) ≅ [X,U]` proof (kTheory.tex:1004): nail the **based vs free**
      homotopy-class bookkeeping — keep clutching functions normalized at x₀.
- [ ] Fix closing sentence of `rem:kTheo-grothendieckEquivalence`:
      only Δ(A) ⊆ [overline(0,0)] is shown, NOT equality (equality needs
      cancellativity). Reword the "justifies the notation" line.
- [ ] K-theory as a cohomology theory — confirm the stated goals are all delivered:
  - [ ] Long exact sequence of a pair (Puppe)   (claimed goal, kTheory.tex:12)
  - [ ] Excision
  - [ ] Additivity (pointed sum)

---

## 4. Fixes & typos

- [ ] kTheory.tex:912 — "unitary goupf of rank n under the standart inclusions"
      → "unitary groups ... standard inclusion".
- [ ] kTheory.tex:705 — "$\R^n{+1}$" → "$\R^{n+1}$".
- [ ] Spell-check pass (recurring: "imidiatly", "becuse", "assignement",
      "Grothendiek", "standart", "kompact", "direkt", "homotopie").
- [ ] kTheory.tex:1016 — "$\C_+$" should be "$C_+$".

---

## 5. Remaining stub sections

- [ ] text/introduction.tex
- [ ] text/orientation.tex
- [ ] text/morseFiltration.tex
- [ ] text/spectralsequence
- [ ] Fill the two "Title" placeholder section headers (TOC entries 6 & 7).
