# MouseShare Official Releases

Official multi-platform release distribution for [MouseShare](https://github.com/rijuann/pointer).

MouseShare enables seamless mouse and keyboard sharing across multiple computers over your local network with sub-millisecond latency.

---

## Downloads (v2.0.0)

### 🪟 Windows (x64)
- **[MouseShare-Setup.msi](https://github.com/rijuann/pointer-release/raw/main/MouseShare-Setup.msi)** (Standard Windows Installer)
  - **SHA-256:** `5498d4024d204708e9616048748b6dd3df0ad662c1b7726de3e47e792b913009`

### 🐧 Linux (x86_64 / amd64)
- **[mouseshare_2.0.0_amd64.deb](https://github.com/rijuann/pointer-release/raw/main/mouseshare_2.0.0_amd64.deb)** (Debian / Ubuntu / Linux Mint)
  - **Install:** `sudo dpkg -i mouseshare_2.0.0_amd64.deb`
  - **SHA-256:** `a2585fe7e277f97d09c88498b0cf85887987ccb2e62ef7913453ec7e204c30c0`
- **[mouseshare-linux-x86_64.tar.gz](https://github.com/rijuann/pointer-release/raw/main/mouseshare-linux-x86_64.tar.gz)** (Standalone Tarball - Arch, Fedora, openSUSE)
  - **Install:** `tar -xzf mouseshare-linux-x86_64.tar.gz && cd mouseshare-linux-x86_64 && sudo ./install.sh`
  - **SHA-256:** `d827a7b37ba5171441027e70c5b88130b074110f336d42ffa7230121792f0ecc`

### 🍏 macOS (Universal: Apple Silicon M1/M2/M3 + Intel)
- **[MouseShare-macOS-Universal.dmg](https://github.com/rijuann/pointer-release/raw/main/MouseShare-macOS-Universal.dmg)** (Drag & Drop Disk Image)
  - **Install:** Open DMG and drag `MouseShare.app` to `/Applications`
  - **SHA-256:** `c334ab772bb97d178580370396fd65f64a2ab034d0c692dfe5eb34868f89780e`
- **[MouseShare-macOS-Universal.app.tar.gz](https://github.com/rijuann/pointer-release/raw/main/MouseShare-macOS-Universal.app.tar.gz)** (Portable App Bundle)
  - **SHA-256:** `b13a37fa7e5e0b591547f3b9184adfdd3fe5f0b77c90fdcb3f8dbb88f5d3aa37`

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
