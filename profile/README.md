<p align="center">
  <img src="https://raw.githubusercontent.com/RustChrome/RustChrome/main/assets/logo-512.png" width="120" alt="RustChrome">
</p>

<h1 align="center">RustChrome</h1>

<p align="center">
  <b>A fast, private, Chrome-familiar browser written in Rust.</b><br>
  No telemetry. No accounts. No sync servers. Open source, MIT.
</p>

<p align="center">
  <a href="https://github.com/RustChrome/RustChrome/releases"><b>Download</b></a> ·
  <a href="https://github.com/RustChrome/RustChrome">Source</a> ·
  <a href="https://github.com/RustChrome/RustChrome/issues">Issues</a> ·
  <a href="https://github.com/RustChrome/RustChrome/blob/main/LICENSE">MIT License</a>
</p>

---

### What we're building

A browser that treats your machine as yours. RustChrome keeps the interface you already
know — tabs, omnibox, bookmarks, per-tab zoom — and boots private by default:

- **Tor-style anti-fingerprinting** — one generic machine profile for every user: fixed
  user agent, pinned screen/CPU/RAM/locale/timezone, canvas noise, WebGL off, WebRTC
  closed, every permission denied.
- **Sessions that don't outlive the window** — closing the browser wipes cookies,
  localStorage, IndexedDB, service workers, caches and HSTS before it exits.
  **New identity** does the same on demand.
- **No history database. Zero telemetry.** Nothing to leak, sync or subpoena.

### The footprint

| | |
|---|---|
| Binary | ~800 KB (stripped), links against system GTK3 + WebKitGTK 4.1 |
| Cold start | ~0.5 s |
| Idle CPU | ~0% |
| Processes | one — no daemons, no proxies, no background services |

### Repositories

- **[RustChrome](https://github.com/RustChrome/RustChrome)** — the browser.

---

<p align="center"><sub>Built with Rust, GTK3 and WebKitGTK. MIT licensed.</sub></p>
