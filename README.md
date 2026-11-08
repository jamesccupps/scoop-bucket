# James Cupps' Scoop bucket

[![Tests](https://github.com/jamesccupps/scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/jamesccupps/scoop-bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/jamesccupps/scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/jamesccupps/scoop-bucket/actions/workflows/excavator.yml)

My Windows apps for [Scoop](https://scoop.sh), the command-line installer. Every app here is open source (MIT) and
downloaded straight from its own GitHub release, checked against the release's SHA-256.

## Install

```pwsh
scoop bucket add jamesccupps https://github.com/jamesccupps/scoop-bucket
scoop install jamesccupps/slate
```

Update everything with `scoop update *`.

## Apps

| App | Install | What it is |
|---|---|---|
| [Slate](https://github.com/jamesccupps/Slate) | `scoop install jamesccupps/slate` | Fast, simple Notepad replacement that opens files of any size instantly |
| [PingerPlot](https://github.com/jamesccupps/PingerPlot) | `scoop install jamesccupps/pingerplot` | Network path monitor like mtr/WinMTR, with loss, latency and jitter per hop |
| [Protect Panes](https://github.com/jamesccupps/UnifiCameraViewer) | `scoop install jamesccupps/protectpanes` | UniFi Protect live view: each camera in its own borderless window |
| [UniFi Stock Watcher](https://github.com/jamesccupps/UnifiStockWatcher) | `scoop install jamesccupps/unifistockwatcher` | Alerts you when a UniFi product is back in stock on the Ubiquiti Store |
| [HVAC Network Scanner](https://github.com/jamesccupps/HVAC-Network-Scanner) | `scoop install jamesccupps/hvac-network-scanner` | Read-only discovery and audit of building automation networks |
| [NetSentinel](https://github.com/jamesccupps/NetSentinel) | `scoop install jamesccupps/netsentinel` | Network monitor and intrusion detection (needs Npcap) |
| [NoteForge](https://github.com/jamesccupps/NoteForge) | `scoop install jamesccupps/noteforge` | Encrypted, offline, OneNote-style notes |

Settings and data stay in each app's usual folder in your profile (`%APPDATA%`, `%LOCALAPPDATA%` or
`.netsentinel`), so they survive Scoop updates and uninstalls.

## How it stays current

The Excavator workflow checks every app's latest GitHub release every 4 hours and updates the manifest's version, URL
and hash on its own. Something wrong with a manifest? [Open an issue](https://github.com/jamesccupps/scoop-bucket/issues).
