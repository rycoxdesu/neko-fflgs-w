# Security Policy

We take the security and stability of **Neko's FastFlags Saver** seriously. This document explains the remote features and how we handle updates.

## 🛡️ Remote Features & Safety Switch

This application includes a **Remote Status Check** mechanism.

### How it works:
1. Upon launch and periodically, the app fetches a `status.json` file from our official GitHub repository.
2. This file contains:
   - **Status Flag:** Determines if the app is safe to run.
   - **Announcements:** Messages from the developer.
   - **Version Info:** Checks for the latest available version.

### Why do we need this? (The "Kill Switch")
If a critical bug is discovered that could harm your computer or get your Roblox account banned, we can **remotely disable the application** immediately. This is a safety measure to protect users from faulty updates or detected risks.

**We DO NOT:**
- Access your personal files.
- Upload your data to any server.
- Execute arbitrary code remotely without your consent (updates require user action).

## 🔄 Update Mechanism

Updates are **only** fetched from the official GitHub Releases page.
- The app downloads the new executable directly from GitHub.
- The app **does not** automatically replace system files. It downloads the new version as a separate file and asks YOU to switch to it.
- This ensures you always have control over which version you are running.

## 🐛 Reporting Vulnerabilities

If you find a security issue or a bug, please open an issue on our GitHub repository or contact the developer directly.

## ⚠️ False Positives (Antivirus)

Because this app modifies Roblox processes (to apply FastFlags) and is written in Python (PyInstaller), some antivirus software might flag it as a false positive.
- We recommend adding an exclusion for the app folder.
- Always download from the official releases page.
