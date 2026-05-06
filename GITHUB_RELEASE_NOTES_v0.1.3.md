# LocalFinder v0.1.3

Index lifecycle and cleanup release.

## macOS package

- `LocalFinder_0.1.3_aarch64.dmg` for Apple Silicon Macs (M1/M2/M3/M4).

Intel Mac requires a separate x64 build on an Intel macOS runner or an x86_64 Python/Rust toolchain.

## Changes

- Fixes a stale-index bug: removing an index directory now also removes files indexed from that directory.
- Avoids false path matches when cleaning files under similarly named folders.
- Keeps first-launch indexing explicit: the app waits for the user to choose folders instead of starting a long automatic home-directory index.
- Keeps the toolbar action as non-destructive index sync rather than clearing and rebuilding the index.
- Keeps the simplified sidebar status summary introduced in v0.1.2.
- Updates desktop and backend version metadata to `0.1.3`.

## Checksum

`0e993f7ed778242269eed821ef46ff444a27de69f4b9ae66447a6b8b3ddf3bac  LocalFinder_0.1.3_aarch64.dmg`

## Note

This build is ad-hoc signed but not Apple notarized. If macOS still blocks it as an unidentified developer, notarization with an Apple Developer ID certificate is required for a fully trusted public release.
