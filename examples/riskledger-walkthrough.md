# Riskledger Walkthrough

The fixture is intentionally compact, so the review starts with the cases that pull farthest apart.

| Case | Focus | Score | Lane |
| --- | --- | ---: | --- |
| baseline | index fit | 185 | ship |
| stress | join width | 189 | ship |
| edge | constraint risk | 144 | ship |
| recovery | plan drift | 191 | ship |
| stale | index fit | 211 | ship |

Start with `stale` and `edge`. They create the widest contrast in this repository's fixture set, which makes them better review anchors than the middle cases.

The useful comparison is `index fit` against `constraint risk`, not the raw score alone.
