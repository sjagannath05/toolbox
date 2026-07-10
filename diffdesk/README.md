# DiffDesk

Cross-platform desktop diff tool that understands the output you actually paste into it.

<!-- TODO: add screenshot: ./screenshot-main.png -->

## Why another diff tool?

Most diff tools treat everything as plain text. DiffDesk adds:

- **Smart table parsing** — paste fixed-width CLI output (`docker ps`, `kubectl get pods`, `ls -l`) and DiffDesk detects columns, letting you diff by column instead of by character
- **CSV column picker** — choose which columns matter before diffing
- **Unified & split views** with syntax highlighting (Monaco editor)
- Fast, native, offline — no data leaves your machine

## Download

Grab the latest from [Releases](../../../releases?q=diffdesk&expanded=true) — tags are prefixed `diffdesk-v*`.

| Platform | Asset |
|----------|-------|
| macOS (Apple Silicon) | `DiffDesk_<ver>_aarch64.dmg` |
| macOS (Intel) | `DiffDesk_<ver>_x64.dmg` |
| Windows | `DiffDesk_<ver>_x64-setup.exe` / `.msi` |
| Linux | `DiffDesk_<ver>_amd64.AppImage` / `.deb` |

**macOS first launch:** if blocked by Gatekeeper: `xattr -d com.apple.quarantine /Applications/DiffDesk.app`

## Tech

Tauri 2 · React 19 · TypeScript · Monaco

## Changelog

### v0.7.0
- Smart table parser for fixed-width CLI output
- CSV column picker
- Unified/split view toggle
