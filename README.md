# Relief — releases

Release binaries and auto-updater manifests for **Relief**. The source lives in a private
repository; this repo exists so the desktop app can fetch updates over a plain, unauthenticated
download.

## Install

Grab the latest `.dmg` from [**Releases**](../../releases). macOS Apple Silicon only for now, and
builds are currently **unsigned** — on first launch, right-click the app → **Open** (or run
`xattr -dr com.apple.quarantine /Applications/Relief.app` once).

## Auto-update

The app updates itself via [`tauri-plugin-updater`](https://v2.tauri.app/plugin/updater/), verifying
each download against a minisign key baked into the app — so these binaries can be downloaded by
anyone but **can't be tampered with**. It polls:

- **nightly** (rolling, from `main`) — `releases/download/nightly/latest.json`
- **stable** (tagged) — `releases/latest/download/latest.json`

## Channels

- `nightly` — published as a GitHub *pre-release* under a rolling `nightly` tag.
- `stable` — tagged `vX.Y.Z` releases.
