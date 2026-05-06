# riskledger

`riskledger` keeps a focused SQL implementation around databases. The project goal is to analyze exposure buckets and settlement reconciliation.

## Use Case

I want this repository to be useful as a quick reading exercise: fixtures first, implementation second, verifier last.

## Riskledger Review Notes

`stale` and `edge` are the cases worth reading first. They show the optimistic and cautious ends of the fixture.

## Highlights

- `fixtures/domain_review.csv` adds cases for index fit and join width.
- `metadata/domain-review.json` records the same cases in structured form.
- `config/review-profile.json` captures the read order and the two review questions.
- `examples/riskledger-walkthrough.md` walks through the case spread.
- The SQL code includes a review path for `index fit` and `constraint risk`.
- `docs/field-notes.md` explains the strongest and weakest cases.

## Code Layout

The fixture data drives the tests. The code stays thin, while `metadata/domain-review.json` and `config/review-profile.json` explain what each case is meant to protect.

The SQL checks add a separate view over the domain review fixture.

## Run The Check

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File scripts/verify.ps1
```

## Regression Path

The check exercises the source code and the review fixture. `stale` is the high score at 211; `edge` is the low score at 144.

## Future Work

The fixture set is small enough to audit by hand. The next useful expansion is malformed input coverage, not extra surface area.
