<h1 align="center">
  <img align="top" width="44" src="https://raw.githubusercontent.com/udit-001/cursor-linux-release/refs/heads/main/assets/logo44.png">
  <span>Cursor AppImage Updater</span>
</h1>


<p align="center">
  <a href="https://github.com/udit-001/cursor-linux-release/releases/latest" target="_blank"><img alt="release" src="https://img.shields.io/github/v/release/udit-001/cursor-linux-release?label=release&labelColor=%231e1e2e&color=%234fa048"></a>
  <span> </span>
  <a href="https://github.com/udit-001/cursor-linux-release/actions/workflows/release.yml" target="_blank"><img alt="downloads" src="https://img.shields.io/github/actions/workflow/status/udit-001/cursor-linux-release/release.yml?branch=main&labelColor=%231e1e2e&color=%234fa048"></a>
  <span> </span>
</p>

## Overview

GitHub Action to fetch the latest **Cursor** Linux AppImage and create a release.

## Why?

Cursor on Linux:
- ❌ Doesn’t auto-update
- ❌ Isn’t hosted at a fixed URL
- ✅ Has an API with the latest version info

This makes it hard for Linux users to keep Cursor up to date & this action solves that by:
- Querying Cursor’s API for the latest version
- Checking if that version already exists as a GitHub release
- If not, downloading the AppImage and publishing a release

Linux users can then update via GitHub releases, scripts, or package managers using a consistent URL.

## Setup Auto Updates with Gear Lever

To automate updates for your Cursor AppImage on Linux, use [Gear Lever](https://github.com/mijorus/gearlever). It supports update sources like GitHub releases and static URLs. Configure the update URL based on your system architecture:

- **x86_64**
  ```
  https://github.com/udit-001/cursor-linux-release/releases/download/*/Cursor-*-x86_64.AppImage
  ```

- **ARM64**
  ```
  https://github.com/udit-001/cursor-linux-release/releases/download/*/Cursor-*-aarch64.AppImage
  ```


These URLs will allow automatic fetching of the latest releases. For more detailed instructions, refer to the [update guide](https://mijorus.it/posts/gearlever/update-url-info/).


## 📅 Release Status
- **⏳ Last Released On**: 2025-06-26 01:55:39 UTC
- **🔄 Last Run**: 2025-06-27 01:56:32 UTC
