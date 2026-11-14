# ffmpeg-mirror

Unmodified copy of a static FFmpeg build from [BtbN/FFmpeg-Builds](https://github.com/BtbN/FFmpeg-Builds), kept here so
a pinned build stays downloadable after the upstream daily release is pruned (BtbN keeps only the last 14 daily builds).

| | |
| --- | --- |
| Upstream release | https://github.com/BtbN/FFmpeg-Builds/releases/tag/autobuild-2026-11-06-12-50 |
| File | `ffmpeg-n8.1.3-34-ga35157abb9-linux64-gpl-8.1.tar.xz` (152,360,560 bytes) |
| sha256 | `2d17c1f53aa6e15882ff76d2a0089d63c3553a401bf2bdc723d798beb5eb4f1b` |
| Stored as | `autobuild-2026-11-06-12-50/<file>.part00` + `.part01` (split below GitHub's 100 MB file limit) |

Rebuild the original file and check it:

```sh
cat ffmpeg-n8.1.3-34-ga35157abb9-linux64-gpl-8.1.tar.xz.part00 ffmpeg-n8.1.3-34-ga35157abb9-linux64-gpl-8.1.tar.xz.part01 \
    > ffmpeg-n8.1.3-34-ga35157abb9-linux64-gpl-8.1.tar.xz
sha256sum -c SHA256SUMS
```

## Licence and source

The binaries are FFmpeg built with `--enable-gpl --enable-version3`: GPL-3.0-or-later (full text: `LICENSE.txt` inside
the archive). Nothing was changed; this repository only redistributes the upstream archive.

- FFmpeg source: commit `a35157abb9` (n8.1.3-34, release/8.1), https://github.com/FFmpeg/FFmpeg/tree/a35157abb9
- Build scripts and the exact sources / versions of every bundled library: https://github.com/BtbN/FFmpeg-Builds
