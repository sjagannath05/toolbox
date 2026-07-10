# sdm-tools

Dual-pane file browser and copier for hosts behind StrongDM — move files between local and remote without leaving the terminal.

<!-- TODO: add screenshot: ./screenshot-tui.png -->

## Features

- Dual-pane browser (local ⇄ remote), keyboard-driven
- Batch copy with progress
- TUI (Textual) and GUI variants

## Download

Grab the latest from [Releases](../../../releases?q=sdm-tools&expanded=true) — tags are prefixed `sdm-tools-v*`.

| Platform | Asset |
|----------|-------|
| macOS (Apple Silicon) | `sdm-tools-darwin-arm64` |
| Linux (x86_64) | `sdm-tools-linux-amd64` |

**macOS first launch:** if blocked by Gatekeeper: `xattr -d com.apple.quarantine ./sdm-tools-darwin-arm64`

## Tech

Python · Textual (TUI) · PyInstaller single-file builds
