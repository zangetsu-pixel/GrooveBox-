# GrooveBox

An offline-first Android music player for people who actually care how their music sounds.

No accounts. No ads. No cloud. Just your files, a pure black screen, and an audio engine that plays the stuff most players give up on.

> **Status: early development.** This repo is at the very beginning. The blueprint is written, the code is not (yet). Everything under "What we're building" is a goal, not a promise that it works today. See the [roadmap](#roadmap) for what's happening first.

---

## Why this exists

Most music players are either pretty but limited, or powerful but ugly. And almost all of them want you online. GrooveBox is an attempt to build the player we wanted ourselves: good-looking on an OLED screen, serious about audio quality, and completely private.

It's also being built entirely from a phone, which is its own kind of adventure.

## What we're building

**Plays almost anything.** FLAC, APE, WavPack, TTA, Musepack and the usual lossy formats, decoded by a native FFmpeg engine instead of whatever the OS happens to support.

**Sounds the way you want.** A layered EQ setup (simple base EQ, graphic EQ, and a 16-band parametric EQ), plus a few small filters for common headphone annoyances: a gentle low-mid cut for muddiness, a sibilance tamer for harsh highs, and crossfeed for easier listening on headphones.

**Looks the part.** True black (#000000) UI to save battery and look great on OLED, with a glassy blur theme that pulls its colors from your album art.

**Covers your way.** A custom cover generator with mosaic layouts and emoji stamps for playlists and albums that don't have good art.

**Lyrics that keep up.** Word-by-word synced lyrics, optional dual-language display, and a vocal-reduction mode for karaoke nights.

**Spatial and warmth effects.** A 3D stage simulator for headphones and a tube-style warmth effect, for when you want it.

**Tidy tags.** Offline fingerprinting, junk-text stripping, filename-to-tag parsing, a BPM analyzer, and an undo stack so you can't wreck your library by accident.

**Private by design.** A locally encrypted vault with biometric lock, local Wi-Fi sharing, and encrypted offline backups. Nothing leaves your phone unless you send it.

## Tech stack

| Layer | What we're using |
|---|---|
| App | React Native, Expo, TypeScript |
| Audio engine | C++ with FFmpeg (libavcodec), bridged through JNI |
| DSP | Custom EQ and filter pipeline in native code |
| Encryption | AES-256-GCM with biometric unlock |
| Builds | Cloud builds through GitHub Actions (no local Android Studio needed) |

Because the audio engine is custom native code, GrooveBox can't run in Expo Go. It needs a development build.

## Roadmap

We're splitting the big feature list into seven blocks and building them in order, starting small.

1. **Core engine and DSP:** the FFmpeg bridge, codec support, EQ, filters
2. **Covers and themes:** cover generator, color extraction, OLED theme
3. **Audio routing and DJ tools:** USB DAC output, pitch and speed controls, gapless playback
4. **Lyrics and visualizers:** synced lyrics, VU meters
5. **Hearing and spatial:** hearing calibration, 3D stage simulator, warmth effect
6. **Tag tools and automation:** fingerprinting, tag cleanup, BPM analysis
7. **Vault and local storage:** encryption, biometric lock, sharing, backups

**First milestone:** a bare-bones app that picks a `.flac` and an `.ape` file and plays both through the native engine. If that works, everything else has something solid to stand on.

## Building it

Builds happen in the cloud with GitHub Actions, so you don't need Android Studio or a computer.

1. Run the FFmpeg workflow once to compile the decoders.
2. Run the app workflow to build the APK.
3. Download the APK from the workflow's artifacts and install it.

The workflows are coming with the first milestone. This section will get real instructions as soon as they exist.

## Contributing

It's very early, so things will move around a lot. Issues, ideas and bug reports are welcome. If you want to send code, open an issue first so we don't step on each other.

## License

GrooveBox is released under the [MIT License](LICENSE).

It uses FFmpeg, which is licensed separately under the LGPL. See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) for details.

## Credits

Built by [Your Name], with help from a couple of AI assistants and a lot of stubbornness.
