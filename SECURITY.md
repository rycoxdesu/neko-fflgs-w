# Security Policy

## 🛡️ Remote Features

This application includes a remote status check mechanism for safety and stability.

### How it works:
- The app periodically checks a configuration file hosted on GitHub
- This allows us to remotely disable the app if critical bugs are discovered
- Helps protect users from potential issues

### What we collect:
- **Nothing.** No personal data is collected or transmitted.

## 🔄 Updates

- Updates are downloaded directly from GitHub Releases
- The app notifies you when a new version is available
- You have full control over when to update

## 🐛 Reporting Issues

If you find a bug or security issue, please open an issue on GitHub.

## ⚠️ Antivirus False Positives

Some antivirus software may flag this app as suspicious because:
- It modifies process memory (to apply FFlags)
- It's packaged with PyInstaller

This is a false positive. Always download from the official GitHub releases page.
