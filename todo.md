# Project checklist

## Completed

- [x] Apéry-set core — `relaxResidue`, `relaxRound`, `aperySet`, `frobeniusNumber`, `genusApery`
- [x] Supporting invariants — `gapsUpTo`, `genusUpTo`, `conductorUpTo`, `conductor`, `multiplicity`
- [x] Flagship elasticity theorem ρ(S) = nₖ/n₁ proved, zero sorries (14 theorems) — *removed from `ns-lean` 2026-09-15, unused in the paper; kept locally if the factorization-invariants work below gets picked back up*
- [x] Mathematical foundations — `Defs.lean`, `Factorization.lean` (also removed alongside the elasticity theorem, see above)
- [x] 45 machine-checked theorems in `PaperClaims.lean`, zero sorries
- [x] 10 of the audit-target papers audited across two categories
- [x] GAP cross-checks run for everything currently encoded
- [x] 6 discrepancies in 3 papers confirmed by two independent systems, logged in `discrepancies.md`

## To do

### Highest value

- [ ] Paste the small-generator-count theorem block (~35 theorems, 3 papers), then run GAP on those rows

### Library work

- [ ] Prove `frobeniusNumber` correct against `Generated`, connecting `Defs.lean` to `Basic.lean` (`Defs.lean` needs restoring from the local archive first — see above)
- [ ] Change small `native_decide` proofs to `decide` where possible to drop the extra axiom

### Longer term

- [ ] Obtain the paywalled Ramanujan J. repunit paper
- [ ] Replace the sweep with a priority queue (Dijkstra) — O(m·k·log m) instead of O(m²·k)
- [ ] Build factorization invariants (length sets, delta sets, elasticity) to unlock the remaining 9 papers
- [ ] Research the Mathlib PR process and write it up as `mathlib-contribution-notes.md`
- [ ] Decide whether and how to contact the authors of the flagged papers
- [ ] Get CI green on every push to `ns-lean`
- [ ] Begin the write-up

## Current weaknesses

### Formal guarantee

`Defs.lean` and `Basic.lean` are unconnected (and `Defs.lean` itself is no longer in `ns-lean` — see Completed, above). Lean proves `frobeniusNumber [5,13,21] = 37`, which is a fact about our code rather than about the semigroup. GAP agreement is strong empirical evidence, but the formal guarantee we advertise does not yet reach the mathematics.

### Verification

- No correctness proof for the Apéry implementation; the loop invariant is argued on paper only.
- All 45 audit proofs use `native_decide`, so every one carries the extra axiom, including small cases where `decide` would work.
- Lean and GAP both start from generator lists transcribed by hand from the papers, so a transcription error would fool both. This has happened once already.

### Performance

The sweep is O(m²·k). The largest audit case, with smallest generator 531,431, took several days to complete; might need more efficient sweep if we encounter larger cases