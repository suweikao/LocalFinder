# LocalFinder v0.1.2

Index persistence and storage-path release.

## macOS package

- `LocalFinder_0.1.2_aarch64.dmg` for Apple Silicon Macs (M1/M2/M3/M4).

Intel Mac requires a separate x64 build on an Intel macOS runner or an x86_64 Python/Rust toolchain.

## Changes

- Reuses saved indexes on app startup instead of rebuilding every time.
- Avoids automatic full-home indexing on first launch; users choose directories before indexing starts.
- Changes the toolbar action from rebuild to lightweight sync.
- Simplifies the sidebar index status into a compact progress summary.
- Adds an index storage path selector in the sidebar.
- Stores the real SQLite/FTS index database at the user-selected path.
- Shows the selected index storage path immediately after the user confirms the folder picker.
- Switches search to the selected index database after migration.
- Keeps local-only indexing and search behavior.

## Checksum

`2ce77d1900832559fdf0d205498bac8fb1281e64bae5c77b2729b960d60c50bd  LocalFinder_0.1.2_aarch64.dmg`

## Note

This build is ad-hoc signed but not Apple notarized. If macOS still blocks it as an unidentified developer, notarization with an Apple Developer ID certificate is required for a fully trusted public release.
