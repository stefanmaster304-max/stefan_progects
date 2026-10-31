# Dangerous World update feed

`manifest.json` is fetched by the installed game at startup when update checks are enabled. The current entries report the versions shipped with this source tree; they do not advertise downloadable updates.

To publish a release, attach these assets to a public GitHub Release and add each available asset's direct download URL, exact byte size, and SHA-256 digest to its manifest entry:

- `game`: the Windows executable `dw.exe`.
- `contents`: the encrypted `settings/contents.dat` bundle.
- `maps`: the encrypted `settings/maps.dat` bundle.
- `sounds`: a ZIP whose extracted root is the complete replacement `sounds/` tree (or contains one top-level `sounds/` directory).

Example entry:

```json
"contents": {
  "version": "1.0.1",
  "url": "https://github.com/OWNER/REPOSITORY/releases/download/v1.0.1/contents.dat",
  "size": 123456,
  "sha256": "lowercase-64-character-sha256"
}
```

Only entries with a newer version and a non-empty `url` are offered. The updater validates the downloaded length and SHA-256 when supplied; encrypted content and map files are decrypted for format validation before installation. Keep every asset versioned and immutable after publication.
