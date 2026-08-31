<p align="center">
  <img src="./assets/relief-icon.png" width="128" height="128" alt="Relief app icon">
</p>

<h1 align="center">Relief</h1>

<p align="center"><strong>Understand code changes and the code that depends on them.</strong></p>

<p align="center">
  <a href="https://github.com/yodaiken/relief-releases/releases/tag/nightly"><strong>Download the latest nightly</strong></a>
</p>

Relief is a workspace for exploring a codebase as it changes. It combines a visual code map with a
focused review reader, showing both changes and their dependents across TypeScript, Rust, and Python.

> Relief is very early. Nightly builds may change quickly.

## Install

Relief currently supports **macOS 26 or later on Apple silicon**.

1. Open the [latest nightly release](https://github.com/yodaiken/relief-releases/releases/tag/nightly).
2. Under **Assets**, download the file ending in `_aarch64.dmg`.
3. Open the disk image and drag **Relief** to **Applications**.
4. Double-click **Relief** once. When macOS blocks it, open **System Settings** → **Privacy &
   Security**. Under **Security**, click **Open**, then **Open Anyway**, enter your password, and
   click **OK**.

The current build is ad-hoc signed and isn't notarized yet, so macOS requires the final first-launch
step. After that, you can open Relief normally.

## Updates

Relief checks for future nightly updates automatically. You only need the `.dmg` for a manual
installation; the other release files support the updater:

| File | Purpose |
| --- | --- |
| `Relief_*_aarch64.dmg` | Install Relief on a Mac. |
| `Relief.app.tar.gz` | App payload downloaded by the updater. |
| `Relief.app.tar.gz.sig` | Signature used to verify the updater payload. |
| `latest.json` | Version and download manifest used by the app. |

## Need help?

[Open an issue](https://github.com/yodaiken/relief-releases/issues/new) with your Relief version,
macOS version, and the steps that led to the problem. Don't include private source code, access
tokens, or credentials.

## About this repository

This public repository contains Relief release binaries and updater metadata. It does not contain
the application's source code.
