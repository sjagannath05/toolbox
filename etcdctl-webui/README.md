# etcdctl-webui

A lightweight, self-contained web UI for etcd v3 clusters. One static binary — Go backend with the React frontend embedded via `go:embed`. No nginx, no separate frontend deploy.

Source is public: [sjagannath05/etcdctl-webui](https://github.com/sjagannath05/etcdctl-webui)

<!-- TODO: add screenshot: ./screenshot-tree.png -->

## Features

- Key tree browser with prefix navigation
- Create / read / update / delete keys, JSON formatting
- Multi-cluster support
- mTLS, TLS, and username/password auth
- Import / export

## 🐳 Docker (recommended)

Multi-platform image on GitHub Container Registry (`linux/amd64` + `linux/arm64` — works on Mac, Linux, ARM servers):

```bash
docker pull ghcr.io/sjagannath05/etcdctl-webui:latest
docker run -p 8080:8080 -v ./config.yaml:/config/config.yaml ghcr.io/sjagannath05/etcdctl-webui:latest
```

All tags: [GHCR package page](https://github.com/sjagannath05/etcdctl-webui/pkgs/container/etcdctl-webui)

## 📦 Binaries

Grab the latest from [Releases](../../../releases?q=etcdctl-webui&expanded=true) — tags are prefixed `etcdctl-webui-v*`.

| Platform | Asset |
|----------|-------|
| macOS (Apple Silicon) | `etcd-webui-darwin-arm64` |
| macOS (Intel) | `etcd-webui-darwin-amd64` |
| Linux (x86_64) | `etcd-webui-linux-amd64` |
| Linux (ARM64) | `etcd-webui-linux-arm64` |
| Windows (x86_64) | `etcd-webui-windows-amd64.exe` |

## Quick start

```bash
chmod +x etcd-webui-*
./etcd-webui-darwin-arm64
# open http://localhost:8080
```

**macOS first launch:** if blocked by Gatekeeper: `xattr -d com.apple.quarantine ./etcd-webui-darwin-arm64`

## Tech

Go · React · etcd client v3 · `go:embed` single binary
