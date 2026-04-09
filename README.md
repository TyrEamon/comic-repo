# ImageMaster External Source Repo

This repository is the clean external source repository for `ImageMaster`.

Current state:
- the repo is intentionally kept minimal
- no Miru-imported manga sources are enabled by default
- only the directory structure and index format are kept

Recommended workflow:
1. Pick a Miru source that is confirmed usable.
2. Convert or rewrite it into the ImageMaster source format.
3. Add the new manifest and script into `sources/`.
4. Update `sources/index.json`.
5. Push changes, then sync the source repo from ImageMaster.

Repository layout:

```text
sources/
  index.json
  miru/
  scripts/
```

Notes:
- `sources/index.json` controls which sources ImageMaster will import.
- `sources/miru/` is reserved for future raw or converted Miru manifests.
- `sources/scripts/` is reserved for future executable JS source scripts.
- This repo is now a clean template so only verified sources are added later.
