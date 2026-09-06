# BlobForge

Short comparison videos — X vs Y, Myth vs Fact, Did You Know and five more
formats — written, voiced, rendered and posted from one desktop app. English,
Urdu, Hindi, Arabic, Spanish and five other languages.

## Download

**[⬇ Download BlobForge](https://github.com/awwdil/blobforge-releases/releases/latest/download/BlobForge.zip)** — Windows, ~545 MB

That link always gives you the newest version. It never changes, so it is safe
to bookmark or pass on.

## Getting started

1. **Unzip it** anywhere you like — `D:\BlobForge` is fine. It is not an
   installer; the folder IS the app.
2. **Run `BlobForge.exe`.** The first screen shows your **Machine ID**.
3. **Send that Machine ID to whoever sold you the app.** A licence key comes
   back that works on that one PC.
4. **Paste the key in.** That is the setup finished.

Your videos, topics and settings live in `%LOCALAPPDATA%\Conveyor`, outside the
program folder, so nothing you make is ever touched by an update.

## Updates

You do not download this page again. When a new version is published the app
shows an **Update now** button, fetches only the parts that changed — usually a
fraction of the full download — checks every file against its published
checksum, and replaces itself. Your licence, topics and videos carry over
untouched, and the previous version is kept until the new one has started.

## Two things you supply yourself

- **An AI provider key** (Google Gemini or Groq — both have free tiers) for
  writing topics and translating them. It goes in Settings and stays on your
  PC.
- **A Facebook Page connection**, if you want the app to post for you. Also in
  Settings.

Neither is needed to render videos by hand.

## What is in this repository

No source code. Only what an installed copy needs to update itself:

- `latest.json` — the current version, its download link and its checksum.
  Every installed copy reads this one file and nothing else.
- Releases — the zip for each version, plus `files.json` listing every file in
  that build with its SHA-256, which is what lets an update fetch only the
  parts that actually changed.

Everything published here is checksummed, and the app refuses to install
anything whose checksum does not match.
