# MouseShare Official Releases

Official multi-platform release distribution for [MouseShare](https://github.com/rijuann/pointer).

MouseShare enables seamless mouse and keyboard sharing across multiple computers over your local network with sub-millisecond latency.

---

## Downloads (v2.0.0)

### 🪟 Windows (x64)
- **[MouseShare-Setup.msi](https://github.com/rijuann/pointer-release/raw/main/MouseShare-Setup.msi)** (Standard Windows Installer)
  - **SHA-256:** `aeab4c56d94a667ca34fb93d0b808c56632e5120e843317b02f4cd23cca19b25`

### 🐧 Linux (x86_64 / amd64)
- **[mouseshare_2.0.0_amd64.deb](https://github.com/rijuann/pointer-release/raw/main/mouseshare_2.0.0_amd64.deb)** (Debian / Ubuntu / Linux Mint)
  - **Install:** `sudo dpkg -i mouseshare_2.0.0_amd64.deb`
  - **SHA-256:** `01d00db162abd6d98c04a06ee256c0687c9f2c33a9225c76fb6c15357ae316a1`
- **[mouseshare-linux-x86_64.tar.gz](https://github.com/rijuann/pointer-release/raw/main/mouseshare-linux-x86_64.tar.gz)** (Standalone Tarball - Arch, Fedora, openSUSE)
  - **Install:** `tar -xzf mouseshare-linux-x86_64.tar.gz && cd mouseshare-linux-x86_64 && sudo ./install.sh`
  - **SHA-256:** `19321145353980fc0ec0d844db7d4d66e228718e203283ff7b6cf08eda5e3273`

### 🍏 macOS (Universal: Apple Silicon M1/M2/M3 + Intel)
- **[MouseShare-macOS-Universal.dmg](https://github.com/rijuann/pointer-release/raw/main/MouseShare-macOS-Universal.dmg)** (Drag & Drop Disk Image)
  - **Install:** Open DMG and drag `MouseShare.app` to `/Applications`
  - **SHA-256:** `2a98e1e932b339db4be819708fc1b46d5bbb72adda1fe72c1609f5edf48a1145`
- **[MouseShare-macOS-Universal.app.tar.gz](https://github.com/rijuann/pointer-release/raw/main/MouseShare-macOS-Universal.app.tar.gz)** (Portable App Bundle)
  - **SHA-256:** `28530fb60a5de03ed1aecf6f1b4f2a9aa29cddf829ae3324908cbf71f8dbb43b`

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
