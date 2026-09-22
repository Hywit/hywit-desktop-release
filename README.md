# Hywit Desktop

Download the Hywit desktop app for Windows, macOS and Linux.

## ⬇️ Download

**[Get the latest version →](https://github.com/Hywit/hywit-desktop-release/releases/latest)**

On the release page, open **Assets** and download the file for your system:

| System | File to download |
|---|---|
| **Windows 11** | `Hywit-Setup-<version>.exe` |
| **macOS – Apple Silicon (M1/M2/M3/M4)** | `Hywit-<version>-arm64.dmg` |
| **macOS – Intel** | `Hywit-<version>-x64.dmg` |
| **Linux – Ubuntu / Debian** | `Hywit-<version>-amd64.deb` |
| **Linux – other distributions** | `Hywit-<version>-x86_64.AppImage` |

> Not sure which Mac you have? Click  → **About This Mac**. If it says **Chip: Apple M…**, choose arm64. If it says **Processor: Intel**, choose x64.

You can ignore the other files on the release page (`.blockmap`, `.yml`, `.zip`, and GitHub's automatic "Source code" links). You don't need them to install Hywit.

## 🛠 Installation

### Windows
1. Run `Hywit-Setup-<version>.exe`.
2. If Windows shows **"Windows protected your PC"**, click **More info → Run anyway**.
3. Hywit installs and opens automatically. You'll find it in the Start menu and on your desktop.

### macOS
1. Open the `.dmg` and drag **Hywit** into **Applications**.
2. The first time you open it, macOS may say it **"cannot be opened"** or **"cannot verify the developer"**:
   - Go to **System Settings → Privacy & Security**, scroll down and click **Open Anyway** next to the Hywit message, **or**
   - run this in Terminal:
     ```bash
     xattr -dr com.apple.quarantine /Applications/Hywit.app
     ```
3. Hywit uses [Homebrew](https://brew.sh) to install Podman. If you don't have Homebrew, install it first.

### Linux
**Ubuntu / Debian (.deb):**
```bash
sudo apt install ./Hywit-<version>-amd64.deb
```

**AppImage:**
```bash
chmod +x Hywit-<version>-x86_64.AppImage
./Hywit-<version>-x86_64.AppImage
```

## 🚀 First launch

The first time Hywit starts, it sets itself up:

- **Podman** (the container engine Hywit runs on) is downloaded and installed automatically if it isn't already on your machine.
- Hywit's backend components are downloaded.

This can take several minutes depending on your internet connection. Later launches are much faste

> **Linux:** installing Podman needs administrator rights. If it's missing, Hywit shows the exact ibution. Run it, then reopen Hywit.

## 🔄 Updating

Download the newest version from the [latest release](https://github.com/Hywit/hywit-desktop-releall it over the existing one.

Your data is **not** stored in the installation folder. It lives in your system's standard app-dat you update Hywit.

## 💻 System requirements

- **Windows:** Windows 11, 64-bit
- **macOS:** Apple Silicon or Intel
- **Linux:** 64-bit (x86_64)
- **Memory:** 8 GB RAM minimum, 16 GB recommended
- **Disk:** at least 20 GB free
- An internet connection for the first launch  
