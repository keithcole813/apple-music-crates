# Apple Music Crates — curated by Keith

Every crate is a DJ set I've actually built and played. Each track is
cross-checked against Apple Music — tap any song to open it for streaming.
Songs that aren't on Apple Music are marked.

**Browse the crates:** https://keithcole813.github.io/apple-music-crates/

## What's here

- `index.html` — the crate directory
- `<crate>.html` — one page per crate, with Apple Music links
- `manifest.json` — crate list with track counts

## How it's built

`build_crates.py` (in my workspace) downloads the `.crate` files from
Google Drive, parses them, matches each track against the iTunes Search
API (most-likely match wins, no confident match = flagged as not
available), and generates these pages. Match results are cached so
rebuilds are fast.

Free for now. Playlists curated by a DJ who actually plays them.
