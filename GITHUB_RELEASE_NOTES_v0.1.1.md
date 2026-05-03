# LocalFinder v0.1.1

macOS packaging maintenance release.

## macOS packages

- `LocalFinder_0.1.1_aarch64.dmg` for Apple Silicon Macs (M1/M2/M3/M4).

Intel Mac requires a separate x64 build on an Intel macOS runner or an x86_64 Python/Rust toolchain.

## Changes

- Renamed package to architecture-specific macOS naming.
- Added ad-hoc macOS code signing configuration.
- Set minimum macOS version for Apple Silicon package to macOS 11.0.
- Kept app and installer icon aligned with the in-app LocalFinder logo.
- Retained local-only indexing and search behavior.

## Note

This build is ad-hoc signed but not Apple notarized. If macOS still blocks it as an unidentified developer, notarization with an Apple Developer ID certificate is required for a fully trusted public release.
