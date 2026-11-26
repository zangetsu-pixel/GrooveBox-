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

## Update 3.2 (test checklist)
- [ ] **One tone:** no more boxes or bars in a different shade. Background, player, bottom bar and mini player are all the same surface, separated by hairlines.
- [ ] **True black OLED:** pure #000 everywhere in OLED theme.
- [ ] **Modern controls:** switch toggles in lists, underline tabs, flat rounded buttons, bottom sheet menus.
- [ ] **Song menu (three dots):** Play next, Add to queue, favorite, add to any playlist, plus size/format/album info.
- [ ] **Library:** Albums and Artists tabs (grouped from tags), sort Tracks by A-Z, Most played, Newest.
- [ ] **Fade between tracks** (Settings, Fade slider, 0-12 s). This fades out and in; it is not an overlapping crossfade.
- [ ] **Skip silence:** skips quiet starts, and moves on when the song ends in silence.
- [ ] **Loudness normalization:** uses ReplayGain tags (MP3 and FLAC). Files without tags are left as they are.

## Update 3.5.1 (test checklist)
- [ ] **New minimal interface:** one flat surface, left-aligned large titles, sentence-case labels, white play button, thin progress bar. No boxes or shaded bars.
- [ ] **Live equalizer curve:** drag the curve on the Sound page to shape all 31 bands; a live spectrum moves behind it while music plays.
- [ ] **Compressor** with threshold and ratio you can change while playing.
- [ ] **Reverb** (amount and room size) and **stereo width** (0 to 200%).
- [ ] **New app icon** (a single sound curve on pure black).
- [ ] Accessibility basics: labels on icon buttons, visible keyboard focus, 44 px tap targets, reduced-motion support.

## Update 3.5.2 (test checklist)
- [ ] **Version number:** Settings, About, should say "Version 3.5.2". If it doesn't, the site is showing old files.
- [ ] **Liquid glass is back** (Settings, Theme, Glass; the default after this update). Frosted glass cards over a glow from the album art, no blur effect so it stays smooth.
- [ ] **Player in one glass card** with a glowing cover.
- [ ] **Error messages:** if a song can't play, a message at the top says why. Tell me what it says.
- [ ] **Safe mode** (Settings, Audio fidelity): plays songs with no effects at all. Reopen the app after switching it on.
- [ ] Reverb only runs when its amount is above 0, to save battery and avoid stutter.
- [ ] Old cached files are cleared automatically when the update installs.

## Update 3.5.3 (test checklist)
- [ ] **Gradient behind everything.** The big dark rectangle with square corners behind the cards is gone. The glow now runs edge to edge under the whole app.
- [ ] Cards have clean rounded corners with nothing showing behind them.
- [ ] **Slider tracks and the on/off switch knobs are visible** (the browser's auto dark mode was recoloring them).
- [ ] Brighter accent from dark album art, so the EQ curve and switches stand out.
- [ ] Settings, About says "Version 3.5.3".

## Update 3.6 (Musicolet audio features, test checklist)
- [ ] **Gapless playback** (Settings, Audio fidelity). The next song is loaded early and starts the instant the current one ends. Test with an album that flows song to song.
- [ ] **Crossfade** (Settings, Audio fidelity, Crossfade slider, 0 to 12 s). The end of one song overlaps the start of the next. 0 seconds means gapless.
- [ ] **Output profiles** (Sound, Output profile): Speaker, Headphones, Bluetooth, Car. Each remembers its own equalizer, filters, reverb, width and compressor. Switch by hand; the app can't see which device is connected.
- [ ] **Remember speed for each song** (Settings, Audio fidelity).
- [ ] **Sleep timer upgrades** (Library, Queue): fades the volume out over 15 seconds at the end of a timed sleep, plus "End of this song", "After 3 more songs" and "After 5 more songs".
- [ ] Already there from earlier updates: ReplayGain normalization, reverb, balance, skip silence, 31-band equalizer.
- [ ] Settings, About says "Version 3.6".

## Update 3.7 (test checklist)
- [ ] **Albums page** (bottom bar): grid of albums with cover art. Open one to see its songs **numbered by track** (and disc), sorted like the album. Needs track-number tags in your files.
- [ ] **Playlists page** (bottom bar): All songs, Most played, Recently played, Recently added, Favorites, Never played, then your own playlists below. Tap any to open it, with Play and Shuffle.
- [ ] Library page now has Queue, Tracks, Artists, Genres and Folders. Song menus got "Go to album" and, inside a playlist, "Remove from playlist".
- [ ] **Live themes** (Settings): Starboy, After Hours, Aurora, Sunset, Ocean, Neon city. They glow and drift, and can pulse to the bass. Turn off Animate background if your phone stutters.
- [ ] **Title style** (Settings): Starboy, After Hours, Retro, Serif, Heavy. Inspired by those albums; the real typefaces are licensed.
- [ ] More lyric/app fonts: Starboy style, After Hours style.
- [ ] **Layout**: cover shape (rounded, square, vinyl that spins), density, cover size, corner roundness, text size, lyric alignment, visualizer on/off and rainbow bars, navigation labels on/off, vibrate on tap.
- [ ] More accent colors plus a custom color picker.
- [ ] **Backup**: copy your settings as text and paste them back on another phone or after clearing the browser.
- [ ] Tap the lyrics area on the Player to open the full Lyrics page.
- [ ] Settings, About says "Version 3.7".

## Update 3.8 (test checklist)
- [ ] **Rain theme** (Settings, Live themes): animated rain over a blue-grey glow. **Adaptive (album art)** theme: background glow and colors follow each song's cover.
- [ ] **Three-tier equalizer** (Sound): Base (bass, mid, treble, deep bass), Graphic (31 bands), Parametric (up to 16 nodes, drag the numbered dots on the curve). The curve shows the combined result of all three.
- [ ] **Extra bass:** Bass up to +15 dB with adjustable frequency, plus Deep bass harmonics.
- [ ] **Album cover by majority:** each album uses the cover most of its songs share.
- [ ] **Full-screen lyrics:** tap the album art on the Player. Lyrics sync is now smooth, with Earlier/Later buttons to fix timing.
- [ ] **Visualizer is back and bigger:** tap the style button on the Player (Bars, Wave, Mirror, Radial, Dots, LED).
- [ ] **Wallpaper** (Settings): pick an image, GIF or video to play behind the app; **blur** and dim sliders; or a blurred album art background.
- [ ] **Spatial audio** (headphones) and **ambient sound** (rain, brown noise, white noise) in Sound.
- [ ] Playlists page: Play all, Shuffle all, and a Your listening summary. Tracks tab has search. Player shows format and bitrate, with a Lossless label for FLAC and WAV.
- [ ] Resumes the last song and position when you pick your music again (Settings, can be turned off).
- [ ] Settings, About says "Version 3.8".

## Update 3.9 (test checklist)
- [ ] **Visualizer and equalizer spectrum:** if they don't move, open Sound. A status line says "Audio engine: on", "Safe mode is on" or shows the error. If Safe mode is on, use "Turn off and restart". Safe mode is now switched off for everyone by this update.
- [ ] **Player is only the player:** cover, title, seek, controls, visualizer. The mini lyrics bar is gone. Tap the album art for full-screen lyrics.
- [ ] **Add songs, Add folder and Lyrics file** moved to Library, Folders.
- [ ] **Video and animated wallpapers show behind full-screen lyrics** too.
- [ ] **Word-by-word lyrics:** Enhanced LRC files (word times in angle brackets) highlight each word as it is sung. Normal LRC files get estimated word timing. Switch both in Settings, Lyrics. Lyrics are remembered per song, and you can paste lyrics there too.
- [ ] **Settings reorganized** into sections: Appearance, Wallpapers, Fonts and glow, Audio, Lyrics, Playback, Backup and about.
- [ ] **Glowing text** (Settings, Fonts and glow): any font can glow, with color, size and pulse. About 10 more fonts.
- [ ] **Animated wallpapers** (Settings, Wallpapers): Rain on window (WebGL, drops run down glass over a blurred city), Storm (3D rain with splashes and lightning), Warp stars, Snow, Aurora, Fireflies, Embers, Waves, Bokeh. They use the album art colors.
- [ ] **Rain theme** (Settings, Appearance, Live themes, Rain window) turns on the rain-on-window wallpaper.
- [ ] **More player features:** Bookmarks (Player button, Library tab), fade on pause and resume, shake to skip, remove or move songs in the queue menu.
- [ ] Settings, About says "Version 3.9".

## Update 3.9.1 (fix, test checklist)
- [ ] **Offline install fixed:** the app was missing `manifest.webmanifest`, which made the service worker fail to install. Added the manifest; the service worker now also tolerates a missing file.
- [ ] Open the site once online, then turn on airplane mode and reload: the app should still open.
- [ ] Chrome menu should now offer "Install app" / "Add to Home screen" as a standalone app.
- [ ] Service worker only caches successful responses; cache name bumped to `groovebox-v14` so old files clear out.
- [ ] Settings, About says "Version 3.9.1".

## Update 3.10 (redesign, test checklist)
Navigation is now Home, Library, Player, Sound, Settings.
- [ ] **Lyrics:** tap the album art on the Player and the full lyrics screen opens (it was hidden behind the page before). The back arrow returns.
- [ ] **Player:** the page no longer scrolls. The cover scales to fit the screen.
- [ ] **Seek bar is the visualizer:** bars move with the music, the played part is colored, tap or drag to seek. Style button cycles Mirror, Bars, Wave, Dots. Settings, Player and layout turns it into a plain bar.
- [ ] **Mini player** on every other page: album art, title, artist, previous, play or pause, next, and a progress line. Tap the art or title to open the Player.
- [ ] **Songs with no cover** show the Glacier White GrooveBox wave on a two-tone OLED black cover (also in lists and the mini player).
- [ ] **OLED Black two-tone** is the new base theme: pure black with a slightly lifted black for cards. New Glacier theme. Live themes and wallpapers only tint the background now, the layout stays the same. Theme picker uses preview tiles, accent colors are swatches.
- [ ] **Equalizer rebuilt Musicolet style:** on/off switch, preset chips, 10 vertical bars with dB readout, and a response curve with live spectrum. Fine tune (31 bands, parametric) is under Presets.
- [ ] **Knobs:** Bass boost, Bass freq, Deep bass, Mid, Treble, Presence, Loudness, Virtualizer, Reverb, Preamp. Drag up or down, double tap to reset. Presence and Loudness are new.
- [ ] **Sound is fuller:** stronger presets (new Full sound, Dance, Metal, Lounge, Piano, Headphones, Small speakers), auto headroom no longer cuts the volume as much, and a safety limiter prevents clipping.
- [ ] **Library** works like Your Library: chips for Songs, Albums, Artists, Playlists, Genres, Folders, Queue, Bookmarks. Song rows have cover thumbnails.
- [ ] **Home:** greeting, Play all, Shuffle all, quick tiles (Favorites, Recently played, Most played, Recently added, All songs, Never played), Jump back in, albums, listening stats.
- [ ] **Settings** grouped into Appearance, Player and layout, Wallpapers, Fonts and text, Audio, Lyrics, Playback, Backup and about, each with an icon.
- [ ] **Fonts:** every font is listed in its own typeface with a check mark. Custom font loader and a preview line are included.
- [ ] New custom line icons for navigation and settings.

## Update 3.10.1 (fix: effects engine without Safe mode)
- [ ] With Safe mode off, if any part of the effects engine fails to start on your phone, the app now keeps playing sound normally instead of going silent. The Sound page status line says what failed, and a message shows the reason (send it to me if you see it).
- [ ] The audio engine now resumes itself if Android pauses it, so music no longer stays silent until you toggle something.
- [ ] Settings, About says "Version 3.10.1".

## Update 3.11 (safe mode is now the base)
- [ ] **Basic playback is the default.** Songs play straight through the phone's own player. No effects engine is started, so nothing can silence or break playback. Safe mode is gone as a separate setting.
- [ ] **Effects are opt-in:** in Sound, turn on the equalizer switch (or tap Turn on effects). The Sound effects engine row in Settings, Audio does the same. The bars, knobs, presets, reverb, spatial and crossfade only change the sound while effects are on.
- [ ] If effects fail to start on your phone, playback keeps going without them and the Sound page says why.
- [ ] Your effects setting is reset to off once on first launch. Your other settings stay.
- [ ] Without effects the seek bar still shows the waveform and progress. The live bouncing needs effects on.
- [ ] Turning effects off after they started needs a reopen of the app (use Pure mode to bypass them right away).
- [ ] Settings, About says "Version 3.11".

## Update 3.12 (lean equalizer engine, self-rescue)
- [ ] **Much lighter on your phone.** The effects engine used to run about 50 filters plus spatial, crossfeed, warmth and bass-harmonic processing all the time, even when switched off. Now only the parts you actually use are connected. A flat equalizer runs 2 filters instead of about 50, and Spatial, Crossfeed, Tube warmth and Deep bass cost nothing until you turn them on.
- [ ] **Self-rescue:** if effects are on and music plays but nothing comes out, the app notices within about 3 seconds, switches effects off and keeps playing normally. The Sound page and a message explain it, and effects stay off the next time you open the app.
- [ ] Turn on the equalizer switch in Sound, play something, and move a few bars and knobs. If anything still drops out or sounds wrong, note what you did right before it.
- [ ] Settings, About says "Version 3.12".
