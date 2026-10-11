# Forge updates

Forge checks this repository for new versions of its code and installs them itself.

- `stable.json`: the newest version for everyone; `test.json`: a version being tried before it goes out.
- Each version's pack lives on its own branch, `pack-<version>`, in parts of at most 45 MB.
- Every part and the whole pack carry a SHA-256 in the manifest; Forge refuses anything that does not match.

Published with `node scripts/release/release.mjs pack|publish` from the Forge repository.
