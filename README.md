# vanedb-cpp has moved

This repository is **archived**. Development continues in the VaneDB monorepo:

### → [github.com/vanedb/vanedb](https://github.com/vanedb/vanedb) — in [`cpp/`](https://github.com/vanedb/vanedb/tree/main/cpp)

## Why

The Rust and C++ engines share one contract: the same distance semantics, the
same persistence format, and the same search-quality expectations. Keeping them
in separate repositories meant the same bug was filed, fixed, and reviewed
twice — the cosine and non-finite-ordering defects existed independently in
both engines before consolidation. They are now fixed once, against shared
fixtures in [`conformance/`](https://github.com/vanedb/vanedb/tree/main/conformance)
that both engines must satisfy.

## What moved

- **Code** — every file now lives under [`cpp/`](https://github.com/vanedb/vanedb/tree/main/cpp).
- **History** — imported commit by commit, not squashed. Old commit IDs map to
  new ones in [`docs/migration/vanedb-cpp-commit-map.txt`](https://github.com/vanedb/vanedb/blob/main/docs/migration/vanedb-cpp-commit-map.txt).
- **Issues** — transferred or consolidated into the monorepo tracker. Paired
  Rust/C++ bugs became a single issue labelled for both components.

Existing links keep working: GitHub redirects repository, issue, and commit
URLs. Nothing is deleted — this repository becomes read-only.
