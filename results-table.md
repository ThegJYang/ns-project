| Paper | Claim | Generators | Paper says | Lean | GAP | Verdict |
|---|---|---|---|---|---|---|
| **arXiv:math/0606717** — Fibonacci | Thm 1.1, case 1a, (i,k)=(5,5) | 5, 13, 55 | F = 47 | pass | pass | ✅ |
| | Thm 1.1, case 1a, (i,k)=(3,6) | 2, 5, 34 | F = 3 | pass | pass | ✅ |
| | Thm 1.1, case 1b, (i,k)=(5,3) | 5, 13, 21 | F = 37 | pass | pass | ✅ |
| | Thm 1.1, case 1b, (i,k)=(7,6) | 13, 34, 233 | F = 356 | pass | pass | ✅ |
| | Thm 1.1, case 2, (i,k)=(11,6) | 89, 233, 1597 | F = 17512 | pass | pass | ✅ |
| | Cor 1.2, genus, (i,k)=(5,3) | 5, 13, 21 | g = 20 | pass | pass | ✅ |
| **arXiv:1510.04801** — generalized Thabit | Lem 4.9, n = 0 | 2, 11 | F = 9 | pass | pass | ✅ |
| | Lem 4.10, k = n | 17, 37, 77, 157, 317 | F = 337 | pass | pass | ✅ |
| | Cor 4.12, k = n−1 | 37, 77, 157, 317, 637, 1277 | F = 1551 | pass | pass | ✅ |
| | §4.2, 2 ≤ k < n, ex. 1 | 281, …, 73721 (9 gens) | F = 81483 | pass | pass | ✅ |
| | §4.2, 2 ≤ k < n, ex. 2 | 1145, …, 1179641 (11 gens) | F = 1325903 | pass | pass | ✅ |
| | §4.3, k > n | 29, 65, 137, 281, 569 | F = 1095 | pass | pass | ✅ |
| **arXiv:2306.10738** — generalized repunit | Thm 3.5, general family | 5, 13, 29 | F = 37 | pass | pass | ✅ |
| | Thm 3.5, genus | 5, 13, 29 | g = 20 | pass | pass | ✅ |
| | Thm 4.1, b=2, n=3, d=3 | 7, 17, 37 | F = 67 | pass | pass | ✅ |
| | Thm 4.1, genus | 7, 17, 37 | g = 38 | pass | pass | ✅ |
| | Cor 4.2, Frobenius, b=2, n=3 | 7, 15, 31 | F = 55 | pass | pass | ✅ |
| | **Cor 4.2, genus, b=2, n=3** | 7, 15, 31 | **g = 36** | **32** | **32** | **❌ D1** |
| **arXiv:2111.04899** — linear-recurrence tails | Cor 5.1 / Ex 5.2(1), a=3, n=3 | 13, 40, 121 | F = 350 | pass | pass | ✅ |
| | **Ex 5.2(2), n = 1** | 7, 22, 67, 202 | **F = 16** | **104** | **104** | **❌ D2** |
| | **Ex 5.2(2), n = 2** | 22, 67, 202, 607, 1822 | **F = 181** | **989** | **989** | **❌ D2** |
| | Ex 6.2, genus, n = 1 | 7, 22, 67, 202 | g = 54 | pass | pass | ✅ |
| | §5, (2ᵏ−1)2ⁿ−1, n=1, k=3 | 13, 27, 55, 111 | F = 207 | pass | pass | ✅ |
| | §5, k=1, n=1, a=3 | 5, 17, 53 | F = 48 | pass | pass | ✅ |
| | §5, k=1, n=2, a=3 | 17, 53, 161, 485 | F = 627 | pass | pass | ✅ |
| | §5, n=1, k=2, k ≤ a+1 | 23, 71, 215, 647 | F = 1125 | pass | pass | ✅ |
| | §5, n=1, k=5, k > a+1 | 725, …, 529253 (7 gens) | F = 1057773 | pass | pass | ✅ |
| | §5, n=2, k=5 — paper gives no closed form | 2177, …, 4763285 (8 gens) | — | 9504780 | 9504780 | ➖ |
| | **§5, k−2 ≥ (a−1)Rₙ, a=3, n=2, k=10** | 531431, …, 282424753511 (13 gens) | **F = 564839409633** | **564848975571** | — | **❌ D3** |
| **Ong–Ponomarenko** — geometric sequences | main thm, k = 1 (Sylvester) | 2, 3 | F = 1 | pass | pass | ✅ |
| | main thm, k = 2, m=2, n=3 | 4, 6, 9 | F = 11 | pass | pass | ✅ |
| | main thm, k = 3, m=2, n=3 | 8, 12, 18, 27 | F = 49 | pass | pass | ✅ |
| | main thm, k = 2, m=2, n=5 | 4, 10, 25 | F = 31 | pass | pass | ✅ |
| | symmetry check, m↔n | 9, 6, 4 | F = 11 | pass | pass | ✅ |
| **arXiv:1706.04378** — triangular & tetrahedral | Prop 6, triangular n odd | 6, 10, 15 | F = 29 | pass | pass | ✅ |
| | Prop 6, triangular n even | 10, 15, 21 | F = 89 | pass | pass | ✅ |
| | Prop 12.1, tetrahedral n ≡ 0 (6) | 56, 84, 120, 165 | F = 1243 | pass | pass | ✅ |
| | Prop 12.2, tetrahedral n ≡ 1 (6) | 84, 120, 165, 220 | F = 1571 | pass | pass | ✅ |
| | Prop 12.3, tetrahedral n ≡ 2 (6) | 120, 165, 220, 286 | F = 2619 | pass | pass | ✅ |
| | Prop 12.4, tetrahedral n ≡ 3 (6) | 165, 220, 286, 364 | F = 5059 | pass | pass | ✅ |
| | Prop 12.5, tetrahedral n ≡ 4 (6) | 20, 35, 56, 84 | F = 253 | pass | pass | ✅ |
| | Prop 12.6, tetrahedral n ≡ 5 (6) | 35, 56, 84, 120 | F = 853 | pass | pass | ✅ |
| **arXiv:2507.01898** — squares of Fibonacci | Cor 5.16.1 / Ex 5.17.3, n = 6 | 64, 169, 441 | F = 3522 | pass | pass | ✅ |
| | Cor 5.16.2 / Ex 5.17.2, n = 5 | 25, 64, 169 | F = 743 | pass | pass | ✅ |
| | Cor 5.16.3 / Ex 5.17.1, n = 4 | 9, 25, 64 | F = 130 | pass | pass | ✅ |
| | degenerate S(3), drops to 2 generators | 4, 9, 25 | F = 23 | pass | pass | ✅ |

## Discrepancies

Detail, corrected formulas, and diagnosis in `discrepancies.md`.

| | Paper | Location | Nature |
|---|---|---|---|
| D1 | arXiv:2306.10738 | Corollary 4.2 | Genus formula: `n−1` should read `n−2`. Contradicts the paper's own Theorem 4.1 and returns non-integers. |
| D2 | arXiv:2111.04899 | Example 5.2(2) | Final simplification wrong; the paper's own preceding line is correct. |
| D3 | arXiv:2111.04899 | §5, saturated sub-case | Closed form short by exactly `2a^(n+k+2)`, confirmed at k = 10, 11, 12. |