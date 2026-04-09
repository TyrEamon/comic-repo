# Source Directory

This folder is the payload that ImageMaster syncs into the local user source directory.

Current policy:
- keep `index.json` empty until a source is verified usable
- add only sources that are confirmed working after conversion/testing
- do not keep bulk imported Miru manifests here by default

Folders:
- `miru/`: optional staging area for raw or converted Miru manifests
- `scripts/`: optional JS source scripts for ImageMaster external sources

When adding a new source:
1. put its manifest in `sources/` or `sources/miru/`
2. put its runtime JS in `sources/scripts/` if needed
3. add the manifest path into `sources/index.json`
