# Cursor AppImage Updater

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

To streamline updates for your Cursor AppImage on Linux, you can use [Gear Lever](https://github.com/mijorus/gearlever), an AppImage manager.

**Setting Up Auto-Updates:**
Gear Lever supports update sources like GitHub releases and static URLs. To enable automatic updates for Cursor, configure the update URL in Gear Lever as follows:

- **For x86_64 systems:**
  ```
  https://github.com/udit-001/cursor-linux-release/releases/download/*/Cursor-*-x86_64.AppImage
  ```

- **For ARM64 systems:**
  ```
  https://github.com/udit-001/cursor-linux-release/releases/download/*/Cursor-*-aarch64.AppImage
  ```

By setting these URLs, Gear Lever will automatically fetch the latest releases. For more detailed instructions, check out the [Gear Lever update guide](https://mijorus.it/posts/gearlever/update-url-info/).


## 📅 Release Status:
- **⏳ Last Released On**: 2025-05-04 00:09:23 UTC
- **🔄 Last Run**: 2025-05-04 00:09:23 UTC
