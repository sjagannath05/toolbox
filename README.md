# 🧰 Toolbox

Tools I've built — binaries downloadable here. Some sources are private; where a source repo is public, it's linked.

## Tools

| Tool | What it is | Platforms | Latest | Source |
|------|-----------|-----------|--------|--------|
| [DiffDesk](./diffdesk/) | Desktop diff tool with smart parsing of CLI table output (`docker ps`, `kubectl get`, …) | macOS · Windows · Linux | <!-- latest:diffdesk -->[v0.7.0](https://github.com/sjagannath05/toolbox/releases/tag/diffdesk-v0.7.0)<!-- /latest:diffdesk --> | private |
| [etcdctl-webui](./etcdctl-webui/) | Single-binary web UI for etcd v3 — multi-cluster, mTLS | macOS · Linux · Windows · [🐳 GHCR](https://github.com/sjagannath05/etcdctl-webui/pkgs/container/etcdctl-webui) | <!-- latest:etcdctl-webui -->[v1.0.1](https://github.com/sjagannath05/toolbox/releases/tag/etcdctl-webui-v1.0.1)<!-- /latest:etcdctl-webui --> | [public](https://github.com/sjagannath05/etcdctl-webui) |
| [sdm-tools](./sdm-tools/) | Dual-pane file browser/copier for StrongDM hosts (TUI + GUI) | macOS · Linux | <!-- latest:sdm-tools -->–<!-- /latest:sdm-tools --> | private |

## Downloads

All binaries are published as [**Releases**](../../releases) on this repo, tagged per tool:

```
<tool>-v<version>      e.g.  diffdesk-v0.7.0
```

Each tool's folder has install notes, screenshots, and a changelog. `SHA256SUMS` files are attached to each release — verify with:

```bash
shasum -a 256 -c SHA256SUMS
```

### macOS note

Binaries are not notarized (yet). If macOS blocks the app on first launch:

```bash
xattr -d com.apple.quarantine /path/to/downloaded/app
```

## License

Binaries are free to use as-is, for personal and commercial purposes, with no warranty. Source code of private tools remains proprietary; public source repos carry their own licenses.

---

Built by [Jagannath Subramanya](https://www.linkedin.com/in/sjaga) · [GitHub](https://github.com/sjagannath05)
