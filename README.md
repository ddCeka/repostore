<div align="center">
  <img src="app/src/main/res/mipmap-xxxhdpi/ic_launcher_round.webp" width="200" alt="Project logo"/>
</div>

<h1 align="center">RepoStore</h1>

<p align="center">
  RepoStore is a GitHub-powered Android app store that discovers repositories shipping real installable APKs and lets you install, track, and update them from one place.
</p>

---

> [!CAUTION]
> Free and Open-Source Android is under threat. Google will turn Android into a locked-down platform, restricting your essential freedom to install apps of your choice. Make your voice heard – [keepandroidopen.org](https://keepandroidopen.org/).

## ✨ What is RepoStore?       

RepoStore is a native Android app that turns GitHub releases into a clean, Play Store style experience:

- Only shows repositories that actually provide installable APK assets.
- Detects installed apps and shows update availability.
- Always installs from the latest published release with changelog.
- Presents a polished details screen with stats, README, and developer info.

---

## 🚀 Features

- **Smart Discovery**
  - Home sections for "Trending", "Recently Updated", and "Featured" projects.
  - Only repos with valid APK assets are shown.
  - Category-based filtering for apps.

- **Latest-Release Installs**
  - Fetches `/releases/latest` for each repo.
  - Shows only assets from the latest release.
  - Single "Install" action with download progress.

- **Rich Details Screen**
  - App name, version, "Install" button.
  - Stars, forks, language stats.
  - Rendered README content ("About this app").
  - Latest release notes with markdown formatting.
  - Screenshot gallery with fullscreen viewer.

- **Install & Update Tracking**
  - Opens APK downloads with the package installer.
  - Tracks installations and shows "Open" for installed apps.
  - Detects when updates are available.

- **Appearance & Theming**
  - Material 3 design with Material You support.
  - Dark mode with system theme support.
  - Clean, Play Store inspired UI.

- **GitHub Integration**
  - Optional GitHub sign-in via OAuth device flow.
  - Increases API rate limit from 60 to 5,000 requests/hour.
  - View developer profiles and repositories.

- **Support Developer**
  - UPI payment integration with QR code.
  - Detects installed UPI apps (GPay, PhonePe, Paytm, etc.).
  - One-tap payment support.

---

## 🔑 Configuration

### GitHub OAuth (Optional)

To enable GitHub sign-in for increased API limits:

1. Create a GitHub OAuth app at **GitHub → Settings → Developer settings → OAuth Apps**.
2. Copy the **Client ID** from the OAuth app.
3. Update in `GitHubAuth.kt`:

```kotlin
private const val CLIENT_ID = "your_client_id_here"
```

---

## 📄 License

RepoStore is released under the **MIT License**.

```
MIT License

Copyright (c) 2026 Samyak Kamble

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---
