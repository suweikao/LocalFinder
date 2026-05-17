# LocalFinder v0.1.4

Empty-state file browsing and metadata index release.

## macOS package

- `LocalFinder_0.1.4_aarch64.dmg` for Apple Silicon Macs (M1/M2/M3/M4).

Intel Mac requires a separate x64 build on an Intel macOS runner or an x86_64 Python/Rust toolchain.

## Changes

- Shows indexed files before the user enters a keyword instead of displaying an empty result area.
- Shows the indexed file list in both `全文` and `文件名` modes when the search box is empty.
- Keeps filename search backed by the metadata index, independent of full-text extraction.
- Keeps the Everything-style table view for file browsing: Name, Path, Size, Modified, and Type.
- Updates desktop and backend version metadata to `0.1.4`.

## Checksum

`4481a4fd46d7df83d04fbe01b87b0dfc000d17deeec645775c7353313a61ab7a  LocalFinder_0.1.4_aarch64.dmg`

## Note

This build is ad-hoc signed but not Apple notarized. If macOS blocks it as an unidentified developer, notarization with an Apple Developer ID certificate is required for a fully trusted public release.
