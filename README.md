# MouseShare Official Releases

Official multi-platform release distribution for [MouseShare](https://github.com/rijuann/pointer).

MouseShare enables seamless mouse and keyboard sharing across multiple computers over your local network with sub-millisecond latency.

---

## Downloads (v1.0.0)

### 🪟 Windows (x64)
- **[MouseShare-Setup.msi](https://github.com/rijuann/pointer-release/raw/main/MouseShare-Setup.msi)** (Standard Windows Installer)
  - **SHA-256:** `f42d2a9f0540252f401ea07ff7ed32b6c6e582868abc60f6fe78039bce42e9f8`

### 🐧 Linux (x86_64 / amd64)
- **[mouseshare_1.0.0_amd64.deb](https://github.com/rijuann/pointer-release/raw/main/mouseshare_1.0.0_amd64.deb)** (Debian / Ubuntu / Linux Mint)
  - **Install:** `sudo dpkg -i mouseshare_1.0.0_amd64.deb`
  - **SHA-256:** `ca447fc3c826c02189f89898231cbc5ef41c2723891088b356aa9e97d5e477ed`
- **[mouseshare-linux-x86_64.tar.gz](https://github.com/rijuann/pointer-release/raw/main/mouseshare-linux-x86_64.tar.gz)** (Standalone Tarball - Arch, Fedora, openSUSE)
  - **Install:** `tar -xzf mouseshare-linux-x86_64.tar.gz && cd mouseshare-linux-x86_64 && sudo ./install.sh`
  - **SHA-256:** `236cb62d35b6e0adc210f6ae96028ee6235728ab705e421aa044e6b927fea113`

### 🍏 macOS (Universal: Apple Silicon M1/M2/M3 + Intel)
- **[MouseShare-macOS-Universal.dmg](https://github.com/rijuann/pointer-release/raw/main/MouseShare-macOS-Universal.dmg)** (Drag & Drop Disk Image)
  - **Install:** Open DMG and drag `MouseShare.app` to `/Applications`
  - **SHA-256:** `4c56024edeb5a0f2c9eead8c9c10aefeaeda8e969fd192c3c72b6a51b7a97c60`
- **[MouseShare-macOS-Universal.app.tar.gz](https://github.com/rijuann/pointer-release/raw/main/MouseShare-macOS-Universal.app.tar.gz)** (Portable App Bundle)
  - **SHA-256:** `edf1a2220d1285ca0a5ed32f54b3d653f836d508b7dd1fdffa48650a31c29fed`

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
