## 🎉 Presence Manager v1.0.0 — First public release

**A modern Windows application for creating and managing custom Discord Rich Presence.**

Set up your Discord status with custom text, activity type, images, timers and buttons — Presence Manager connects to Discord automatically and keeps your presence in sync.

---

### ✨ What's new in v1.0.0

**Rich Presence editor**

- Custom **Details** and **State** text.
- Activity type: **Playing / Listening / Watching / Competing**.
- **Large and small images** with hover text (using your Discord app's Rich Presence assets).
- **Timers**: elapsed time, remaining time, or no timer — the elapsed counter can start when you activate the presence or at a **specific date and time** (e.g. already counting since 3 hours ago).
- Up to **2 custom buttons** with label and URL.

**Convenience & automation**

- **Presets** — save named combinations of all fields and apply them instantly with one click.
- **Automatic Discord detection** — monitors whether Discord is open (stable, PTB and Canary).
- **Automatic reconnection** — reconnects and re-applies your presence automatically when Discord opens.
- **Test Connection** button to check the state at any time.

**Application**

- **System tray** — minimize to the tray, keep running in the background, apply or toggle the presence from the tray menu.
- **Start with Windows** — optional, no administrator privileges required.
- **Light / Dark / System themes** — modern Windows 11 style interface.
- **Persistent settings** — everything is saved locally in JSON (`%AppData%\PresenceManager`).
- **Open settings folder** button — easy backup or migration to another PC.
- 100% free, no telemetry, no analytics, no server.

---

### 📦 Download

| File | Type | Architecture |
| --- | --- | --- |
| [PresenceManager-Portable-x64.exe](#) | Portable | 64-bit |
| [PresenceManager-Portable-x86.exe](#) | Portable | 32-bit |
| [PresenceManager-Setup-x64.exe](#) | Installer | 64-bit |
| [PresenceManager-Setup-x86.exe](#) | Installer | 32-bit |

> Replace the `#` links with the actual asset links after uploading the files (or remove them — the GitHub UI already shows the files below).

**Which one should I download?**

- **x64** — most Windows computers (64-bit). Recommended for the vast majority of users.
- **x86** — only for 32-bit systems or older machines.
- **Portable** — no installation needed. Download, run and it's ready. Perfect for USB drives or temporary use.
- **Setup** — installs Presence Manager on your PC (Start Menu access, etc.).

All builds are **self-contained**: the .NET runtime is included, so **no extra installation is required**.

---

### 🚀 Installation

**Portable version**

1. Download `PresenceManager-Portable-x64.exe` (or `-x86`).
2. Run the executable directly — no installation needed.
3. Your settings are stored in `%AppData%\PresenceManager`, so updating (replacing the file) keeps your configuration intact.

**Setup version**

1. Download `PresenceManager-Setup-x64.exe` (or `-x86`).
2. Run the installer and follow the instructions.
3. Launch Presence Manager from the Start Menu or desktop shortcut.

---

### ⚙️ Requirements

- **Windows 10 or Windows 11** (64-bit for `x64`, 32-bit for `x86`).
- **Discord Desktop** installed and running — Presence Manager needs Discord open to apply the presence.
- An internet connection while connecting to Discord.
- No .NET runtime required (self-contained builds).

---

### 🎮 First-time setup (Discord)

Presence Manager uses Discord's official Rich Presence feature, which requires an **Application ID** from the [Discord Developer Portal](https://discord.com/developers/applications):

1. Open the [Discord Developer Portal](https://discord.com/developers/applications).
2. Click **New Application**, give it a name, and create it.
3. Copy the **Application ID** from the application's general information page.
4. In Presence Manager, open the **Presence** page and paste the Application ID.
5. To use images in your presence, add them as **Rich Presence Assets** (Developer Portal → *Rich Presence → Art Assets*) and use their names as image keys.

You can also open the Developer Portal directly from the application — the **Presence** page has a "Developer Portal" shortcut button.

---

### 💡 Quick usage

1. Open Presence Manager.
2. Go to the **Presence** page and paste your **Application ID**.
3. Fill in the fields you want (text, activity type, images, timer, buttons).
4. Click **Save Configuration**.
5. Make sure Discord Desktop is running.
6. Click **Apply Presence** — done!

You can check the connection state on the home page (Discord connected/disconnected, presence active/inactive, last update).

---

### 📖 Resources

- [README](https://github.com/MaelllDev/PresenceManager#readme) — full documentation
- [Troubleshooting guide](https://github.com/MaelllDev/PresenceManager/blob/main/docs/TROUBLESHOOTING.md)
- [Report a bug](https://github.com/MaelllDev/PresenceManager/issues/new?template=bug_report.md)
- [Request a feature](https://github.com/MaelllDev/PresenceManager/issues/new?template=feature_request.md)

---

<sub>Presence Manager is **proprietary software** — all rights reserved. Source code is not public.</sub>
<sub>Made with ❤️ by [MaellDev](https://github.com/MaelllDev)</sub>
