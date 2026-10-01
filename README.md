# Singhouse processing packs

Runtime packs that the Singhouse desktop app downloads during setup so it can
process songs from your own library locally on your computer.

This repository holds release assets only. There is no source code here; the
application lives in the main Singhouse repository.

## What a pack contains

- A Python runtime and the third-party open-source Python packages the app
  uses for local audio separation and lyric timing.
- A `notices/` folder with the licence and notice files for every included
  package. Each package remains under its own licence.

## What a pack does not contain

- No model weights. Models are retrieved separately from their upstream
  publishers, only after you review and accept their terms in the app.
- No music, lyrics, or other media.

## Integrity

You do not need to download these files by hand. The app fetches the pack for
your platform, checks every byte against hashes built into the app, and
refuses a pack that does not match.
