# GrooveBox changelog

## Update 2 (test checklist)
- [ ] **Liquid glass theme:** frosted translucent cards over colored glow. Theme card, "Liquid glass" toggles it off for pure OLED black.
- [ ] **Embedded album art:** MP3 (ID3v2.3/2.4) and FLAC covers show up; M4A works if the cover is near the start of the file. Accent color follows the art. No art = generated cover.
- [ ] **31-band EQ:** scroll sideways; every band is 1/3 octave (20 Hz to 20 kHz), -12 to +12 dB.
- [ ] **EQ presets:** Flat, Bass boost, Treble boost, Vocal, Rock, Pop, Jazz, Classical, Electronic, Hip-hop, Loudness, Acoustic + Save/Load custom.
- [ ] **Auto lyrics:** pick `song.mp3` and `song.lrc` together; matching names load automatically.
- [ ] **Volume** and **Balance** sliders
- [ ] **-10 / +10 second** skip buttons
- [ ] **Favorites** heart, queue shows hearts, "heart only" filter
- [ ] **Sort A-Z** and **Clear** queue
- [ ] **A-B loop** (tap once for A, again for B, again to clear)
- [ ] **Limiter** (tames loud peaks)
- [ ] **Mono** downmix
- [ ] **Fade-in** on each new track
- [ ] **Keep screen on** toggle
- [ ] **Wave/Bars** visualizer switch
- [ ] **Play counts** are stored per song (not displayed yet)

## Update 1
Cover generator, accent themes, spectrum, .lrc lyrics, karaoke, 10-band EQ, speed/pitch, tube warmth, shuffle, repeat, search, sleep timer.

## Known limits
Word-by-word lyrics, BPM, tag editing, vault, hearing test and DJ tools are not built yet.

## Update 3 (test checklist)
- [ ] **Pages like Musicolet:** bottom bar with Player, Queue, Lyrics, Sound, Settings. A mini player bar shows on every page except Player.
- [ ] **Embedded lyrics:** read from MP3 (USLT synced-less and SYLT synced), FLAC (LYRICS / UNSYNCEDLYRICS / SYNCEDLYRICS tags) and M4A. Synced ones highlight line by line; plain ones show as text. A same-name .lrc file wins over embedded lyrics.
- [ ] **Lyrics page:** full list, current line highlighted and centered, tap a line to jump to it.
- [ ] **Lyrics font:** Default, Serif, Mono, Rounded, Handwriting, Bold, or upload your own .ttf/.otf/.woff2 (custom font must be re-added after reopening). Size slider.
- [ ] **Adaptive background:** glow color fades smoothly when the album art changes. "Glow" slider sets the strength (0 = off).
- [ ] **Audio fidelity:** sample rate (Auto/44.1/48/96 kHz, applies after reopening), EQ width (Narrow/Normal/Wide), Auto headroom (lowers the preamp to match EQ boosts so nothing clips), Pure mode (bypass EQ, filters and warmth).
- [ ] Playback uses the "playback" latency mode for steadier audio.

## Update 3.1 (test checklist)
- [ ] **Smoother:** blur and heavy effects removed, visualizer throttled and paused off-screen, no full-page color animation.
- [ ] **New look:** Tint (adaptive gradient from the art), OLED, Dim and Light themes in Settings. Flat modern cards, big rounded cover.
- [ ] **Custom vector icons** everywhere (no emoji). Layout fills the whole screen; bottom bar sits on the bottom edge.
- [ ] **Track info:** title, artist and album from the file tags show in the player, queue, mini player and lock screen.
- [ ] **Folder picker** (Player page, "Folder"). Songs are scanned in the background for their tags.
- [ ] **Library page:** Queue / Tracks / Playlists tabs. Tracks are sorted by title.
- [ ] **Playlists:** create, add with "+" in Tracks, tap to play, delete. They store song names and reconnect when you pick the folder again.
- [ ] **Fonts:** Apple (SF) and Spotify-style stacks, Roboto, Google Sans, Palatino and more, for lyrics and for the whole app. Custom font upload for lyrics.
- [ ] Coming in 3.2: real crossfade, skip silence, loudness normalization, more quality-of-life.
