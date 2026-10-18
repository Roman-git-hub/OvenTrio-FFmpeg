# OvenTrio-FFmpeg

Custom Windows x64 FFmpeg tools and a modified FFplay build for Oven Trio Studio.

This is an independent distribution based on the official FFmpeg project. It is not an official FFmpeg release.

## Included

Each release provides a versioned ZIP archive containing the FFmpeg tools and runtime files used by Oven Trio Studio, including:

- `ffmpeg.exe` for media processing.
- `ffprobe.exe` for media inspection.
- A customized `ffplay.exe` with SDL playback controls.
- The DLLs and other runtime components required by that build.

The modified FFplay build supports queued playback using one FFplay process. It can advance to the next queued file while keeping the player process and SDL window open. The Repeat control is available in the player window.

Supported formats and codecs depend on the components enabled in each release. Check that release’s build notes for the exact configuration.

## Downloads

Download the Windows x64 ZIP archive from the repository’s **Releases** section.

Each release should include:

- The versioned Windows x64 binary archive.
- A `SHA256SUMS.txt` file with the archive’s SHA-256 checksum.
- Build notes listing the FFmpeg version, source commit, configuration, toolchain, and included third-party components.
- The corresponding source package and build instructions, as described under **Source and build information**.

SHA-256 checksums help verify that a downloaded file matches the published release. They do not, by themselves, authenticate who published it.

## Source and build information

FFmpeg is based on the official FFmpeg source code:

- Project website: <https://ffmpeg.org/>
- Official source repository: <https://git.ffmpeg.org/ffmpeg.git>

Each binary release must be accompanied by source materials corresponding to that exact build. The source materials include the matching upstream FFmpeg version, OvenTrio-specific patches, build configuration, and instructions needed to reproduce the build.

See the matching release’s source archive and build notes. A link to upstream FFmpeg alone does not include OvenTrio-specific modifications.

## Licensing and third-party notices

FFmpeg and the components included in each build are provided under their respective licenses. The applicable terms depend on the exact build configuration and its dependencies.

The currently tested FFmpeg 9.0.2 build was configured without `--enable-gpl` and `--enable-nonfree`. Each release must still be checked against its actual configuration and included components before its license is stated.

The matching release includes the applicable license texts and third-party notices. The FFmpeg source and modifications remain subject to their applicable FFmpeg license terms. This repository’s GitHub license setting does not replace or override those terms.

This repository does not claim ownership of FFmpeg or its third-party components.

## Compatibility

These builds are intended primarily for use with Oven Trio Studio. Compatibility with other applications is not guaranteed.

## Disclaimer

FFmpeg is an independent project. OvenTrio-FFmpeg is not affiliated with or endorsed by the FFmpeg project.

## Project

**OvenTrio-FFmpeg**  
Customized multimedia tools for Oven Trio Studio.
