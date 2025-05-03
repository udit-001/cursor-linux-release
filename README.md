# Cursor AppImage Updater

A GitHub Action that automates fetching the latest **Cursor** Linux AppImage and creates a GitHub release—**only if one doesn't already exist**.

## ❓ Why This Exists

As of now, **Cursor does not support auto-updates on Linux**. The provided AppImage:

- ❌ Does **not** have a built-in update mechanism  
- ❌ Is **not** hosted at a stable URL that always points to the latest version  
- ✅ However, Cursor **does provide an API** that returns a JSON response with the latest version info and download link

This GitHub Action bridges the gap by:

- Automatically fetching the latest version
- Creating a GitHub Release with a stable AppImage link
- Allowing Linux users to **auto-update Cursor** via GitHub releases or package scripts

## 📦 What It Does

- Runs daily at midnight (UTC)
- Fetches the latest stable Cursor version info via API
- Checks if a GitHub release with that version already exists
- If not, downloads the AppImage and creates a new release

## 📅 Release Status:
- **⏳ Last Released On**: 2025-05-03 23:30:55 UTC
- **🔄 Last Run**: 2025-05-03 23:34:09 UTC
