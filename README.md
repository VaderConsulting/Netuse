# Netuse

VB6 console-style drive mapper (`NetUseDrive.exe`) built around class `ClassNetUse`. `Sub Main` connects a local drive letter to a UNC share via MPR `WNetAddConnection`, then disconnects with `WNetCancelConnection`, surfacing mapped WNet error strings when either call fails. Sample call uses `K:` against `\\server01\abc`.

**Source last updated:** 2026-08-27 · **Language:** VB6 · **Target:** VB6 Win32 · **Output:** WinForms exe

_Note: original OneDrive LastWriteTime values were wiped to 2026-08-27 by a zip transfer; date above uses best available evidence (headers/copyright where helpful)._

## Solution structure

| Project | Language | Type | Purpose |
|---------|----------|------|---------|
| `NetUseDrive` (`NetUseDrive.VBP`) | VB6 | WinForms exe | Map/unmap network drives via WNetAddConnection / WNetCancelConnection |

## How to open

Open the `.vbp` in Visual Basic 6.0 IDE:
- `NetUseDrive.VBP`

## Requirements

- Visual Basic 6.0 IDE
- Windows MPR (`mpr.dll`) privileges to add or cancel drive connections

## Attribution and provenance

Working copy from my Historical Dev folder `VB/Old/Netuse`.

## License

MIT (c) 2026 VaderConsulting for Dave Robinson's code. See `LICENSE`.
