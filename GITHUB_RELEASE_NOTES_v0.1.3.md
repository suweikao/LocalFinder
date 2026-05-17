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
- Redesigns the sidebar into clearer `索引范围`, `索引数据库`, `限定检索`, and `索引状态` sections.
- Replaces the old extension checkbox grid with Everything-style category filters for documents, spreadsheets, presentations, web files, data files, and code.
- Fixes a left sidebar layout issue where long index database paths could overlap the `限定检索` section.
- Reworks filename search to behave more like Everything: scanned files are searchable by filename immediately, even before or without successful content extraction.
- Adds case-insensitive multi-keyword and substring filename matching while keeping filename search separate from full-text search.
- Separates filename metadata indexing from full-text content indexing: visible files are indexed by filename/path metadata, while only supported text-bearing files enter the full-text extraction pipeline.
- Adds an Everything-style filename result table with Name, Path, Size, Date Modified, and Type columns.
- Expands filename filter categories to include images, audio/video, and archives in addition to documents, spreadsheets, presentations, web files, data files, and code.
- Fixes misleading index progress: files that were scanned and processed but failed text extraction now count toward completed progress, while full-text indexed and error counts are shown separately.
- Keeps the simplified compact index status summary introduced in v0.1.2.
- Updates desktop and backend version metadata to `0.1.3`.

## Checksum

`22f6803b1c578a98c63c382e50e6711fb5e5b3d95bfabfbb63a00e9e9f4e34ea  LocalFinder_0.1.3_aarch64.dmg`

## Note

This build is ad-hoc signed but not Apple notarized. If macOS still blocks it as an unidentified developer, notarization with an Apple Developer ID certificate is required for a fully trusted public release.
