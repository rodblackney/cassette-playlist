# cassette-playlist

Dub a Spotify playlist onto a screenprinted cassette and share it as a link.

**Live:** https://rodblackney.github.io/cassette-playlist/

- Paste a Spotify playlist, album or track link; the cassette plays it, reels spin and wind with the track.
- Write on the tape: click any text to select, drag to move, pull the corner to resize, click again to retype.
- Pick a handwriting, brand, type, length and colourway.
- **Copy share link** saves the whole tape in the URL hash, so no server or account. Anyone who opens it gets a listen-only view.
- **Download PNG** exports the tape at 2×.

Single `index.html`, no build step. Serve it over http (the Spotify player won't load from `file://`):

```bash
python3 -m http.server 8791
```

Listeners who aren't logged into Spotify in their browser hear 30-second previews.
