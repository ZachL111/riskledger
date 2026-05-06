# Review Journal

The repository goal stays the same: analyze exposure buckets and settlement reconciliation. This note explains the added review angle.

The local checks classify each case as `ship`, `watch`, or `hold`. That gives the project a small review vocabulary that matches its databases focus without claiming live deployment or external usage.

## Cases

- `baseline`: `index fit`, score 185, lane `ship`
- `stress`: `join width`, score 189, lane `ship`
- `edge`: `constraint risk`, score 144, lane `ship`
- `recovery`: `plan drift`, score 191, lane `ship`
- `stale`: `index fit`, score 211, lane `ship`

## Note

This file is intentionally plain so the fixture remains the source of truth.
