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

## Download

Grab the latest from [Releases](../../../releases?q=etcdctl-webui&expanded=true) — tags are prefixed `etcdctl-webui-v*`.

| Platform | Asset |
|----------|-------|
| macOS (Apple Silicon) | `etcdctl-webui-darwin-arm64` |
| Linux (x86_64) | `etcdctl-webui-linux-amd64` |
| Docker | see source repo |

## Quick start

```bash
chmod +x etcdctl-webui-*
./etcdctl-webui-darwin-arm64 --endpoints http://127.0.0.1:2379
# open http://localhost:8080
```

## Tech

Go · React · etcd client v3
