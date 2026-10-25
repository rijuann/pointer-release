# MouseShare Official Releases

Official multi-platform release distribution for [MouseShare](https://github.com/rijuann/pointer).

MouseShare enables seamless mouse and keyboard sharing across multiple computers over your local network with sub-millisecond latency.

---

## Downloads (v2.0.0)

### 🪟 Windows (x64)
- **[MouseShare-Setup.msi](https://github.com/rijuann/pointer-release/raw/main/MouseShare-Setup.msi)** (Standard Windows Installer)
  - **SHA-256:** `09b0d145e58bf25a34a578b593b6bb10f0a544e7afff9f1a8a751977f032712a`

### 🐧 Linux (x86_64 / amd64)
- **[mouseshare_2.0.0_amd64.deb](https://github.com/rijuann/pointer-release/raw/main/mouseshare_2.0.0_amd64.deb)** (Debian / Ubuntu / Linux Mint)
  - **Install:** `sudo dpkg -i mouseshare_2.0.0_amd64.deb`
  - **SHA-256:** `1534e18b6d6a183546257ba3f8d4d705d0e06a08f5c3a55ed81e58a6e250b4cf`
- **[mouseshare-linux-x86_64.tar.gz](https://github.com/rijuann/pointer-release/raw/main/mouseshare-linux-x86_64.tar.gz)** (Standalone Tarball - Arch, Fedora, openSUSE)
  - **Install:** `tar -xzf mouseshare-linux-x86_64.tar.gz && cd mouseshare-linux-x86_64 && sudo ./install.sh`
  - **SHA-256:** `22c3f06502175c242bc2e63e4bac27a982a10104094b679469101d32e1b38f38`

### 🍏 macOS (Universal: Apple Silicon M1/M2/M3 + Intel)
- **[MouseShare-macOS-Universal.dmg](https://github.com/rijuann/pointer-release/raw/main/MouseShare-macOS-Universal.dmg)** (Drag & Drop Disk Image)
  - **Install:** Open DMG and drag `MouseShare.app` to `/Applications`
  - **SHA-256:** `9e0726bcd4b92e8b2efc95902d8674d06ec83c3e50840c1bad38c2f6d5139019`
- **[MouseShare-macOS-Universal.app.tar.gz](https://github.com/rijuann/pointer-release/raw/main/MouseShare-macOS-Universal.app.tar.gz)** (Portable App Bundle)
  - **SHA-256:** `25371419e9d2cf450697efe6922128a0c3ac2ad5a2a8106cb73984ce4dbf021d`

---

## Quick Installation & Setup

### Linux uinput Permissions
MouseShare requires access to `/dev/uinput` to emulate mouse events. The installer automatically configures `/etc/udev/rules.d/99-mouseshare.rules`. Ensure your user belongs to the `input` group:
```bash
sudo usermod -a -G input $USER
```
Log out and log back in for permissions to take effect.

### macOS Accessibility Permissions
On macOS, grant Accessibility permissions to MouseShare when prompted:
`System Settings` → `Privacy & Security` → `Accessibility` → Enable `MouseShare`.
