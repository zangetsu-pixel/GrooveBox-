# Third-Party Notices

GrooveBox is MIT licensed (see [LICENSE](LICENSE)), but it includes or depends on other software with its own licenses.

## FFmpeg

GrooveBox uses libraries from the [FFmpeg](https://ffmpeg.org) project (libavcodec, libavformat, libavutil and libswresample) for audio decoding.

- FFmpeg is licensed under the **GNU Lesser General Public License, version 2.1 or later (LGPL-2.1+)**.
- GrooveBox builds FFmpeg **without** the `--enable-gpl` and `--enable-nonfree` options, so the LGPL applies.
- FFmpeg is linked **dynamically** as shared libraries (`.so` files). You are free to replace them with your own build of FFmpeg.
- The exact build configuration and scripts used to compile FFmpeg for this app are kept in this repository, under the FFmpeg build workflow, so the build can be reproduced.
- FFmpeg source code is available at https://ffmpeg.org/download.html
- A copy of the LGPL is available at https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html

FFmpeg is a trademark of Fabrice Bellard, originator of the FFmpeg project. GrooveBox is not affiliated with or endorsed by the FFmpeg project.

## Other dependencies

GrooveBox is built with React Native, Expo, and other open-source packages, each under its own license (mostly MIT). A full list of dependencies and their licenses will be generated from `package.json` as the project grows.
