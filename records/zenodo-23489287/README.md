# Asymptotics of centered inverse-binomial moments: regimes, bounds and open questions (working note).

## Record of origin

This repository is a mirror of a Zenodo record. The Zenodo record is the record of origin;
cite it, not this repository.

All versions: [10.5281/zenodo.23489287](https://doi.org/10.5281/zenodo.23489287)

## Description

Working note on the asymptotics of the normalized centered inverse-binomial moment R(m,n) = 4^m A_m(n)/n^(2m), building on the author's paper "Centered inverse-binomial moments" (Zenodo). R tends to a finite limit for m < n/2, grows like n^(1/4) at m = n/2, and grows exponentially for m > n/2; the note gives results for every regime, including m much larger than n, many with explicit constants. Three files: the working note as of 18 October 2026 (unchanged from version 1); the first addendum recording later work (unchanged from version 1); and a second addendum (new in version 2) with an internal audit of the note's lemmas and theorems, a correction to one constant (Lemma 3: M2 = 0.0118455788..., previously stated as 0.0118453...; no result changes), and new limit laws for maximal and fixed points of surjective pistols. Every result is labelled proved, certified, formal, checked, or conjecture. None has yet been checked line by line by the author or an outside referee; the work is under review.

Method and credit. The earlier paper's results (the decomposition, the moment representation and the coefficient laws) were developed by three AI systems, Claude (Anthropic), Grok (xAI) and Gemini (Google), working in exchange with one another and proofreading one another's work, under the author's direction; the project began in a Grok session. The asymptotic results in this note and its addenda were developed in the same round-table process, principally with Claude, in which the author ran the sessions and relayed between the assistants, chose the problem and the questions, directed each stage, reviewed each step, and decided what was recorded and how each result is labelled. Results were tested against exact-arithmetic and interval-arithmetic scripts; agreement between AI systems was not treated as verification.

## Versions

Each Zenodo version is one commit and one git tag here.

| Version | Published | DOI |
|---|---|---|
| - | 2026-10-20 | [10.5281/zenodo.23489288](https://doi.org/10.5281/zenodo.23489288) |
| 2 | 2026-10-20 | [10.5281/zenodo.23504406](https://doi.org/10.5281/zenodo.23504406) |

## Files in the latest version

Fingerprint is the first 16 hex digits of SHA-256. Zenodo's own checksum was checked on download.

| File | Fingerprint | Bytes |
|---|---|---|
| `ADDENDUM_asymptotics_after_2026-10-18.pdf` | b1ff77729db3bcc5 | 282615 |
| `SECOND_ADDENDUM_after_2026-10-20.pdf` | ff62b6f1517ad424 | 125623 |
| `asymptotics_note.pdf` | 4635d7a620fff6b5 | 106758 |

## Mirror note

Made with zenodo_to_github.py (Loia Labs LLC). This repository is not switched on in
Zenodo's GitHub settings, so GitHub releases here do not create Zenodo records.
