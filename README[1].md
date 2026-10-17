# Neurix Group — Official Releases

This public repository is the planned distribution catalogue for **Neurix AI** in **Neurix Hub**.

**Status: preparation only.** No installers have been published and online distribution is not active yet.

## Files

- `catalog/versions.json` — machine-readable catalogue; initially empty.
- `catalog/schema.json` — JSON Schema for catalogue validation.
- `docs/PUBLISHING.md` — manual release checklist.

## Planned workflow

1. Build and test the Windows installer.
2. Review the binary, compute its SHA-256, and **explicitly approve public distribution**.
3. Publish the installer in a GitHub Release.
4. Add the verified metadata to the catalogue.
5. Neurix Hub fetches the catalogue, downloads installers on user request, verifies hashes, and stores checked installers in its cache.

Your private source repositories can stay private. Never upload `.env` files, secrets, local user databases, or private source archives to this public repository.

SHA-256 and HTTPS guard against data corruption and mismatches; a checksum hosted in the same repository is not independent code authenticity verification. Do not bypass Windows security warnings.
