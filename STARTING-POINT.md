# Starting Point — Chromium

This repository is a **forward-only fork-anchor** of upstream `chromium/chromium` from a chosen release tag, not a full-history mirror.

## Anchor

| Field | Value |
|---|---|
| Upstream | https://github.com/chromium/chromium |
| Anchor tag | `152.0.7947.0` |
| Upstream tag SHA | `18aeeb51dd7e909510d599bee93599bf91ef9ef9` |
| Anchor commit on `main` | re-rooted as orphan (single-commit anchor) |
| Reshape date | 2026-07-13 UTC |

## Why an anchor, not full history

Per `UPSTREAM-MERGE-DISCIPLINE.md`, this repository tracks upstream **forward from a chosen anchor**. History before the anchor lives at upstream and is not mirrored here. This keeps:

- the repository size proportionate to active work
- forward merges from upstream small and reviewable
- GitHub's per-file 100 MB and per-pack 2 GiB limits comfortably within reach

## How to bring in a new upstream release

1. Fetch the new upstream tag into this clone (fetched into `upstream` remote).
2. Create a merge or replacement anchor commit on `main`.
3. Merge `main` → `unicore` to bring upstream changes onto our additions.

See `UPSTREAM-MERGE-DISCIPLINE.md` for the full canonical procedure.

## Pre-anchor history

Pre-anchor history (every commit upstream produced before tag `152.0.7947.0`) is available at https://github.com/chromium/chromium and is not redundantly stored in this repository.
