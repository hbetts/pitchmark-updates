# Pitchmark updates

Compiled, signed builds that installed copies of Pitchmark download to update themselves.
This repo is written by CI only. It contains no source code.

- `stable/manifest.json` describes the latest build (version, file list, SHA-256 of every file).
- `stable/manifest.sig` is an Ed25519 signature of that manifest. The app refuses any update whose
  signature doesn't match the public key it was built with, and any file whose hash doesn't match.
- `builds/<n>/` holds the files of recent builds.
