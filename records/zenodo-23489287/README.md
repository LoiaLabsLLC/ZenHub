# Asymptotics of centered inverse-binomial moments: regimes, bounds and open questions (working note)

## Record of origin

This repository is a mirror of a Zenodo record. The Zenodo record is the record of origin;
cite it, not this repository.

All versions: [10.5281/zenodo.23489287](https://doi.org/10.5281/zenodo.23489287)

## Description

This record contains the working note "Asymptotics of centered inverse-binomial moments: regimes, bounds and open questions", version 4 (21 November 2026). Versions 1, 2 and 3 (doi:10.5281/zenodo.23489288, doi:10.5281/zenodo.23504406, doi:10.5281/zenodo.23535132) carry the note of 18 October 2026 unchanged, together with three addenda; version 4 is a full revision of the note itself, and the addenda remain in those records. Not independently refereed. The scripts, logs and proof texts are in the companion code record doi:10.5281/zenodo.24431534.

STATEMENT

The normalized moment R(m,n) = 4^m A_m(n)/n^(2m) of the centered inverse-binomial sums changes behaviour at m = n/2: below it R tends to a finite limit, at it R grows like n^(1/4), and above it R grows exponentially in n. The note gives results for every regime: below, at and above the transition, across it, and for m much larger than n, many with explicit two-sided bounds valid for every n. The main tool is the weight |Γ(y+it)|², the symmetric Meixner (generalized hyperbolic secant) law, with y = (n+2)/2.

MOTIVATION

The main paper (doi:10.5281/zenodo.23325629) writes S_m(n) = A_m(n)U_n + B_m(n) and represents A_m(n) as a moment of |Γ(y+ix)|². This note asks how A_m(n) grows in every joint regime of m and n, and how firmly each answer is known. We have not found these results for these moments in the literature or in a direct search of zbMATH Open; MathSciNet has not been searched.

STATUS

Lemma 1 (two-sided bound on the weight): Proved, explicit.
Lemma 2′ (error of the Stirling form of the weight, between −w²/(3(n+2)(w²+(1+2/n)²)) − min(2w², 3/4)/n² and 0): Proved, explicit (new in version 4).
Lemma 3 (uniform Stirling form with Binet constants; M₂ corrected to 0.0118455788…): Proved, explicit.
Lemma 3″ (−2y³/(3t³) ≤ η′ ≤ 0 for y ≥ 2, t ≥ max(5y, 20)): Proved (new in version 4).
Theorem 1 (θ = m/n < 1/2: R → (1 − 2θ)^(−1/2)): Proved, explicit domination; its 1/n and 1/n² terms: Proved, constant not explicit (new in version 4; was Heuristic).
Theorem 2 (θ = 1/2: R ~ C n^(1/4), C = 1.131876): Proved, explicit bounds for even n ≥ 10.
Theorem 3 (rate (1/n) ln R → φ(θ) within (ln n + C₂(θ))/n): Proved, explicit.
Theorem 4 (θ > 1/2: R = K(θ) e^(nφ(θ))(1 + O(1/n))): Proved (cites a standard Laplace theorem).
Theorem 5 (Theorem 4 uniform in θ ≥ θ₀ > 1/2; ratio law for A_m/h_m): Proved, constant not explicit (was Sketch).
Theorem 6 (fixed n, m → ∞): Proved.
Theorem 7 (m ≥ n²: A_m/h_m = 1 + π²n²/(16m) + O(n⁴/m²)): Proved, explicit for n ≥ 4.
Theorem 8 (m ~ λn²: A_m/h_m → e^(π²/(16λ))): Proved, constants omitted.
Theorem 9 (Gamma-model formula for A_m/h_m): Proved, computer-assisted (102,747 certified boxes, replicated by an independent implementation and on a second machine).
Theorem 10 (m = n/2 + x√n: R/(C n^(1/4)) → F(x), a parabolic cylinder function): Proved, no rate (was Conjecture 1 in version 1).
Theorem U (uniform expansion across θ = 1/2): Conditional on written but unreviewed arguments; its interval bounds are in doi:10.5281/zenodo.24426089.
The constant c₁(0) = 0.910691 in Theorem 2's correction: Heuristic.
Every new section was read by the author on 21 November 2026. No proof has yet been checked by an independent mathematician.

RESULTS

Bounds on the weight (Lemmas 1, 2′, 3, 3″); the three regimes θ < 1/2, θ = 1/2, θ > 1/2 (Theorems 1 to 5, including the new proof of the 1/n and 1/n² terms and the new proof of Theorem 5); m much larger than n (Theorems 6 to 9); the crossover at the transition (Theorem 10); and the conditional uniform expansion (Theorem U). New in version 4: a section "How the results were found", which shows in five steps how each result was reached (exact values from the recursion, the exponent Ψ, the w²/w⁴ expansion (θ − 1/2)w² + (1/12 − θ/2)w⁴ behind Theorems 1 to 4 and 10, the Gamma-law picture behind Theorems 6 to 9, and testing before proving); the secant identity Σ h_m u^(2m)/(2m)! = sec(u/2)^(n+2), proved; and "Worked by hand", sixteen blocks W1 to W16 that redo Lemmas 1, 2′ and 3 and Theorems 1 to 10 with pencil-sized numbers, each with a case that must fail. Two errors found since version 1 are corrected: the constant M₂ in Lemma 3, and a gap in the proof of Theorem 6 for n ≤ 3.

FILES

The note, asymptotics_note_v4_42ac618cc7c5fe93.pdf (33 pages). The code record, doi:10.5281/zenodo.24431534, holds asymptotics_code_record_892de09ffa95a21d.zip (SHA-256 beginning 892de09ffa95a21d; SHA256SUMS.txt lists 92 files) under the MIT licence: the fourteen scripts of the 18 October note, the checks written for version 4 with their mutation tests (27, 85, 20 and 15 checks in exact arithmetic), the Theorem 9 box list with its reference verifier and an independent re-implementation, the Theorem 5 scripts and written proof, the Lemma 3 audit, the review checks of 15 November 2026, the written proof of the 1/n terms, and the logs of the reruns of 21 November 2026 on two machines. Every script in it has been run on one machine or the other.

AI ASSISTANCE

The work was directed by the author. Most of the computational work was done with Claude (Anthropic) and Gemini (Google), with support from Grok (xAI). The text was drafted with AI assistance from the project's records and edited by the author, who takes responsibility for its contents.

REFERENCES

J. W. Davis, Centered inverse-binomial moments: polynomial decomposition, continuous dual Hahn moments, and non-holonomicity, Zenodo, doi:10.5281/zenodo.23325629. J. W. Davis, Interval-arithmetic bounds for the Taylor-remainder constants of a uniform expansion of centred inverse-binomial moments (Theorem U, K = 1, 2), Zenodo, doi:10.5281/zenodo.24426089. W. L. Harkness and M. L. Harkness, Generalized hyperbolic secant distributions, J. Amer. Statist. Assoc. 63 (1968), 329–337. X.-S. Jin and R. Wong, Uniform asymptotic expansions for Meixner polynomials, Constr. Approx. 14 (1998), 113–150. X. Li and R. Wong, On the asymptotics of the Meixner–Pollaczek polynomials and their zeros, Constr. Approx. 17 (2001), 59–90. E. Marciniak and J. Wesołowski, Asymptotic Eulerian expansions for binomial and negative binomial reciprocals, Proc. Amer. Math. Soc. 127 (1999), 3329–3338. J. Meixner, J. London Math. Soc. 9 (1934), 6–13. C. N. Morris, Natural exponential families with quadratic variance functions, Ann. Statist. 10 (1982), 65–80. The full list, with which entries were checked at the source, is in the note.

## Versions

Each Zenodo version is one commit and one git tag here.

| Version | Published | DOI |
|---|---|---|
| - | 2026-10-20 | [10.5281/zenodo.23489288](https://doi.org/10.5281/zenodo.23489288) |
| 2 | 2026-10-20 | [10.5281/zenodo.23504406](https://doi.org/10.5281/zenodo.23504406) |
| 3 | 2026-10-21 | [10.5281/zenodo.23535132](https://doi.org/10.5281/zenodo.23535132) |
| 4 | 2026-11-22 | [10.5281/zenodo.24431735](https://doi.org/10.5281/zenodo.24431735) |

## Files in the latest version

Fingerprint is the first 16 hex digits of SHA-256. Zenodo's own checksum was checked on download.

| File | Fingerprint | Bytes |
|---|---|---|
| `asymptotics_note_v4_42ac618cc7c5fe93.pdf` | 42ac618cc7c5fe93 | 734751 |

## Mirror note

Made with zenodo_to_github.py (Loia Labs LLC). This repository is not switched on in
Zenodo's GitHub settings, so GitHub releases here do not create Zenodo records.
