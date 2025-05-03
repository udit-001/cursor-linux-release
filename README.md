# Cursor AppImage Updater

GitHub Action to fetch the latest **Cursor** Linux AppImage and create a release.

## Why?

Cursor on Linux:
- ❌ Doesn’t auto-update  
- ❌ Isn’t hosted at a fixed URL  
- ✅ Has an API with the latest version info

This makes it hard for Linux users to keep Cursor up to date.

This action solves that by:

- Querying Cursor’s API for the latest version
- Checking if that version already exists as a GitHub release
- If not, downloading the AppImage and publishing a release

Linux users can then update via GitHub releases, scripts, or package managers using a consistent URL.

## 📅 Release Status:
- **⏳ Last Released On**: 2025-05-03 23:51:33 UTC
- **🔄 Last Run**: 2025-05-03 23:51:33 UTC
