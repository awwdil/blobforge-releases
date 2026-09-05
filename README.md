# BlobForge releases

Download links and update information for [BlobForge](https://blobforge.app).

This repository holds no source code. It exists so that an installed copy of
BlobForge can check for updates and download them without needing an account,
a token, or a login of any kind:

- `latest.json` — the current version, its download link, and its checksum.
  Every installed copy reads this file and nothing else to decide whether an
  update exists.
- Releases — the installer zip for each version, plus `files.json`, which
  lists every file in that build with its SHA-256 so an install can fetch only
  the parts that changed.

Everything published here is checksummed, and the app refuses to install
anything whose checksum does not match.
